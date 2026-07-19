<style>

.markdown-section tr:nth-child(2n) {
    background-color: #fff;
}
.markdown-section td {
    padding: 5px 8px;
}

.table-container {
    overflow-x: auto;
    -webkit-overflow-scrolling: touch;
}

.rune-table {
    border-collapse: collapse;
    width: 100%;
    font-family: 等线, sans-serif;
    text-align: center;
    vertical-align: middle;
    white-space: nowrap;
    margin: 5px 0 20px;
    border: 1px solid #ccc;
}

.rune-table th {
    padding: 7px 8px;
    font-weight: 500;
}

.rune-table .price {
    font-family: Exo, sans-serif;
}

</style>

# 制式符文

## 简介

制式符文拥有固定的属性搭配，可通过 `Kc` 购买。 1 CNY = **100** Kc。

制式符文现分为 `核心符文` `附属符文`，两类符文均可独立购买、使用。

且**同类符文**只能购买一个。

当你为 `核心符文` 购置「附属槽位」时，可将已拥有的 `附属符文` 镶嵌于其上，节约符文位。「附属槽位」至多拥有 `3` 个。

!> Rapids 的「附属槽位」系统暂未开放，因此替代的是目前玩家符文槽位拥有 `6` 个。

## 符文明细

所附价格单位均为 `Kc`。百分比属性以 `%` 标注；固定属性直接显示数值。<br>
配置中通过公式乘以等级基准值的属性以 `unit` 表示，例如 `0.25 unit` 表示对应属性等级基准值的 `0.25` 倍，不代表固定面板数值。

<p id="核心符文" style="font-size: 1em; text-shadow: 0 0 1px rgba(0,0,0,0.25); padding: 2px 10px; margin: 20px 0; border-left: 5px solid rgb(60, 110, 197); color: rgb(48, 93, 170); background: #f9fbfc;">核心符文</p>

### 咒文的咏叹调

属性简析：

法球是一个持续向前移动覆盖的矩形棱柱范围，会对范围内的所有怪物造成伤害。

- `法球伤害半径` 决定法球的半径，即宽度。
- `法球飞行速度` 决定法球每秒步进的距离，也可以等价视作 1/2 **可穿透距离** 。
- `法球飞行距离` 决定法球可步进的最远距离。

> `柔韧` 词条新增于 2026/07/19 午间，如你的符文尚未更新至含柔韧的版本，请联系管理员更新。

<div class="table-container">
  <table style="border-collapse: collapse; overflow: hidden; width: fit-content; font-family: 等线; text-align: center; border-image: initial; vertical-align: middle; white-space: nowrap; margin: 5px; padding: 16px; border-radius: 24px; border: 1px solid #ccc;" class="rune-table">
    <thead><tr><th>等级</th><th>魔法攻击</th><th>法力恢复</th><th>施法速度</th><th>魔法穿透</th><th>柔韧</th><th>法力上限</th><th>法球伤害半径</th><th>法球飞行速度</th><th>法球飞行距离</th><th>价格 (Kc)</th></tr></thead>
    <tbody>
      <tr><td>I</td><td>+15%</td><td>+1</td><td>&nbsp;</td><td>&nbsp;</td><td>+0.5 unit</td><td>+40</td><td>+0.2</td><td>&nbsp;</td><td>&nbsp;</td><td class="price">7,500</td></tr>
      <tr><td>II</td><td>+30%</td><td>+2</td><td>&nbsp;</td><td>&nbsp;</td><td>+1 unit</td><td>+80</td><td>+0.3</td><td>+1</td><td>&nbsp;</td><td class="price">15,000</td></tr>
      <tr><td>III</td><td>+45%</td><td>+4</td><td>&nbsp;</td><td>&nbsp;</td><td>+1.5 unit</td><td>+80</td><td>+0.3</td><td>+2</td><td>+10</td><td class="price">30,000</td></tr>
      <tr><td>IV</td><td>+60%</td><td>+6</td><td>&nbsp;</td><td>&nbsp;</td><td>+2 unit</td><td>+120</td><td>+0.5</td><td>+3</td><td>+20</td><td class="price">60,000</td></tr>
      <tr><td>V</td><td>+100%</td><td>+6</td><td>&nbsp;</td><td>+10%</td><td>+2.5 unit</td><td>+120</td><td>+0.625</td><td>+4</td><td>+20</td><td class="price">100,000</td></tr>
      <tr><td>VI</td><td>+135%</td><td>+8</td><td>+0.2次/秒</td><td>+10%</td><td>+3 unit</td><td>+160</td><td>+0.75</td><td>+4</td><td>+25</td><td class="price">150,000</td></tr>
      <tr><td>VII</td><td>+175%</td><td>+8</td><td>+0.35次/秒</td><td>+20%</td><td>+4 unit</td><td>+160</td><td>+0.75</td><td>+5</td><td>+30</td><td class="price">225,000</td></tr>
      <tr><td>VIII</td><td>+225%</td><td>+8</td><td>+0.5次/秒</td><td>+20%</td><td>+5 unit</td><td>+160</td><td>+0.875</td><td>+6</td><td>+30</td><td class="price">325,000</td></tr>
    </tbody>
  </table>
