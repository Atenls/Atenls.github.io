# 属性与相关计算公式

## 属性

|属性全称|简称 |  描述  |备注|
|-----   |:---:|   :---:   |  ----  |
|MeleeDamage |`D`| 近战伤害|存在 $\small D_{min}$ & $\small D_{max}$|
|ArrowDamage |`AD`| 箭矢伤害|存在 $\small AD_{min}$ & $\small AD_{max}$
|MagicDamage |`MD`| 魔法伤害|存在 $\small MD_{min}$ & $\small MD_{max}$
|Health|`HP`|生命值|通常情况下指生命值上限，即$\small HP_{max}$
|HealthRegen|`HPR`|生命恢复
|Armor |`A`| 护甲
|ArmorPenetration |`AP`| 护甲穿透
|Mana|`MANA`|法力
|MagicPenetration |`MaP`| 魔法穿透
|ManaRegen|`MR`|法力恢复
|HealthSteal|`HS`|生命偷取/吸血|百分比$\%$数值
|DamageReduse |`R`| 减伤|非固定值，关联 `A` `L` ，百分比/数值
|MagicDefense |`MaD`| 魔法抗性
|MagicReduse |`MaR`| 减伤|非固定值，关联 `MaD` `L` ，百分比/数值
|Knowing |`K`| 会心
|Flexible |`F`| 柔韧
|CriticalChance|`C`|暴击几率|非固定值，关联 `K` `F` ，百分比$\%$数值
|CriticalResistance|`CR`|抗暴击率|非固定值，关联 `K` `F` ，百分比$\%$数值
|Hit |`H`| 命中
|Dodge |`D`| 闪避
|DodgeChance|`DC`|闪避几率|非固定值，关联 `H` `D` ，百分比/数值
|HitChance|`HC`|命中几率|非固定值，关联 `H` `D` ，百分比/数值
|CritDamage|`CD`|暴击伤害|百分比$\%$数值
|ElementIncrease |`EI`| 元素强化
|WholeElementIncrease | / | 全元素强化|又称全属性强化，同时强化四项元素属性
|ElementDefense |`ED`| 元素抗性
|WholeElementDefense | / | 全元素抗性|又称全属性抗性，同时提升四项元素抗性

<table>
    <tr>
        <th>$X_a$</th>
        <th>$Attribute_a$ 对象$a$ 意为玩家的属性</th>
    </tr><tr>
        <th>$X_b$</th>
        <th>$Attribute_b$ 对象$b$ 意为目标的属性</th>
    </tr>
</table>

**※** *关联属性详见下方公式 此简称并无较大实用意义，仅作避免本文行文冗长或公式混淆之用。*

---

## 计算公式(中文)


For English version, please refer to the latter part of this docs.

?> 受限于早期技术力等问题，大部分内容通过多项式拟合指数函数效果，已形成根深蒂固的路径依赖，无法变更。

!> 中文文稿为较早期(2019)最终修订内容，尽管无甚变更，但或仍将存在部分细微错误内容，如有出入，请以英文版为准。


- **伤害** *(Melee/Arrow/Maigc Damage)*


- `近战伤害` 以空手或物品对目标攻击命中后造成的伤害，伤害($\small {D_{min} \thicksim D_{max}}$)，最终伤害公式为

    $D_a^1=D_a·(1-R_b\%)$

- `箭矢伤害` 以箭矢对目标攻击命中后造成的伤害，伤害($\small {AD_{min}\thicksim AD_{max}}$)，最终伤害公式为

    $AD_a^1=\dfrac{AD_a·(1-R_b\%)}{3}$

- `魔法伤害` 以法杖对目标攻击命中后造成的伤害，伤害($\small {MD_{min} \thicksim MD_{max}}$)，最终伤害公式为

    $MD_a^1=MD_a·(1-MaR_b\%)$

`近战伤害` `箭矢伤害` 参与 `命中` `暴击` `护甲穿透`判定

所有伤害均 参与 `属性强化` `生命偷取` 判定

`魔法伤害` 参与 `魔法穿透` 判定

下文中参与公式或提到的$\small D$，如无特殊说明，则一般为三项伤害


-----

- **元素** *(Elements)*

    共有 `光` `暗` `火` `冰` 四项，且分别独立

    攻击时仅计算手持武器之属性的增益伤害，其余不做计算，增益公式为

    $D_{a}^1=D_a\times\;\dfrac{1+(EI_a-ED_b)}{1000}$

