<style>
.dptag {
  color: #f0f0f0;
  background-color: #538aec;
  text-shadow: 0.5px 1px 0.5px rgba(0, 0, 0, 0.25);
  padding: 2px 3px;
  margin: 0 2px;
  border-radius: 2px;
  font-family: 等线;
  font-weight: 500;
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

.tag-graypurple {
  background: #987eaa;
  padding: 4px 6px;
  border-radius: 6px;
}

.tag-gray {
  background: #989899;
}

.tag-cyan {
  background: #9999cc;
}

.cards-container {
  display: flex;
  max-width: 1000px;
  flex-direction: column;
  gap: 20px;
}

.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 280px));
  gap: 18px;
  align-items: stretch;
}

.card {
  display: flex;
  flex-direction: column;
  background: #ffffff;
  font-size: 15px;
  border-radius: 8px;
  min-width: 0;
  max-width: 275px;
  min-height: 170px;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15);
  text-shadow: none;
  transition: all 0.3s ease;
  overflow: hidden;
  text-decoration: none;
  color: #606974;
}

.acards {
  --card-title-bg: linear-gradient(135deg, #538aec, #7a31aa);
}

.card-title {
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 74px;
  padding: 16px 18px;
  background: var(--card-title-bg, #538aec);
  color: #fffffff8;
  text-align: center;
  font-size: 2em;
  font-weight: 800;
  line-height: 1.2;
  text-shadow: 0 1px 4px rgba(0, 0, 0, 0.15);
}

.card-body {
  display: flex;
  flex-direction: column;
  flex: 1;
  min-height: 240px;
  padding: 14px 16px 16px;
  color: #606974;
  text-align: left;
  font-size: 0.92em;
  font-weight: 400;
  line-height: 1.55;
}

.card-body strong {
  color: #7a31aa;
  font-weight: 700;
}

.card-copy {
  flex: 1;
}

.card-link {
  align-self: stretch;
  margin-top: 18px;
  padding: 9px 12px;
  border-radius: 6px;
  background: linear-gradient(135deg, rgba(83, 138, 236, 0.07), rgba(122, 49, 170, 0.08));
  color: #5873b9;
  text-align: center;
  font-size: 0.92em;
  font-weight: 700;
  line-height: 1.25;
  transition: background 0.25s ease, color 0.25s ease;
}

.card:hover .card-link {
  background: linear-gradient(135deg, rgba(83, 138, 236, 0.16), rgba(122, 49, 170, 0.18));
  color: #6c4ab2;
}

.card:hover {
  box-shadow: 0 1px 10px rgba(0, 0, 0, 0.2);
  transform: translateY(-1px);
}


.markdown-section a {
    color: var(--force-text-fill-color, --theme-color, #538aec)
}

.markdown-section a.card {
  color: #606974;
}

* {
  font-family: 'PingFang SC', 'SF Pro', 'Hiragino Sans GB', '等线', 'Microsoft YaHei', '微软雅黑', 'Helvetica Neue', 'Helvetica', 'Arial', 'sans-serif';
  --force-text-fill-color: #6080b6;
}

.markdown-section {
  max-width: 1200px;
}

:root {
  --quality-color-legendary: #7ec5ff;
  --quality-color-unique: #ff5cf7;
  --quality-color-mythic: #ff3939;
}

.context {
  max-width: 1000px;
}

.markdown-section code {
  font-family: 'Inter', 'Roboto Mono', 'Monaco', 'courier', 'monospace';
}

.redtext {
  color: #f84040; 
  font-weight: 600;
}

.quote {
  background: #fbfdff;
  color: #606974;
  border: 1px dashed #ccc;
  border-radius: 5px;
  font-size: 18px;
  padding: 5px;
  margin: 0px;
}

.table-container {
  overflow-x: auto;
  -webkit-overflow-scrolling: touch;
}

.maintitle {
  font-size: 24px;
  font-weight: 800;
  margin: 0.6rem 0;
  color: #333;
  line-height: 1.8;
}

.box-context {
  font-size: 16px;
  font-weight: 500;
  color: #888;
  line-height: 1.35;
  text-align: left;
  margin: 12px 24px;
  padding: 12px 0;

  &:hover {
    color: transparent;
  }

  @media (max-width: 768px) {
    margin: 0;
    padding: 12px 4px;
  }

}

.redbox {
  background: #fdf4f4;
  color: #85553e;
  box-shadow: 0 0 6px #441313a0;
  border-radius: 18px;
  font-size: 20px;
  font-weight: 600;
  text-align: center;
  padding: 20px;
  margin: 0px;
}

.greenbox {
  background: #f4fdf7;
  color: #3e854f;
  border: 1px solid #40924e;
  border-radius: 18px;
  font-size: 20px;
  font-weight: 600;
  text-align: center;
  padding: 20px;
  margin: 0px;
}

.bluebox {
  background: #f2faff;
  color: #466fa1;
  border: 1px solid #5b9abe;
  border-radius: 18px;
  font-size: 20px;
  font-weight: 600;
  text-align: center;
  padding: 20px;
  margin: 0px;
}

.yellowbox {
  background: #fff9f1;
  color: #c5985c;
  border: 1px solid #cfae8f;
  border-radius: 18px;
  font-size: 20px;
  font-weight: 600;
  text-align: center;
  padding: 20px;
  margin: 0px;
}

.quote-hl {
  display: inline-block;
  background-color:rgb(248, 248, 248);
  color:rgb(240, 25, 211);
  border-radius: 3px;
  margin: 3px;
  padding: 0px 3px;
}

.markdown-section img:not([width]):not([style]) {
  max-width: 600px;
  height: auto;
  max-height: 400px;
}

.markdown-section h1 {
  font-size: 2em;
  font-weight: 800;
  text-shadow: 0 0 1px rgba(0,0,0,0.25);
  font-family: 'Times New Roman';
}

.markdown-section h2 {
  font-size: 1.75em;
  font-weight: 800;
  font-family: 'Times New Roman';
  margin: 1em 0 0.2em;
}

.markdown-section h3 {
  font-size: 1.5em;
  font-weight: 600;
  font-family: 'Times New Roman';
  margin: 0.75em 0 0.2em;
}

.markdown-section h4 {
  font-size: 1.25em;
  margin: 0.5em 0 0.2em;
}

.markdown-section figure, .markdown-section p {
  margin: 0;
}

.inline-tips {
  position: relative;
  margin: 5px 7px;
  padding: 1px 12px;
  font-size: 16px;
  line-height: 1.5;
  color: #999;
  max-width: 750px;

  &::before {
    content: "";
    position: absolute;
    left: 0;
    top: 50%;
    transform: translateY(-50%);
    width: 5px;
    height: 20px;
    background: rgb(180, 180, 180);
    border-radius: 4px;
  }

  &:hover::before {
    content: "";
    position: absolute;
    left: 0;
    top: 50%;
    transform: translateY(-50%);
    width: 5px;
    height: 20px;
    background: rgb(146, 173, 230);
    border-radius: 4px;
  }
}

.little-tips {
  max-width: 360px;
  padding: 1em;
  box-shadow: 0 0 4px #3f9c4380;
  background: #f8fffa;
  border-radius: 1em;
  font-size: 14px;
  margin: 8px 0;
  display: flex;
  gap: 1em;
  align-items: center;
}

.little-tips-blue {
  box-shadow: 0 0 4px #5d8cb6a0;
  background: #f7fcff;
}

.little-tips-purple {
  box-shadow: 0 0 4px #a45db6a0;
  background: #fef7ff;
}
.little-tips-pink {
  box-shadow: 0 0 4px #ca6ac2a0;
  background: #fff7ff;
}

.item-name-tag {
  background: #faf7f5;
  padding: 1px 4px;
  border-radius: 4px;
  margin: 4px;
  font-weight: 600;
  color: #333;
  box-shadow: 0 0 1px rgba(46, 22, 6, 0.1);
}

.number-block {
  display: inline-block;
  width: var(--width, 8em);
  background: rgb(250, 252, 254);
  box-shadow: 0 1px 2px rgba(11, 36, 87, 0.15);
  border-radius: 6px;
  padding: 0.5px 6px;
  line-height: 1.33;
  text-align: center;
  font-size: 0.8rem;
  font-family: 'Roboto Mono', Monaco, courier, monospace, 'CONSOLA';
  font-weight: 500;
  color: rgb(135, 115, 228);
}

.nowrap {
  display: inline-block;
  text-decoration: inherit;
  white-space: nowrap;
}

.highlight-purple {
  font-weight: 600;
  color: rgba(0,0,0,0.75);
  padding: 0 4px;
  border-radius: 20px 20px 10px 10px; 
  background: linear-gradient(
    to bottom, 
    transparent, 
    transparent 30%, 
    rgba(228, 212, 248, 0.6) 50%, 
    rgba(192, 180, 220, 0.5) 100%
  );
}

details[open] {
  margin: 0.5em 0;
  transition: margin 0.25s ease-in-out;
  background: rgba(170, 177, 187, 0.07);
  width: max-content;
  border-radius: 0.5em;
  padding: 0.25em 0.5em;
}

details {
  transition: margin 0.25s ease-in-out;
}

@media (max-width: 768px) {
  .markdown-section img:not([width]):not([style]) {
    width: 100%;
    max-width: 400px;
  }
  
  .cards {
    grid-template-columns: minmax(0, 1fr);
  }

  .card {
    width: 100%;
  }
}

</style>

# 增值服务

<p style="border-left: 5px solid #745691ff; color: #826199ff; padding-left: 10px;">
敝服属于商业服，不可避免会出现影响平衡之特权或物资。如对此不满，敬请谅解。<br>
尽管如此，您仍可在无任何赞助的情况下获得较完整的游戏体验。<br>
除此之外，社区支援（包括自发宣传、Wiki维护等）亦是我们认可的赞助行为。
</p>

## 简介

为了DP的健康成长，我们需要你的支援。<br>
服务器的运行维护、硬件维新都代表着一笔笔高昂的支出。<br>
内容创新、地图创作等方面受到赞助也可以获得更大的动力。**你的支援**可以使得我坚持更好地完成服务器更新与运营。<br>
通过赞助，你可以获得诸多特权或数值、道具回赠。

## 可选择的赞助方向

<div class="cards" style="padding: 2em 0 ;">

<a href="#/pages/月卡" class="card acards">
<div class="card-title" style="background: linear-gradient(135deg, oklch(0.7 0.18 300), oklch(0.85 0.2 60))">月卡</div>
<div class="card-body">
<div class="card-copy">
月卡是我们提供的一种 <strong>订阅制服务</strong>。<br>通过订阅月卡，你可以在期限内获得额外的资源、便利功能，获得较佳的游戏体验。
</div>
<div class="card-link">查看月卡介绍 ▶</div>
</div>
</a>

<a href="#/pages/regularrune" class="card acards">
<div class="card-title" style="background: linear-gradient(135deg, oklch(0.7941 0.1135 224.47), oklch(0.6294 0.1973 308.12))">符文</div>
<div class="card-body">
<div class="card-copy">
制式符文是一类可通过 <strong>Kc</strong> 购买的属性强化道具。<br>它们拥有固定搭配，可独立提供额外属性，也可通过核心符文与附属符文的组合进一步整理符文位。
</div>
<div class="card-link">查看符文介绍 ▶</div>
</div>
</a>

<a href="#/pages/supplybox" class="card acards">
<div class="card-title" style="background: linear-gradient(135deg, oklch(0.62 0.16 225), oklch(0.78 0.17 150))">补给箱</div>
<div class="card-body">
<div class="card-copy">
补给箱是一类使用后可立即获得资源的消耗性道具。<br>通常分为 <strong>装备型补给箱</strong> 与 <strong>抽奖型补给箱</strong>，可用于获取指定装备、材料或奖池中的高价值奖品。
</div>
<div class="card-link">查看补给箱介绍 ▶</div>
</div>
</a>

</div>

## 赞助渠道

通过联系 <span class="dptag tag-graypurple">Atenls (<span>atenls</span>@dp4.us)</span> 以进行你的赞助。

我们支持以下付款渠道：
- 微信(WechatPay)
- WeChatPay HK
- 支付宝(Alipay)
- AlipayHK
- PayPal
- 转数快(FPS)

所有物资或服务的定价基于 `CNY`，如你在付款时使用其他货币，以付款时汇率为准，如涉及服务费或手续费，需由付款者承担。