<style>
.rapids-sets {
  max-width: 1000px;
  color: #293241;
}
.rapids-sets-hero {
  margin: 1.2em 0 1.8em;
  padding: 1.8em 0 1.35em 1.5em;
  border-left: 3px solid #8090e0;
}
.rapids-sets-hero .kicker,
.rapids-sets .eyebrow {
  margin: 0 0 .65em;
  color: #7b8799;
  font-size: .76em;
  font-weight: 700;
  letter-spacing: .16em;
}
.rapids-sets-hero h1 {
  margin: 0 0 .35em;
  color: #202b3c;
  font-size: 2.35em;
  font-weight: 650;
  letter-spacing: -.045em;
}
.rapids-sets-hero p {
  max-width: 48em;
  margin: 0;
  color: #748094;
  font-size: 1.04em;
  line-height: 1.75;
}
.rapids-sets .quick-links {
  display: flex;
  flex-wrap: wrap;
  gap: .55em 1.4em;
  margin: 0 0 2em;
  font-size: .9em;
}
.rapids-sets a {
  color: #4f70a5;
  font-weight: 600;
}
.rapids-sets .unit-note {
  margin: 1.2em 0 2.2em;
  padding: 1em 1.15em;
  color: #59677c;
  background: #f5f7fa;
  border: 1px solid #e1e7ef;
  border-left: 3px solid #70d0c8;
  line-height: 1.75;
}
.rapids-sets .unit-note p {
  margin: .35em 0 0;
}
.rapids-sets code {
  padding: .12em .35em;
  color: #49658b;
  background: #edf3f8;
  border-radius: .35em;
}
.rapids-sets .legend-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 12px;
  margin: 1.2em 0 3em;
}
.rapids-sets .legend-card {
  padding: 1em 1.05em;
  border: 1px solid #e1e7ef;
  border-radius: 10px;
  background: #fff;
}
.rapids-sets .legend-card strong {
  display: block;
  margin-bottom: .35em;
  color: #415a83;
  font-size: .92em;
}
.rapids-sets .legend-card span {
  color: #7b8594;
  font-size: .86em;
  line-height: 1.65;
}
.rapids-sets .set-section {
  --accent: #5969b0;
  --soft: #f5f6fc;
  margin: 3.2em 0 0;
}
.rapids-sets .set-section.harmony { --accent: #bd7a5d; --soft: #fff7f0; }
.rapids-sets .set-section.origin { --accent: #5d8db7; --soft: #f2f8fc; }
.rapids-sets .set-section.valley { --accent: #5969b0; --soft: #f3f5ff; }
.rapids-sets .set-section.wind { --accent: #9b5cb2; --soft: #fbf4fd; }
.rapids-sets .set-section.river { --accent: #348f8a; --soft: #f0fbfa; }
.rapids-sets .set-section.mist { --accent: #777fa9; --soft: #f5f6fc; }
.rapids-sets .set-heading {
  display: flex;
  align-items: flex-end;
  justify-content: space-between;
  gap: 1.5em;
  margin-bottom: 1.1em;
  padding: 0 0 .8em 1em;
  border-bottom: 1px solid #dce3ec;
  border-left: 3px solid var(--accent);
}
.rapids-sets .set-heading h2 {
  margin: 0 0 .3em;
  padding: 0;
  color: #283852;
  border: 0;
  font-size: 1.55em;
  font-weight: 650;
  letter-spacing: -.025em;
}
.rapids-sets .set-heading p {
  margin: 0;
  color: #7b8594;
  font-size: .9em;
  line-height: 1.65;
}
.rapids-sets .set-chip {
  flex: none;
  padding: .4em .75em;
  color: var(--accent);
  background: var(--soft);
  border: 1px solid color-mix(in srgb, var(--accent) 25%, white);
  border-radius: 999px;
  font-size: .78em;
  font-weight: 700;
}
.rapids-sets .tier-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 14px 18px;
}
.rapids-sets .tier-card {
  padding: 1em 1.05em 1.1em;
  background: linear-gradient(135deg, var(--soft), #fff 58%);
  border: 1px solid #e1e7ef;
  border-top: 2px solid var(--accent);
  border-radius: 10px;
}
.rapids-sets .tier-top {
  display: flex;
  align-items: baseline;
  justify-content: space-between;
  gap: 1em;
  margin-bottom: .75em;
}
.rapids-sets .tier-name {
  color: var(--accent);
  font-size: 1.04em;
  font-weight: 700;
}
.rapids-sets .tier-level {
  color: #8b95a3;
  font-size: .78em;
  letter-spacing: .06em;
}
.rapids-sets .bonus-row {
  display: flex;
  align-items: baseline;
  gap: .75em;
  line-height: 1.65;
}
.rapids-sets .bonus-row + .bonus-row {
  margin-top: .5em;
  padding-top: .5em;
  border-top: 1px solid rgba(220, 227, 236, .75);
}
.rapids-sets .bonus-count {
  flex: none;
  min-width: 2.55em;
  color: #748094;
  font-size: .84em;
  font-weight: 700;
}
.rapids-sets .bonus-text {
  color: #536177;
  font-size: .92em;
}
.rapids-sets .bonus-text strong {
  color: var(--accent);
  font-weight: 700;
}
.rapids-sets .closing-note {
  margin: 3.2em 0 1em;
  color: #7b8594;
  font-size: .88em;
  line-height: 1.75;
}
@media (max-width: 720px) {
  .rapids-sets .legend-grid,
  .rapids-sets .tier-grid {
    grid-template-columns: 1fr 1fr;
  }
  .rapids-sets .set-heading {
    align-items: flex-start;
    flex-direction: column;
    gap: .7em;
  }
}
@media (max-width: 460px) {
  .rapids-sets .legend-grid,
  .rapids-sets .tier-grid {
    grid-template-columns: 1fr;
  }
  .rapids-sets-hero h1 {
    font-size: 2em;
  }
}
</style>
<div class="rapids-sets">
  <header class="rapids-sets-hero">
    <p class="kicker">RAPIDS / SET ATLAS</p>
    <h1>套装属性</h1>
    <p>套装效果按穿着件数逐段解锁。这里集中披露当前配置中的套装门槛、属性类型与数值，不展开单件装备的基础属性。</p>
  </header>
  <nav class="quick-links">
    <a href="#/rapids/dungeon">副本流程</a>
    <a href="#/rapids/dungeonlist">副本图鉴</a>
    <a href="#/rapids/materials">材料图鉴</a>
    <a href="#/rapids/combat_system">战斗系统</a>
  </nav>
  <div class="unit-note">
    <strong>数值阅读方式</strong>
    <p><code>unit</code> 表示配置中的等级缩放基准单位，不是固定面板数值。例如 <code>0.75 unit</code> 表示对应基准值的 0.75 倍；这里保留倍率，省略后台公式。百分比属性直接以百分比显示，法力与生命恢复则按恢复速度理解。</p>
  </div>
  <div class="legend-grid">
    <div class="legend-card"><strong>固定属性</strong><span>会心、柔韧、护甲穿透、魔法穿透、最大法力值。</span></div>
    <div class="legend-card"><strong>百分比属性</strong><span>护甲穿透率、箭矢速度、移动速度、暴击伤害、经验加成。</span></div>
    <div class="legend-card"><strong>恢复属性</strong><span>法力恢复以 P/s 表示；生命恢复若使用 unit，则随对应基准值缩放。</span></div>
  </div>
  <section class="set-section harmony" id="harmony">
    <div class="set-heading"><div><p class="eyebrow">SET / 和光同尘</p><h2>和光同尘</h2><p>均衡型套装，随着品质提升强化会心、护甲穿透率与暴击伤害。</p></div><span class="set-chip">会心 · 穿透率 · 暴击</span></div>
    <div class="tier-grid">
      <article class="tier-card"><div class="tier-top"><span class="tier-name">传奇</span><span class="tier-level">Tier 3</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+25</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透率 <strong>+10%</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">暴击伤害 <strong>+35%</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">史诗</span><span class="tier-level">Tier 2</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+20</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透率 <strong>+8%</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">卓越</span><span class="tier-level">Tier 1</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+10</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透率 <strong>+5%</strong></span></div></article>
    </div>
  </section>
  <section class="set-section origin" id="origin">
    <div class="set-heading"><div><p class="eyebrow">SET / 初生</p><h2>初生</h2><p>基础成长套装，提供稳定的经验获取加成。</p></div><span class="set-chip">经验加成</span></div>
    <div class="tier-grid">
      <article class="tier-card"><div class="tier-top"><span class="tier-name">基础套装</span><span class="tier-level">无品质分档</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">经验加成 <strong>+10%</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">经验加成 <strong>+10%</strong></span></div></article>
    </div>
  </section>
  <section class="set-section valley" id="valley">
    <div class="set-heading"><div><p class="eyebrow">SET / 峡谷</p><h2>峡谷</h2><p>以会心和固定护甲穿透为核心，传奇档位额外提升箭矢与移动能力。</p></div><span class="set-chip">会心 · 护甲穿透</span></div>
    <div class="tier-grid">
      <article class="tier-card"><div class="tier-top"><span class="tier-name">传奇</span><span class="tier-level">Tier 6</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+60</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透 <strong>+60</strong> · 箭矢速度 <strong>+20%</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">移动速度 <strong>+15%</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">史诗</span><span class="tier-level">Tier 5</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+40</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透 <strong>+40</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">箭矢速度 <strong>+20%</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">卓越</span><span class="tier-level">Tier 4</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+30</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透 <strong>+30</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">优秀</span><span class="tier-level">Tier 3</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+25</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透 <strong>+25</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">普通</span><span class="tier-level">Tier 2</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+20</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透 <strong>+20</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">粗糙</span><span class="tier-level">Tier 1</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+10</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透 <strong>+10</strong></span></div></article>
    </div>
  </section>
  <section class="set-section wind" id="wind-shape">
    <div class="set-heading"><div><p class="eyebrow">SET / 风之形</p><h2>风之形</h2><p>以会心、护甲穿透和机动性为主轴，高品质档位同时强化箭矢速度。</p></div><span class="set-chip">会心 · 机动 · 箭矢</span></div>
    <div class="tier-grid">
      <article class="tier-card"><div class="tier-top"><span class="tier-name">神话</span><span class="tier-level">Tier 6</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+90</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透 <strong>+90</strong> · 移动速度 <strong>+35%</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">箭矢速度 <strong>+35%</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">传奇</span><span class="tier-level">Tier 5</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+60</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透 <strong>+60</strong> · 移动速度 <strong>+25%</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">箭矢速度 <strong>+25%</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">史诗</span><span class="tier-level">Tier 4</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+40</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透 <strong>+40</strong> · 移动速度 <strong>+20%</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">箭矢速度 <strong>+20%</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">卓越</span><span class="tier-level">Tier 3</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+30</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">移动速度 <strong>+15%</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">优秀</span><span class="tier-level">Tier 2</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+25</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">移动速度 <strong>+10%</strong></span></div></article>
    </div>
  </section>
  <section class="set-section river" id="river-gate">
    <div class="set-heading"><div><p class="eyebrow">SET / 河隘</p><h2>河隘</h2><p>围绕柔韧与魔法穿透构筑，较高档位补充法力上限与法力恢复。</p></div><span class="set-chip">柔韧 · 魔法穿透</span></div>
    <div class="tier-grid">
      <article class="tier-card"><div class="tier-top"><span class="tier-name">传奇</span><span class="tier-level">Tier 6</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>1.5 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>3 unit</strong> · 最大法力值 <strong>+50</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">法力恢复 <strong>+1.5 P/s</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">史诗</span><span class="tier-level">Tier 5</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>1 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>2 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">法力恢复 <strong>+0.75 P/s</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">卓越</span><span class="tier-level">Tier 4</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>0.75 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>1.5 unit</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">优秀</span><span class="tier-level">Tier 3</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>0.625 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>1.25 unit</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">普通</span><span class="tier-level">Tier 2</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>0.5 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>1 unit</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">粗糙</span><span class="tier-level">Tier 1</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>0.25 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>0.5 unit</strong></span></div></article>
    </div>
  </section>
  <section class="set-section mist" id="river-mist">
    <div class="set-heading"><div><p class="eyebrow">SET / 河雾</p><h2>河雾</h2><p>以柔韧、魔法穿透和法力循环为核心；神话档位额外提供移动速度与生命恢复。</p></div><span class="set-chip">柔韧 · 法力 · 恢复</span></div>
    <div class="tier-grid">
      <article class="tier-card"><div class="tier-top"><span class="tier-name">神话</span><span class="tier-level">Tier 7</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>1.5 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>4.5 unit</strong> · 最大法力值 <strong>+50</strong> · 移动速度 <strong>+20%</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">生命恢复 <strong>0.25 unit</strong> · 法力恢复 <strong>+1.5 P/s</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">传奇</span><span class="tier-level">Tier 6</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>1.5 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>3 unit</strong> · 最大法力值 <strong>+50</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">法力恢复 <strong>+1.5 P/s</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">史诗</span><span class="tier-level">Tier 5</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>1 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>2 unit</strong> · 最大法力值 <strong>+30</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">法力恢复 <strong>+0.75 P/s</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">卓越</span><span class="tier-level">Tier 4</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>0.75 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>1.5 unit</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">优秀</span><span class="tier-level">Tier 3</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>0.625 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>1.25 unit</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">普通</span><span class="tier-level">Tier 2</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>0.5 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>1 unit</strong></span></div></article>
      <article class="tier-card"><div class="tier-top"><span class="tier-name">粗糙</span><span class="tier-level">Tier 1</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>0.25 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>0.5 unit</strong></span></div></article>
    </div>
  </section>
  <p class="closing-note"><strong>说明：</strong>本页按照 ZeroAttribute 的套装配置整理；Tier 表示配置中的套装档位。套装门槛按穿着件数累计，达到更高门槛时，较低门槛效果仍保留。</p>
</div>