</div>

### 不屈的凯旋颂

属性简析：

近战造成的是范围伤害，默认伤害半径 `1.5` 格，最大攻击数量 `3` 个。

即单次攻击最多对 3 格内最多 3 个怪物造成伤害。

- `近战攻击距离` 决定近战攻击范围半径。
- `近战攻击数量` 决定近战单次攻击可选取的怪物数量。

<div class="table-container">
  <table style="border-collapse: collapse; overflow: hidden; width: fit-content; font-family: 等线; text-align: center; border-image: initial; vertical-align: middle; white-space: nowrap; margin: 5px; padding: 16px; border-radius: 24px; border: 1px solid #ccc;" class="rune-table">
    <thead><tr><th>等级</th><th>近战攻击</th><th>攻击速度</th><th>近战攻击距离</th><th>近战攻击数量</th><th>最大生命</th><th>生命恢复</th><th>护甲穿透</th><th>价格 (Kc)</th></tr></thead>
    <tbody>
      <tr><td>I</td><td>+15%</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>+5%</td><td>+0.25 unit</td><td>+5%</td><td class="price">7,500</td></tr>
      <tr><td>II</td><td>+30%</td><td>&nbsp;</td><td>+20%</td><td>&nbsp;</td><td>+10%</td><td>+0.4 unit</td><td>+5%</td><td class="price">15,000</td></tr>
      <tr><td>III</td><td>+45%</td><td>&nbsp;</td><td>+25%</td><td>+1</td><td>+15%</td><td>+0.625 unit</td><td>+10%</td><td class="price">30,000</td></tr>
      <tr><td>IV</td><td>+60%</td><td>+0.25</td><td>+40%</td><td>+1</td><td>+20%</td><td>+0.875 unit</td><td>+15%</td><td class="price">60,000</td></tr>
      <tr><td>V</td><td>+100%</td><td>+0.375</td><td>+50%</td><td>+2</td><td>+25%</td><td>+1.375 unit</td><td>+20%</td><td class="price">100,000</td></tr>
      <tr><td>VI</td><td>+135%</td><td>+0.5</td><td>+60%</td><td>+2</td><td>+30%</td><td>+1.75 unit</td><td>+20%</td><td class="price">150,000</td></tr>
      <tr><td>VII</td><td>+175%</td><td>+0.5</td><td>+60%</td><td>+3</td><td>+30%</td><td>+2.25 unit</td><td>+25%</td><td class="price">225,000</td></tr>
      <tr><td>VIII</td><td>+225%</td><td>+0.625</td><td>+75%</td><td>+3</td><td>+35%</td><td>+2.75 unit</td><td>+25%</td><td class="price">325,000</td></tr>
    </tbody>
  </table>
</div>

### 穿云的鸣镝歌

属性简析：

箭矢射出后不会受重力影响下坠，且能直线贯穿最多 `2` 个怪物。

即单次攻击最多对射线路径上最多 3 个怪物造成伤害。

- `箭矢速度` 决定箭矢的飞行速度。与 `箭矢存活时间` 共同决定箭矢的飞行距离。
- `箭矢存活时间` 决定箭矢的最大飞行时间。与 `箭矢速度` 共同决定箭矢的飞行距离。
- `箭矢穿透` 决定箭矢的可穿透数量。

