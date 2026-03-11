<style>

.markdown-section tr:nth-child(2n) {
    background-color: #fff;
}
.markdown-section td {
    padding: 3px 6px;
}

.dptag {
  color: #f0f0f0;
  background-color: #538aec;
  text-shadow: 0.5px 1px 0.5px rgba(0, 0, 0, 0.25);
  padding: 3px 4px;
  margin: 0 2px;
  border-radius: 3px;
  font-family: 等线;
  font-weight: 500;
}


.table-container {
  overflow-x: auto;
  -webkit-overflow-scrolling: touch;
}

.tag-gold {
  background: #eeaa10;
  color: #efffef;
}

.tag-yellow {
  background: #efbe40;
  color: #efffef;
}

.tag-green {
  background: #279027;
}

.tag-red {
  background: #ef8080;
  color: #ffffff;
}

.tag-red-blue {
  background: linear-gradient(135deg,#ef8080,#538aec);
  color: #f8ffef;
}

.tag-pink-gold {
  background: linear-gradient(135deg,#ff9b1a, #ff80f0);
  color: #f8ffef;
}

.tag-purple {
  background: #7a31aa;
}

.tag-gray {
  background: #989899;
}

.tag-cyan {
  background: #9999cc;
}

.tag-cyan {
  color: #f0f0f0;
  background: #9999cc;
  text-shadow: 0.5px 1px 0.5px rgba(0, 0, 0, 0.25);
  padding: 3px 4px;
  margin: 0 2px;
  border-radius: 5px;
  font-weight: 500;
}

ul {
    margin-block: 0em;
}

</style>
# 补给箱

## 简介

补给箱是一类消耗性道具，使用后可以立即获得一定资源。<br>
通常情况下分为 2 类： `装备型补给箱` `抽奖型补给箱`

---

## 装备型补给箱

封装有装备的补给箱<br>
使用后立即依照类型(随机)获得指定装备，如：
- **逐梦者补给箱 Tier 1**：获得 1 件 `传奇` 或 `神话` 的 「逐梦者装备」随机部位(头盔/护甲/护腿/靴子)
- **天之子补给箱 Tier 1**：获得 1 件 `传奇 [传承级]` 的 「天之子(Uranus)装备」随机部位(头盔/护甲/护腿/靴子)
- **弥赛亚补给箱 Tier 1**：获得 1 件 `传奇` 的 「弥赛亚(Messiah)装备」随机部位(头盔/护甲/护腿/靴子)

通常情况下，装备等级为玩家开启时的自身等级。<br>
你可以通过多种渠道获得「装备型补给箱」，包括但不限于：TokenStore、BattlePass、赞助满赠、抽奖型补给箱等。

---

## 抽奖型补给箱

封装有多种材料的补给箱，奖池中含有高价值奖品，每次开启均有概率获得。

<p style="font-size: 1em; text-shadow: 0 0 1px rgba(0,0,0,0.25); padding: 2px 10px; margin: 20px 0; border-left: 5px solid rgb(60, 110, 197); color: rgb(48, 93, 170); background: #f9fbfc;">保底机制</p>

当开启时将累加累计次数，当累加次数达到一定次数时，将触发保底，高概率获得高价值奖品。

累计次数参考下方详细表格，其中 `xx/yy` 意为：
- 每 `xx` 次触发一次**小保底**；
- 每 `yy` 次触发一次**大保底**。

<p style="border-left: 4px solid #aaa; color: #999; padding-left: 10px;">通常情况下开启次数需要 +1，即 10/60 在 #11/#61 触发。</p>

<p style="font-size: 1em; text-shadow: 0 0 1px rgba(0,0,0,0.25); padding: 2px 10px; margin: 20px 0; border-left: 5px solid rgb(60, 110, 197); color: rgb(48, 93, 170); background: #f9fbfc;">碎片机制</p>

可以通过碎片合成大奖，碎片可自由交易，每满足一次小保底将额外获得一枚碎片。<br>
可以通过分解大奖获得碎片，如大奖为装备，则需满足**装备等级**不小于 `当前等级 * 95%`，即：当前为 100 级，可拆解的装备等级至少为 95 级。

<p style="font-size: 1em; text-shadow: 0 0 1px rgba(0,0,0,0.25); padding: 2px 10px; margin: 20px 0; border-left: 5px solid rgb(60, 110, 197); color: rgb(48, 93, 170); background: #f9fbfc;">如何购买</p>

在游戏内输入 `/supplybox` 可查看所有可用补给箱，并查询当前累计次数或尝试购买。<br>
补给箱的基准定价为 `5 Kc`/个，你可以通过 [月卡](pages/月卡) 获得更优惠价格。亦可在购买时通过补给箱兑换券直接抵消购置补给箱。<br>
在所有购买请求尝试前，你都有机会进行二次检查。

<p style="font-size: 1em; text-shadow: 0 0 1px rgba(0,0,0,0.25); padding: 2px 10px; margin: 20px 0; border-left: 5px solid rgb(60, 110, 197); color: rgb(48, 93, 170); background: #f9fbfc;">补给箱详情</p>

<div class="table-container">
<table style="max-width: 700pt; text-align: center; font-family: 等线; border-image: initial; vertical-align: middle; white-space: nowrap;" cellspacing="0" cellpadding="0"><colgroup><col style="width: 100pt;" /> <col style="width: 80pt;" /> <col style="width: 160pt;" /> <col style="width: 80pt;" span="2" /> <col style="width: 200pt;" /></colgroup>
<tbody>
<tr style="height: 30pt; font-family: normal; font-size: 14pt; font-weight: 600;">
<td style="width: 100pt;">补给箱类型</td>
<td style="width: 80pt;">保底计划</td>
<td style="width: 160pt;">大奖</td>
<td style="width: 80pt;">合成碎片</td>
<td style="width: 80pt;">分解碎片</td>
<td style="width: 200pt;">备注</td>
</tr>
<tr style="height: 22.5pt;">
<td style="font-family: normal; font-size: 13pt; font-weight: 500;">祈愿</td>
<td>10/60</td>
<td>Adrasteia</td>
<td>48</td>
<td>24</td>
<td>已不可用；碎片名为神性碎片</td>
</tr>
<tr style="height: 10.00pt;">
<td colspan="6"></td>
</tr>
<tr style="height: 22.5pt;">
<td style="font-family: normal; font-size: 13pt; font-weight: 500;" rowspan="2">神权</td>
<td rowspan="2">10/60</td>
<td>权杖 Release</td>
<td>48</td>
<td>24</td>
<td style="font-family: normal;">高强度光属性法杖</td>
</tr>
<tr style="height: 22.5pt;">
<td>荣耀桂冠</td>
<td>48</td>
<td>24</td>
<td style="font-family: normal;">高强度光属性头盔</td>
</tr>
<tr style="height: 10.00pt;">
<td colspan="6"></td>
</tr>
<tr style="height: 22.5pt;">
<td style="font-family: normal; font-size: 13pt; font-weight: 500;" rowspan="3">混沌</td>
<td rowspan="3">20/120</td>
<td>theLia F&aacute;il</td>
<td>48</td>
<td>/</td>
<td style="font-family: normal;">命运之石，俗称 FS，提供多种加成</td>
</tr>
<tr style="height: 22.5pt;">
<td>潜影盒[P] unLimited</td>
<td>48</td>
<td>12</td>
<td style="font-family: normal;">不绑定紫色潜影盒</td>
</tr>
<tr style="height: 22.5pt;">
<td>潜影盒[P]</td>
<td>24</td>
<td>6</td>
<td style="font-family: normal;">绑定紫色潜影盒</td>
</tr>
<tr style="height: 10.00pt;">
<td colspan="6"></td>
</tr>
<tr style="height: 22.5pt;">
<td style="font-family: normal; font-size: 13pt; font-weight: 500;">悲剧</td>
<td>10/60</td>
<td>Hamlet</td>
<td>48</td>
<td>24</td>
<td style="font-family: normal;">高穿透近战镰刀</td>
</tr>
<tr style="height: 10.00pt;">
<td colspan="6"></td>
</tr>
<tr style="height: 22.5pt;">
<td style="font-family: normal; font-size: 13pt; font-weight: 500;">乱序</td>
<td>10/60</td>
<td>终境彼岸</td>
<td>48</td>
<td>24</td>
<td style="font-family: normal;">高属强暗属性长剑</td>
</tr>
<tr style="height: 10.00pt;">
<td colspan="6"></td>
</tr>
<tr style="height: 22.5pt;">
<td style="font-family: normal; font-size: 13pt; font-weight: 500;" rowspan="3">空间</td>
<td rowspan="3">10/60</td>
<td>界域引继者</td>
<td>48</td>
<td>24</td>
<td style="font-family: normal;">传送技能近战武器</td>
</tr>
<tr style="height: 22.5pt;">
<td>潜影盒[B] unLimited</td>
<td>96</td>
<td>32</td>
<td style="font-family: normal;">不绑定蓝色潜影盒</td>
</tr>
<tr style="height: 22.5pt;">
<td>潜影盒[B]</td>
<td>32</td>
<td>16</td>
<td style="font-family: normal;">绑定蓝色潜影盒</td>
</tr>
<tr style="height: 10.00pt;">
<td colspan="6"></td>
</tr>
<tr style="height: 40.00pt;">
<td style="font-family: normal; font-size: 13pt; font-weight: 500;" rowspan="2">潜影</td>
<td rowspan="2">10/60</td>
<td style="width: 147.75pt;">潜影盒[O/W/Y/G/PK/R]<br />unLimited</td>
<td>96</td>
<td>48</td>
<td style="font-family: normal;">不绑定「橙/白/黄/绿/粉/红」潜影盒</td>
</tr>
<tr style="height: 22.5pt;">
<td style="width: 147.75pt;">潜影盒[O/W/Y/G/PK/R]</td>
<td>48</td>
<td>24</td>
<td style="font-family: normal;">绑定「橙/白/黄/绿/粉/红」潜影盒</td>
</tr>
<tr style="height: 10.00pt;">
<td colspan="6"></td>
</tr>
<tr style="height: 22.5pt;">
<td style="font-family: normal; font-size: 13pt; font-weight: 500;" rowspan="2">腐败</td>
<td rowspan="2">20/120</td>
<td>权杖 Corruption</td>
<td>48</td>
<td>24</td>
<td style="font-family: normal;">超高强度暗属性法杖</td>
</tr>
<tr style="height: 22.5pt;">
<td>深渊王冠 Chaos</td>
<td>48</td>
<td>24</td>
<td style="font-family: normal;">超高强度暗属性吸血头盔</td>
</tr>
<tr style="height: 10.00pt;">
<td colspan="6"></td>
</tr>
<tr style="height: 22.5pt;">
<td style="font-family: normal; font-size: 13pt; font-weight: 500;" rowspan="4">通用</td>
<td rowspan="4">/</td>
<td>Hephaestus</td>
<td colspan="2" rowspan="4">/</td>
<td style="font-family: normal;">工匠武器</td>
</tr>
<tr style="height: 22.5pt;">
<td>12x 本类型碎片</td>
<td style="font-family: normal;">祈愿对应「神性」</td>
</tr>
<tr style="height: 22.5pt;">
<td>弥赛亚补给箱 Tier 1/2</td>
<td>&nbsp;</td>
</tr>
<tr style="height: 22.5pt;">
<td>天之子补给箱 Tier 1/2</td>
<td>&nbsp;</td>
</tr>
</tbody>
</table>
</div>
### 补给箱装备技能详情

部分补给箱装备提供了升级可能，通过拆解重复的装备或对等碎片可以用以消耗升级技能强度。


<p style="font-size: 1em; text-shadow: 0 0 1px rgba(0,0,0,0.25); padding: 2px 10px; margin: 20px 0; border-left: 5px solid rgb(60, 110, 197); color: rgb(48, 93, 170); background: #f9fbfc;">界域引继者：横跨空间的界限</p>

<span class="dptag">可升级</span><span class="dptag tag-green">位移</span><span class="dptag tag-purple">群攻</span>

消耗 `ManaCost` 点法力，并给自身增加 `ElementIncrease` 暗属性强化（基准属性单位）、`40` 单位命中。<br>
向前方最多 `Distance` 距离发起一次传送，对沿途的所有敌对生物及最终落点 `8x6x8` 范围内的所有生物造成一次暗属性魔法伤害。<br>
如落点为空气且 `TurboMode` 未达到 `3` 级，落点将下落至离地面最多 `4` 格高度。

<div class="table-container">
<table style="border-collapse: collapse; max-width: 679.52pt; font-size: 12pt; font-family: YuGothicUI; text-align: center; vertical-align: middle; white-space: nowrap; padding: 16px 16px 24px; border-radius: 24px; border: 1px solid #ccc;" cellspacing="0" cellpadding="0"><colgroup><col style="width: 45.75pt;" /> <col style="width: 14.25pt;" /> <col style="width: 56.25pt;" span="2" /> <col style="width: 10pt;" /> <col style="width: 56.25pt;" span="2" /> <col style="width: 10pt;" /> <col style="width: 56.25pt;" span="2" /> <col style="width: 10pt;" /> <col style="width: 56.25pt;" span="2" /> <col style="width: 10pt;" /> <col style="width: 56.25pt;" span="2" /></colgroup>
<tbody>
<tr style="height: 24.00pt; border-top: none;">
<td style="width: 45.75pt; color: #172436; font-weight: 500; border: none;">Tier</td>
<td style="width: 10pt; border: none;" rowspan="11"></td>
<td style="width: 112.5pt; color: #172436; font-weight: 500; border: none;" colspan="2">CD</td>
<td style="width: 10pt; border: none;" rowspan="11"></td>
<td style="width: 112.5pt; color: #172436; font-weight: 500; border: none;" colspan="2">Distance</td>
<td style="width: 10pt; border: none;" rowspan="11"></td>
<td style="width: 112.5pt; color: #172436; font-weight: 500; border: none;" colspan="2">ManaCost</td>
<td style="width: 10pt; border: none;" rowspan="11"></td>
<td style="width: 112.5pt; color: #172436; font-weight: 500; border: none;" colspan="2">ElementIncrease</td>
<td style="width: 10pt; border: none;" rowspan="11"></td>
<td style="width: 112.5pt; color: #172436; font-weight: 500; border: none;" colspan="2">TurboMode</td>
</tr>
<tr style="height: 24.00pt;">
<td style="font-size: 12pt; border-bottom: 0.5pt solid #808080; font-family: 微软雅黑; ">0</td>
<td style="color: #808080; border-top: none; border-bottom: 0.5pt solid #808080;">60</td>
<td style="color: #172436; border-top: none; border-bottom: 0.5pt solid #808080;">Cost</td>
<td style="color: #808080; border-top: none; border-bottom: 0.5pt solid #808080;">25</td>
<td style="color: #172436; border-top: none; border-bottom: 0.5pt solid #808080;">Cost</td>
<td style="color: #808080; border-top: none; border-bottom: 0.5pt solid #808080;">40</td>
<td style="color: #172436; border-top: none; border-bottom: 0.5pt solid #808080;">Cost</td>
<td style="color: #808080; border-top: none; border-bottom: 0.5pt solid #808080;">16</td>
<td style="color: #172436; border-top: none; border-bottom: 0.5pt solid #808080;">Cost</td>
<td style="color: #808080; border-top: none; border-bottom: 0.5pt solid #808080;">无</td>
<td style="color: #172436; border-top: none; border-bottom: 0.5pt solid #808080;">Cost</td>
</tr>
<tr style="height: 24.00pt;">
<td>1</td>
<td>40</td>
<td>1</td>
<td>30</td>
<td>1</td>
<td>36</td>
<td>1</td>
<td>20</td>
<td>2</td>
<td>1</td>
<td>4</td>
</tr>
<tr style="height: 24.00pt;">
<td>2</td>
<td>30</td>
<td>1</td>
<td>35</td>
<td>4</td>
<td>32</td>
<td>2</td>
<td>24</td>
<td>4</td>
<td>2</td>
<td>16</td>
</tr>
<tr style="height: 24.00pt;">
<td>3</td>
<td>24</td>
<td>2</td>
<td>40</td>
<td>8</td>
<td>28</td>
<td>4</td>
<td>32</td>
<td>8</td>
<td>3</td>
<td>32</td>
</tr>
<tr style="height: 24.00pt;">
<td>4</td>
<td>18</td>
<td>2</td>
<td style="vertical-align: bottom; color: #aaa; white-space: wrap; font-size: 14px;" colspan="2" rowspan="6"><span style="color: #172436">提升</span><br>传送的最远距离</td>
<td>24</td>
<td>8</td>
<td style="vertical-align: bottom; color: #aaa; white-space: wrap; font-size: 14px;" colspan="2" rowspan="6"><span style="color: #172436">提升</span><br>释放技能时增加的<br>暗属性强化单位</td>
<td style="vertical-align: bottom; color: #aaa;" colspan="2" rowspan="6"><span style="color: #172436;">狂暴模式</span><br>
<div style="display: flex; justify-content: space-evenly; align-items: center; padding: 8px 0;">
    <div style="vertical-align: middle;"><span class="tag-cyan">1</span> </div>
    <div style="vertical-align: middle; text-align: left; font-size: 13.33px;">法耗提升至 2x<br>冷却降低至 1/2</div>
</div>
<div style="display: flex; justify-content: space-evenly; align-items: center;">
    <div style="vertical-align: middle;"><span class="tag-cyan">2</span> </div>
    <div style="vertical-align: middle; text-align: left; font-size: 13.33px;">法耗提升至 4x<br>冷却降低至 1/3</div>
</div>
<div style="display: flex; justify-content: space-evenly; align-items: center; padding: 8px 0;">
    <div style="vertical-align: middle;"><span class="tag-cyan">3</span> </div>
    <div style="vertical-align: middle; text-align: left; font-size: 13.33px;">允许落点为空气</div>
</div>
</td>
</tr>
<tr style="height: 24.00pt;">
<td>5</td>
<td>12</td>
<td>4</td>
<td style="vertical-align: bottom; color: #aaa; white-space: wrap; font-size: 14px;" colspan="2" rowspan="5"><span style="color: #172436">降低</span><br>释放技能的法力消耗</td>
</tr>
<tr style="height: 24.00pt;">
<td>6</td>
<td>9</td>
<td>4</td>
</tr>
<tr style="height: 24.00pt;">
<td>7</td>
<td>6</td>
<td>8</td>
</tr>
<tr style="height: 24.00pt;">
<td>8</td>
<td>3</td>
<td>16</td>
</tr>
<tr style="height: 36.00pt;">
<td>/</td>
<td style="vertical-align: bottom; color: #aaa; white-space: wrap; font-size: 14px;" colspan="2"><span style="color: #172436">降低</span><br>技能冷却</td>
</tr>
</tbody>
</table>
</div>

<h5 id="终境彼岸" style="font-size: 1em; text-shadow: 0 0 1px rgba(0,0,0,0.25); padding: 2px 10px; margin: 20px 0; border-left: 5px solid rgb(60, 110, 197); color: rgb(48, 93, 170); background: #f9fbfc; font-weight: 400;">终境彼岸： 于时间的间隙向过往回望</h5>

<span class="dptag tag-purple">群攻</span>

消耗 `ManaCost` 点法力，基于自身个人暗属性强化获得 `Value` 点暗属性强化（基准属性单位，灰字为 Lv.360 属性）。<br>
随后，以前方 `3` 格为中心，在 `Area` 范围内击出 `6` 道斩击。<br>
每道斩击可对 `1` 名敌方目标造成 `1` 次近战伤害（最多 `6` 次伤害）。如当次攻击的目标未死亡，则下一次斩击将**无视目标攻击免疫**继续攻击同一目标。<br>
基准冷却时间为 `CD` 秒。每次成功攻击时，若目标死亡，则冷却时间减少 `CDR` 秒；若目标存活，则技能冷却时间减少 `1.5 x CDR` 秒。<br>
技能结束后，接下来的 `10` 秒内将扣除双倍增益的暗属性强化。

<div class="table-container">
<table style="font-size: 12pt; max-width: 700px; font-family: YuGothicUI; text-align: center; vertical-align: middle; white-space: nowrap; padding: 8px 16px 24px; border-radius: 24px; border: 1px solid #ccc;">
<tr style="height: 24.00pt; border-top: none; font-family: 微软雅黑;">
<td style="width: 120pt; color: #172436; font-weight: 500; border: none;" colspan="2" >Buff</td>
<td style="width: 10pt; border: none;" rowspan="10"></td>
<td style="width: 120pt; color: #172436; font-weight: 500; border: none;">CD</td>
<td style="width: 10pt; border: none;" rowspan="10"></td>
<td style="width: 120pt; color: #172436; font-weight: 500; border: none;">ManaCost</td>
<td style="width: 10pt; border: none;" rowspan="10"></td>
<td style="width: 120pt; color: #172436; font-weight: 500; border: none;">Area</td>
<td style="width: 10pt; border: none;" rowspan="10"></td>
<td style="width: 120pt; color: #172436; font-weight: 500; border: none;">CDR</td>
</tr>
<tr style="height: 28.00pt;">
<td style="width: 180pt; color: #484c52; font-family: 微软雅黑;">个人暗属强</td>
<td style="width: 180pt; color: #484c52; font-family: 微软雅黑;">Value</td>
<td style="font-size: 1.25em" rowspan="6">48</td>
<td style="font-size: 1.25em" rowspan="6">80</td>
<td style="font-size: 1.25em" rowspan="6">9x4x9</td>
<td style="font-size: 1.25em" rowspan="6">3</td>
</tr>
<tr style="height: 24.00pt; padding: 8px;">
<td>&lt;3 <span style="color: #999; font-size: 12px;">(7172)</span></td>
<td>6 <span style="color: #999; font-size: 12px;">(14344)</span></td>
</tr>
<tr style="height: 24.00pt; padding: 8px;">
<td>≥ 3 <span style="color: #999; font-size: 12px;">(7172)</span></td>
<td>15 <span style="color: #999; font-size: 12px;">(35860)</span></td>
</tr>
<tr style="height: 24.00pt; padding: 8px;">
<td>≥ 6 <span style="color: #999; font-size: 12px;">(14344)</span></td>
<td>22.5 <span style="color: #999; font-size: 12px;">(53790)</span></td>
</tr>
<tr style="height: 24.00pt; padding: 8px;">
<td>≥ 15 <span style="color: #999; font-size: 12px;">(35860)</span></td>
<td>30 <span style="color: #999; font-size: 12px;">(71720)</span></td>
</tr>
<tr style="height: 24.00pt; padding: 8px;">
<td>≥ 22.5 <span style="color: #999; font-size: 12px;">(53790)</span></td>
<td>40 <span style="color: #999; font-size: 12px;">(95627)</span></td>
</tr>

</table>
</div>

<h5 id="战争践踏" style="font-size: 1em; text-shadow: 0 0 1px rgba(0,0,0,0.25); padding: 2px 10px; margin: 20px 0; border-left: 5px solid rgb(60, 110, 197); color: rgb(48, 93, 170); background: #f9fbfc; font-weight: 400;">战争践踏</h5>

<span class="dptag tag-green">位移</span><span class="dptag tag-purple">群攻</span><span class="dptag tag-pink-gold">增益</span>

消耗 `ManaCost` 点法力。<br>
随后，向前方跃出，`0.5`s 后落地，并对 `Area` 范围内最多 `6` 个敌对目标造成一次近战伤害并击飞。<br>
每成功造成 `1` 次攻击，都将为自身提供 `3%` 近战攻击加成，持续 `Duration`s 。<br>
基准冷却时间为 `CD` 秒。<br>

<div class="table-container">
<table style="font-size: 12pt; width: 100%; max-width: 540px; font-family: YuGothicUI; text-align: center; vertical-align: middle; white-space: nowrap; padding: 8px 16px 24px; border-radius: 24px; border: 1px solid #ccc;">
<tr style="height: 24.00pt; border-top: none; font-family: 微软雅黑;">
<td style="width: 90pt; color: #172436; font-weight: 500; border: none;">CD</td>
<td style="width: 10pt; border: none;" rowspan="10"></td>
<td style="width: 90pt; color: #172436; font-weight: 500; border: none;">ManaCost</td>
<td style="width: 10pt; border: none;" rowspan="10"></td>
<td style="width: 90pt; color: #172436; font-weight: 500; border: none;">Area</td>
<td style="width: 10pt; border: none;" rowspan="10"></td>
<td style="width: 90pt; color: #172436; font-weight: 500; border: none;">Duration</td>
</tr>
<tr style="height: 90.00pt;">
<td style="font-size: 1.25em" rowspan="6">27</td>
<td style="font-size: 1.25em" rowspan="6">60</td>
<td style="font-size: 1.25em" rowspan="6">7x3x7</td>
<td style="font-size: 1.25em" rowspan="6">12</td>
</tr>
</div>