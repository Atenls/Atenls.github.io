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
    min-width: 760px;
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

.rune-table .rune-name {
    min-width: 150px;
    font-size: 16px;
    font-weight: 600;
}

.rune-table .attributes {
    min-width: 430px;
    text-align: left;
    white-space: normal;
    line-height: 1.75;
}

.rune-table .price {
    font-family: Exo, sans-serif;
}

</style>

# 制式符文

## 简介

制式符文拥有固定的属性搭配，可通过 `Kc` 购买。下表属性与价格提取自当前 `regularrune.yml` 配置。

## 符文明细

所附价格单位均为 `Kc`。百分比属性以 `%` 标注；固定属性直接显示数值。<br>
配置中通过公式乘以等级基准值的属性以 `unit` 表示，例如 `0.25 unit` 表示对应属性等级基准值的 `0.25` 倍，不代表固定面板数值。

<p id="核心符文" style="font-size: 1em; text-shadow: 0 0 1px rgba(0,0,0,0.25); padding: 2px 10px; margin: 20px 0; border-left: 5px solid rgb(60, 110, 197); color: rgb(48, 93, 170); background: #f9fbfc;">核心符文</p>

<div class="table-container">
  <table class="rune-table">
    <thead>
      <tr>
        <th>Name</th>
        <th>Tier</th>
        <th>Attributes</th>
        <th>Price</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td class="rune-name" rowspan="5">咒文的咏叹调</td>
        <td>I</td>
        <td class="attributes">魔法攻击 +15% · 法力恢复 +1 · 法力上限 +40 · 法球伤害半径 +0.2</td>
        <td class="price">7,500</td>
      </tr>
      <tr>
        <td>II</td>
        <td class="attributes">魔法攻击 +30% · 法力恢复 +2 · 法力上限 +80 · 法球伤害半径 +0.3 · 法球飞行速度 +1</td>
        <td class="price">15,000</td>
      </tr>
      <tr>
        <td>III</td>
        <td class="attributes">魔法攻击 +45% · 法力恢复 +4 · 法力上限 +80 · 法球伤害半径 +0.3 · 法球飞行速度 +2 · 法球飞行距离 +10</td>
        <td class="price">30,000</td>
      </tr>
      <tr>
        <td>IV</td>
        <td class="attributes">魔法攻击 +60% · 法力恢复 +6 · 法力上限 +120 · 法球伤害半径 +0.5 · 法球飞行速度 +3 · 法球飞行距离 +20</td>
        <td class="price">60,000</td>
      </tr>
      <tr>
        <td>V</td>
        <td class="attributes">魔法攻击 +100% · 法力恢复 +6 · 魔法穿透 +10% · 法力上限 +120 · 法球伤害半径 +0.625 · 法球飞行速度 +4 · 法球飞行距离 +20</td>
        <td class="price">100,000</td>
      </tr>
      <tr>
        <td class="rune-name" rowspan="5">不屈的凯旋颂</td>
        <td>I</td>
        <td class="attributes">近战攻击 +15% · 最大生命 +5% · 生命恢复 +0.25 unit · 护甲穿透 +5%</td>
        <td class="price">7,500</td>
      </tr>
      <tr>
        <td>II</td>
        <td class="attributes">近战攻击 +30% · 近战攻击距离 +20% · 最大生命 +10% · 生命恢复 +0.4 unit · 护甲穿透 +5%</td>
        <td class="price">15,000</td>
      </tr>
      <tr>
        <td>III</td>
        <td class="attributes">近战攻击 +45% · 近战攻击距离 +25% · 近战攻击次数 +1 · 最大生命 +15% · 生命恢复 +0.625 unit · 护甲穿透 +10%</td>
        <td class="price">30,000</td>
      </tr>
      <tr>
        <td>IV</td>
        <td class="attributes">近战攻击 +60% · 攻击速度 +0.25 · 近战攻击距离 +40% · 近战攻击次数 +1 · 最大生命 +20% · 生命恢复 +0.875 unit · 护甲穿透 +15%</td>
        <td class="price">60,000</td>
      </tr>
      <tr>
        <td>V</td>
        <td class="attributes">近战攻击 +100% · 攻击速度 +0.375 · 近战攻击距离 +50% · 近战攻击次数 +2 · 最大生命 +25% · 生命恢复 +1.375 unit · 护甲穿透 +20%</td>
        <td class="price">100,000</td>
      </tr>
      <tr>
        <td class="rune-name" rowspan="5">穿云的鸣镝歌</td>
        <td>I</td>
        <td class="attributes">箭矢攻击 +15% · 箭矢速度 +15% · 会心 +2 unit · 护甲穿透 +5%</td>
        <td class="price">7,500</td>
      </tr>
      <tr>
        <td>II</td>
        <td class="attributes">箭矢攻击 +30% · 箭矢速度 +30% · 会心 +4 unit · 护甲穿透 +5%</td>
        <td class="price">15,000</td>
      </tr>
      <tr>
        <td>III</td>
        <td class="attributes">箭矢攻击 +45% · 箭矢速度 +45% · 箭矢飞行时间 +5 · 会心 +6 unit · 暴击伤害 +30% · 护甲穿透 +10%</td>
        <td class="price">30,000</td>
      </tr>
      <tr>
        <td>IV</td>
        <td class="attributes">箭矢攻击 +60% · 箭矢速度 +50% · 箭矢穿透 +1 · 箭矢飞行时间 +5 · 会心 +8 unit · 暴击伤害 +50% · 护甲穿透 +15%</td>
        <td class="price">60,000</td>
      </tr>
      <tr>
        <td>V</td>
        <td class="attributes">箭矢攻击 +100% · 箭矢速度 +50% · 箭矢穿透 +2 · 箭矢飞行时间 +5 · 会心 +12 unit · 暴击伤害 +75% · 护甲穿透 +20%</td>
        <td class="price">100,000</td>
      </tr>
      <tr>
        <td class="rune-name" rowspan="4">逐风的轻快曲</td>
        <td>I</td>
        <td class="attributes">移动速度 +50%</td>
        <td class="price">7,500</td>
      </tr>
      <tr>
        <td>II</td>
        <td class="attributes">移动速度 +100%</td>
        <td class="price">15,000</td>
      </tr>
      <tr>
        <td>III</td>
        <td class="attributes">移动速度 +150%</td>
        <td class="price">30,000</td>
      </tr>
      <tr>
        <td>IV</td>
        <td class="attributes">移动速度 +200%</td>
        <td class="price">60,000</td>
      </tr>
      <tr>
        <td class="rune-name">偶然的狂想曲</td>
        <td>V</td>
        <td class="attributes">自然幸运 +50</td>
        <td class="price">15,000</td>
      </tr>
    </tbody>
  </table>
</div>
