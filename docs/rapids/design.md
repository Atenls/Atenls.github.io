<style>
* {
  --force-text-fill-color: #6080b6;
  font-family: 'SFPro', 'PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', 'WenQuanYi Micro Hei', 'Helvetica Neue', 'Helvetica', 'Arial', 'sans-serif';
}

.attributes-content {
  color: rgb(222,222,224);
  background: rgb(29,29,30);
  padding: 2em;
  border-radius: 2em;
  border: 0 0 8px rgb(43,43,43);

  @media (max-width: 768px) { 
    margin: 4px;
  }
}

.markdown-section .attributes-content h2 {
  margin: 0;
}

.attributes-content .anchor span {
  color: rgb(245,245,247);
}

.markdown-section {
  max-width: 1200px;
  @media (max-width: 768px) {
    margin: 4px;
    padding: 12px 4px;
  }

}

.attrtag {
  border-left: 5px solid var(--bordercolor, --color, #333);
  padding: 0 10px;
  margin: 0 10px;
  text-shadow: 0 0 1px rgba(127,127,127, 0.25);
  color: var(--color, #333);
}

.content-container {
  border-radius: 1em;
  padding: 1em;
  background: rgb(22,7,22);
  color: rgb(222,222,224);
  text-align: left;
  border: 2px solid rgb(36, 0, 90);
  box-shadow: 0 0 8px rgba(36, 0, 90, 0.75);
}

.content-container p {
  margin: 1em 0;
  line-height: 1.375rem;
}

.element-container {
  background: rgb(22,7,22);
  border-radius: 12px;
  width: 300px;
  padding: 20px;
  text-align: left;
  box-shadow: 0 0 8px rgba(36, 0, 90, 0.75);
}

.element-container p {
  margin: 0.75rem 0;
  line-height: 1.6rem;
}

@media (max-width: 768px) {
  .markdown-section img:not([width]):not([style]) {
    width: 100%;
    max-width: 400px;
  }
}

</style>

# Rapids Design

你可于本栏获得 Rapids 之设计相关内容。

<div class="attributes-content">

## 配色

由于大部分颜色相关内容因颜色亮度会导致在白色背景下难以阅读，故将背景颜色设置为黑灰色以模拟游戏内情况。敬请谅解。

### 属性

<div style="display: flex; gap: 2em; flex-wrap: wrap;">
<div class="element-container" style="width: 275px;">
<p style="font-size: 18px; font-weight: 600; margin: 0; text-align: center;">基础属性</p>
<p><span class="attrtag" style="--color: #008000">❤ 最大生命 #008000</span></p>
<p><span class="attrtag" style="--color: #60f060">❤ 生命恢复 #60f060</span></p>
<p><span class="attrtag" style="--color: #b02020">🩸 生命偷取 #b02020</span></p>
<p><span class="attrtag" style="--color: #9f289f">⚔ 灵魂攻击 #9f289f</span></p>
<p><span class="attrtag" style="--color: #e8bf40">⚒ 全系伤害加成 #e8bf40</span></p>
<p><span class="attrtag" style="--color: #ffaa00">移动速度 #ffaa00</span></p>
<p><span class="attrtag" style="--color: #ffff00">自然馈赠 #ffff00</span></p>
<p><span class="attrtag" style="--color: #f040f0">经验加成 #f040f0</span></p>
<p><span class="attrtag" style="--color: #aaaaaa">描述内容 #aaaaaa</span></p>
<p><span class="attrtag" style="--color: #ffffff;">数值内容 #ffffff</span></p>
</div>

<div class="element-container" style="width: 275px;">
<p style="font-size: 18px; font-weight: 600; margin: 0; text-align: center;">物理属性</p>
<p><span class="attrtag" style="--color: #ff3030">⚔ 近战攻击 #ff3030</span></p>
<p><span class="attrtag" style="--color: #f08060">⚔ 箭矢攻击 #f08060</span></p>
<p><span class="attrtag" style="--color: #ffa060">➹ 攻击速度 #ffa060</span></p>
<p><span class="attrtag" style="--color: #5599dd">🔰 护甲 #5599dd</span></p>
<p><span class="attrtag" style="--color: #5599dd">护甲穿透 #5599dd</span></p>
<p><span class="attrtag" style="--color: #ffc170">暴击伤害 #ffff70</span></p>
<p><span class="attrtag" style="--color: #e0e080">会心 #e0e080</span></p>
<p><span class="attrtag" style="--color: #e0e080">柔韧 #e0e080</span></p>
<p><span class="attrtag" style="--color: #e0e080">命中 #e0e080</span></p>
<p><span class="attrtag" style="--color: #e0e080">闪避 #e0e080</span></p>
</div>

<div class="element-container" style="width: 275px;">
<p style="font-size: 18px; font-weight: 600; margin: 0; text-align: center;">魔法属性</p>
<p><span class="attrtag" style="--color: #60ffff">⚛️ 法力值 #60ffff</span></p>
<p><span class="attrtag" style="--color: #20ffb0">✨ 法力恢复 #20ffb0</span></p>
<p><span class="attrtag" style="--color: #40e8ff">⚔ 魔法攻击 #40e8ff</span></p>
<p><span class="attrtag" style="--color: #50b8f8">🔰 魔法抗性 #50b8f8</span></p>
<p><span class="attrtag" style="--color: #ffa060">➹ 施法速度 #a8714c</span></p>
<p><span class="attrtag" style="--color: #d0a060">⚶ 法力消耗 #d08d60</span></p>
<p><span class="attrtag" style="--color: #50b8f8">魔法穿透 #50b8f8</span></p>
<p><span class="attrtag" style="--color: #70e8f0">法球伤害半径 #70e8f0</span></p>
<p><span class="attrtag" style="--color: #70e8f0">法球飞行速度 #70e8f0</span></p>
<p><span class="attrtag" style="--color: #70e8f0">法球飞行距离 #70e8f0</span></p>
</div>
</div>

### 元素

<div class="element-container" style="width: 275px;">
<p><span class="attrtag" style="--color: #ffff00">🌟 光属性 #ffff00</span></p>
<p><span class="attrtag" style="--color: #A000A0">⚛ 暗属性 #a000a0</span></p>
<p><span class="attrtag" style="--color: #60ffff">❄ 冰属性 #60ffff</span></p>
<p><span class="attrtag" style="--color: #ff6060">❃ 火属性 #ff6060</span></p>
<p><span class="attrtag" style="--color: #008000">⛰ 地属性 #008000</span></p>
<p><span class="attrtag" style="--color: #8080ff">🌩 雷属性 #8080ff</span></p>
</div>

### 品质

<div class="element-container" style="width: 275px; padding-right: 0;">
<p><span class="attrtag" style="--bordercolor: #444444; --color: #808080">粗糙 #444444 | #808080</span></p>
<p><span class="attrtag" style="--bordercolor: #aaaaaa; --color: #dddddd">普通 #AAAAAA | #DDDDDD</span></p>
<p><span class="attrtag" style="--bordercolor: #40DF40; --color: #65CF65">优秀 #40DF40 | #65CF65</span></p>
<p><span class="attrtag" style="--bordercolor: #8090E0; --color: #80B0E0">卓越 #8090E0 | #80B0E0</span></p>
<p><span class="attrtag" style="--bordercolor: #EE77EE; --color: #CC80CC">史诗 #EE77EE | #CC80CC</span></p>
<p><span class="attrtag" style="--bordercolor: #FF6000; --color: #FFAA00">传奇 #FF8000 | #FFAA00</span></p>
<p><span class="attrtag" style="--bordercolor: #FF4040; --color: #FF8080">神话 #FF4040 | #FF8080</span></p>
</div>
</div>

## 排版

### 武器 & 装备 通用模板

<div style="display: flex; gap: 2em; flex-wrap: wrap;">
<div class="content-container" style="width: 400px;">
<p style="padding-left: 1em; margin: 0;">▌ <装备名称></p>
<p></p>
<p style="padding-left: 1em; margin: 0;">┌ <可用位置> | <装备类型> | <元素属性>(如有)</p>
<p style="padding-left: 1em; margin: 0;">└ <装备品质> | <等级需求></p>
<p></p>
<p style="padding-left: 1.5em; margin: 0;">⚔ 基准属性: <数值></p>
<p style="padding-left: 1.5em; margin: 0;">➹ 基准属性: <数值></p>
<p style="padding-left: 1.5em; margin: 0;">⚶ 基准属性: <数值></p>
<p></p>
<p style="padding-left: 1.5em; margin: 0;">┌ 额外属性: <数值>(如有)</p>
<p style="padding-left: 1.5em; margin: 0;">├ 额外属性: <数值>(如有)</p>
<p style="padding-left: 1.5em; margin: 0;">├ 额外属性: <数值>(如有)</p>
<p style="padding-left: 1.5em; margin: 0;">└ 额外属性: <数值>(如有)</p>
<p></p>
<p style="padding-left: 1.5em; margin: 0;">「 武器或装备描述 」</p>
<p></p>
<p style="padding-left: 1em; margin: 0;">💰 <数值> E</p>
<p></p>
</div>
<img class="content-container" style="padding: 0; overflow: hidden;" src="/rapids/rapids_img/20260409_introsword.png" loading="lazy"></img>
</div>