-----

- **减伤** *(DamageReduse & MagicReduse)*

    基于护甲 `A` 和 等级 `L` 计算得出的百分比$\%$数值，计算公式为

    $R_a=\dfrac{A_a}{ A_a + 420 + 8.4·( \frac{9}{1000}L^3 - \frac{63}{250}L^2 + \frac{21}{2}L)}\times\;100\%$

    同理，魔法减伤计算公式为

    基于魔法抗性 `MaD` 和 等级 `L` 计算得出的百分比$\%$数值

    $MaR_a=\dfrac{MaD_a}{ MaD_a + 420 + 8.4·( \frac{9}{1000}L^3 - \frac{63}{250}L^2 + \frac{21}{2}L)}\times\;100\%$

    `护甲` 与 `魔法抗性` 将优先计算穿透数值，而后计算减伤。

-----

- **穿透** *(ArmorPenetration & MagicPenetration)*

    基于护甲 `A` 和 护甲穿透 `AP` `AP%` 计算得出更新的护甲 `A` 数值，计算公式为

    $AP_a=[A_b\times\;(1-\dfrac{AP\%_a}{100})-AP]\times\;100\%$

    同理，魔法减伤计算公式为<br>
    基于魔法抗性 `MaD` 和 魔法穿透 `MaP` `MaP%` 计算得出更新的魔法抗性 `MaD` 数值，计算公式为

    $MaP_a=[MaD_b\times\;(1-\dfrac{MaD\%_a}{100})-MaD]\times\;100\%$


-----

- **命中率 & 闪避率** *(HitChance & DodgeChance)*

    基于命中 `H` 和 闪避 `D` 计算得出的百分比数值，闪避率计算公式为

    $DC_a=\dfrac{D_a}{\frac{3}{2}D_a+800+H_b}\times\;100\%$

    同理，命中率公式为 

    $HC_a=(1-\dfrac{D_b}{\frac{3}{2}D_b+800+H_a})\times\;100\%$

    同时，由显而易见的$\frac{3}{2}D_{a/b}$可得 $DC_{max}=\frac{2}{3}=66.67\%$

    同理可得，$HC_{min}=\frac{1}{3}=33.33\%$

-----

- **暴击率 & 抗暴击率** *(CritChance & AC)*

    基于会心 `K` 和 柔韧 `F` 计算得出的百分比数值，暴击率计算公式为

    $C_a=\dfrac{3K_a}{4(K_a+800+F_b)}\times\;100\%$

    同理，抗暴击率公式为 

    $AC_a=(1-\dfrac{3K_b}{4(K_b+800+F_a)})\times\;100\%$

    同时，由显而易见的$\frac{3}{4}·\frac{K_b}{(K_b+800+F_a)}$可得 $C_{max}=75.00\%$

- **暴击 & 暴击伤害** *(CritAttack & CritDamage)*

    基于暴击几率 `C` 随机判定本次攻击是否为暴击，若判定为真，则进行计算额外攻击伤害，计算公式为

    $D_a^1=D_a\times\;(1+CrD\%)$


-----

- **生命偷取** *(HealthSteal)*

    基于生命偷取值 `HS` 判定本次攻击嗜血血量 `HSH`，计算公式为

    $HSH_a=D_a\times\;HS\%$


---

## Formulas (English)

?> The cubic polynomial approximates an exponential scaling by level, a design choice inherited from early technical constraints. <br>
This implementation has resulted in entrenched path dependencies, making modification infeasible.

**Damage**

- **Melee Damage**: 

    The damage dealt by a bare-handed attack or an item upon suCessfully hitting a target. The damage range is denoted by $\small {D_{\min} \thicksim D_{\max}}$. The final damage is calculated as:

    $D_a^1 = D_a \cdot (1 - R_b\%)$

- **Arrow Damage**: 

    The damage dealt by an arrow upon suCessfully hitting a target. The damage range is denoted by $\small {AD_{\min} \thicksim AD_{\max}}$. The final damage is calculated as:

    $AD_a^1 = \dfrac{AD_a \cdot (1 - R_b\%)}{3}$

- **Magic Damage**: 

    The damage dealt by a wand upon suCessfully hitting a target. The damage range is denoted by $\small {MD_{\min} \thicksim MD_{\max}}$. The final damage is calculated as:

    $MD_a^1 = MD_a \cdot (1 - MaR_b\%)$