<div class="table-container">
  <table style="border-collapse: collapse; overflow: hidden; width: fit-content; font-family: 等线; text-align: center; border-image: initial; vertical-align: middle; white-space: nowrap; margin: 5px; padding: 16px; border-radius: 24px; border: 1px solid #ccc;" class="rune-table">
    <thead><tr><th>等级</th><th>箭矢攻击</th><th>箭矢速度</th><th>攻击速度</th><th>箭矢穿透</th><th>箭矢存活时间</th><th>会心</th><th>暴击伤害</th><th>护甲穿透</th><th>价格 (Kc)</th></tr></thead>
    <tbody>
      <tr><td>I</td><td>+15%</td><td>+15%</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>+2 unit</td><td>&nbsp;</td><td>+5%</td><td class="price">7,500</td></tr>
      <tr><td>II</td><td>+30%</td><td>+30%</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>+4 unit</td><td>&nbsp;</td><td>+5%</td><td class="price">15,000</td></tr>
      <tr><td>III</td><td>+45%</td><td>+45%</td><td>&nbsp;</td><td>&nbsp;</td><td>+5</td><td>+6 unit</td><td>+30%</td><td>+10%</td><td class="price">30,000</td></tr>
      <tr><td>IV</td><td>+60%</td><td>+50%</td><td>&nbsp;</td><td>+1</td><td>+5</td><td>+8 unit</td><td>+50%</td><td>+15%</td><td class="price">60,000</td></tr>
      <tr><td>V</td><td>+100%</td><td>+50%</td><td>&nbsp;</td><td>+2</td><td>+5</td><td>+12 unit</td><td>+75%</td><td>+20%</td><td class="price">100,000</td></tr>
      <tr><td>VI</td><td>+135%</td><td>+50%</td><td>&nbsp;</td><td>+2</td><td>+8</td><td>+16 unit</td><td>+100%</td><td>+20%</td><td class="price">150,000</td></tr>
      <tr><td>VII</td><td>+175%</td><td>+50%</td><td>+0.3</td><td>+3</td><td>+8</td><td>+20 unit</td><td>+125%</td><td>+25%</td><td class="price">225,000</td></tr>
      <tr><td>VIII</td><td>+225%</td><td>+60%</td><td>+0.6</td><td>+3</td><td>+10</td><td>+30 unit</td><td>+150%</td><td>+25%</td><td class="price">325,000</td></tr>
    </tbody>
  </table>
</div>


<p id="附属符文" style="font-size: 1em; text-shadow: 0 0 1px rgba(0,0,0,0.25); padding: 2px 10px; margin: 20px 0; border-left: 5px solid rgb(60, 110, 197); color: rgb(48, 93, 170); background: #f9fbfc;">附属符文</p>

### 逐风的轻快曲

<div class="table-container">
  <table style="border-collapse: collapse; overflow: hidden; width: fit-content; font-family: 等线; text-align: center; border-image: initial; vertical-align: middle; white-space: nowrap; margin: 5px; padding: 16px; border-radius: 24px; border: 1px solid #ccc;" class="rune-table">
    <thead><tr><th>等级</th><th>移动速度</th><th>价格 (Kc)</th></tr></thead>
    <tbody>
      <tr><td>I</td><td>+50%</td><td class="price">7,500</td></tr>
      <tr><td>II</td><td>+100%</td><td class="price">15,000</td></tr>
      <tr><td>III</td><td>+150%</td><td class="price">30,000</td></tr>
      <tr><td>IV</td><td>+200%</td><td class="price">60,000</td></tr>
    </tbody>
  </table>
</div>

### 坚城的镇魂歌

<div class="table-container">
  <table style="border-collapse: collapse; overflow: hidden; width: fit-content; font-family: 等线; text-align: center; border-image: initial; vertical-align: middle; white-space: nowrap; margin: 5px; padding: 16px; border-radius: 24px; border: 1px solid #ccc;" class="rune-table">
    <thead><tr><th>等级</th><th>护甲</th><th>魔法抗性</th><th>价格 (Kc)</th></tr></thead>
    <tbody>
      <tr><td>I</td><td>+1.25 unit</td><td>+1.25 unit</td><td class="price">5,000</td></tr>
      <tr><td>II</td><td>+2.5 unit</td><td>+2.5 unit</td><td class="price">10,000</td></tr>
      <tr><td>III</td><td>+3.75 unit</td><td>+3.75 unit</td><td class="price">20,000</td></tr>
      <tr><td>IV</td><td>+5 unit</td><td>+5 unit</td><td class="price">40,000</td></tr>
    </tbody>
  </table>
</div>

### 偶然的狂想曲

以 `自然馈赠/200` 的比例加成**怪物**掉落材料的几率。（不生效于宝箱或采集物）

> 参考: 50/200 → 25% → x1.25 | 如原 10% → 12.5%<br>
> 生效范围如：普通怪物的 绿色/蓝色材料 ；Elite / Essence 的蓝色材料；Final 的紫色材料

<div class="table-container">
  <table style="border-collapse: collapse; overflow: hidden; width: fit-content; font-family: 等线; text-align: center; border-image: initial; vertical-align: middle; white-space: nowrap; margin: 5px; padding: 16px; border-radius: 24px; border: 1px solid #ccc;" class="rune-table">
    <thead><tr><th>等级</th><th>自然馈赠</th><th>价格 (Kc)</th></tr></thead>
    <tbody>
      <tr><td>I</td><td>+50</td><td class="price">15,000</td></tr>
    </tbody>
  </table>
</div>