Melee Damage and Arrow Damage are subject to Hit Chance, Critical Strike Chance, and Armor Penetration.<br>
All types of damage are subject to Attribute Enhancement and Life Steal.<br>
Magic Damage is subject to Magic Penetration.<br>
In the following, the symbol $\small D$ (without specification) generally refers to any of the three damage types.

---

**Elements**


There are four independent elements: `Light`, `Dark`, `Fire`, and `Ice`. <br>
During an attack, only the elemental damage bonus of the equipped weapon is calculated. The bonus formula is:

$D_{a}^1 = D_a \times \dfrac{1 + (EI_a - ED_b)}{1000}$

where $EI_a$ is the attacker's Elemental Intensity and $ED_b$ is the defender's Elemental Defense.

---

**Damage Reduction**

The percentage of damage reduction due to Armor ($A$) and Level ($L$) is calculated as:

$R_a = \dfrac{A_a}{ A_a + 420 + 8.4 \cdot \left( \frac{9}{1000}L^3 - \frac{63}{250}L^2 + \frac{21}{2}L \right)} \times 100\%$

Similarly, the percentage of magic damage reduction due to Magic Resistance ($MaD$) and Level ($L$) is calculated as:

$MaR_a = \dfrac{MaD_a}{ MaD_a + 420 + 8.4 \cdot \left( \frac{9}{1000}L^3 - \frac{63}{250}L^2 + \frac{21}{2}L \right)} \times 100\%$

The calculation of Armor and Magic Resistance takes into aCount penetration values before reduction.

---

**Penetration**

The effective Armor after penetration is calculated based on the target's Armor ($A_b$), the attacker's Armor Penetration percentage ($AP\%_a$), and fixed Armor Penetration ($AP_a$). The formula is:

$A_{\text{effective}} = A_b \cdot \left(1 - \dfrac{AP\%_a}{100}\right) - AP_a$

Similarly, the effective Magic Resistance after penetration is calculated based on the target's Magic Resistance ($MaD_b$), the attacker's Magic Penetration percentage ($MaP\%_a$), and fixed Magic Penetration ($MaP_a$). The formula is:

$MaD_{\text{effective}} = MaD_b \cdot \left(1 - \dfrac{MaP\%_a}{100}\right) - MaP_a$

Note: The updated effective values are then used in the damage reduction formulas.

---

**Hit Chance and Dodge Chance**

The Dodge Chance ($DC_a$) of an entity $a$ is calculated based on its Dodge ($D_a$) and the attacker's Hit ($H_b$):

$DC_a = \dfrac{D_a}{\frac{3}{2}D_a + 800 + H_b} \times 100\%$

Similarly, the Hit Chance ($HC_a$) of an attacker $a$ against a defender $b$ is:

$HC_a = \left(1 - \dfrac{D_b}{\frac{3}{2}D_b + 800 + H_a}\right) \times 100\%$

It is evident that the maximum Dodge Chance is $DC_{\max} = \frac{2}{3} \approx 66.67\%$, and the minimum Hit Chance is $HC_{\min} = \frac{1}{3} \approx 33.33\%$.

---

**Critical Strike Chance and Critical Resistance**

The Critical Strike Chance ($C_a$) of an attacker $a$ against a defender $b$ is calculated based on the attacker's Critical Strike Value ($K_a$) and the defender's Flexibility ($F_b$):

$C_a = \dfrac{3K_a}{4(K_a + 800 + F_b)} \times 100\%$

The Critical Resistance ($CR_a$) of an entity $a$ is:

$CR_a = \left(1 - \dfrac{3K_b}{4(K_b + 800 + F_a)}\right) \times 100\%$

Clearly, the maximum Critical Strike Chance is $C_{\max} = 75.00\%$.

**Critical Strike and Critical Damage**

If a Critical Strike is triggered (determined by $C_a$), the damage is amplified by the Critical Damage multiplier ($CrD\%$). The formula for the amplified damage is:

$D_a^1 = D_a \cdot (1 + CrD\%)$

---

**Life Steal**

The amount of health restored through Life Steal is calculated based on the Life Steal percentage ($HS\%$) and the damage dealt ($D_a$). The formula is:

$HSH_a = D_a \cdot HS\%$

where $HSH_a$ is the health stolen by attacker $a$.

