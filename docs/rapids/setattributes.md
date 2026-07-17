<style>
.rapids-sets {
  max-width: 1000px;
  color: #293241;
}
.rapids-sets-hero {
  position: relative;
  margin: 1.2em 0 2.3em;
  padding: 1.7em 0 1.25em 1.5em;
  border: 1px solid #e2e7f0;
  border-radius: 0 18px 18px 0;
  border-left: 2px solid #A0A2A4;
  box-shadow: 0 10px 28px rgba(47, 62, 89, .045);
}
.rapids-sets-hero .kicker,
.rapids-sets .eyebrow {
  margin: 0 0 .6em;
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
  letter-spacing: -.04em;
}
.rapids-sets-hero p {
  max-width: 48em;
  margin: 0;
  color: #748094;
  font-size: 1.04em;
  line-height: 1.75;
}
.rapids-sets .hero-meta {
  display: flex;
  flex-wrap: wrap;
  gap: .45em .7em;
  margin-top: 1.2em;
}
.rapids-sets .hero-meta span {
  padding: .28em .65em;
  color: #667691;
  background: rgba(255, 255, 255, .78);
  border: 1px solid #dfe5ef;
  border-radius: 999px;
  font-size: .78em;
  font-weight: 700;
}
.rapids-sets .quick-links {
  display: flex;
  flex-wrap: wrap;
  gap: .55em 1.4em;
  margin: 0 0 2em;
  padding: .65em .8em;
  border-top: 1px solid #edf0f4;
  border-bottom: 1px solid #edf0f4;
  font-size: .9em;
}
.rapids-sets a {
  color: #4f70a5;
  font-weight: 600;
}
.rapids-sets .quick-links a {
  padding: .18em .35em;
  border-radius: .35em;
  transition: color .18s ease, background .18s ease;
}
.rapids-sets .quick-links a:hover {
  color: #344f79;
  background: #f0f4fa;
}
.rapids-sets .unit-note {
  margin: 1.2em 0 2.2em;
  padding: 1em 1.15em;
  color: #59677c;
  background: #f5f7fa;
  border: 1px solid #e1e7ef;
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
  margin: 3em 0 0;
  padding: 1.25em 1.25em 1.4em;
  background: linear-gradient(180deg, var(--soft) 0%, rgba(255, 255, 255, .62) 42%, #fff 100%);
  border: 1px solid #e2e7ef;
  border-radius: 18px;
  box-shadow: 0 10px 28px rgba(47, 62, 89, .035);
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
  margin-bottom: 1.15em;
  padding: .15em 0 .9em .85em;
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
  position: relative;
  padding: 1em 1.05em 1.1em 1.15em;
  background: rgba(255, 255, 255, .9);
  border: 1px solid #e1e7ef;
  border-left: 3px solid var(--accent);
  border-radius: 10px;
  box-shadow: 0 4px 14px rgba(47, 62, 89, .035);
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
  align-items: center;
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
  min-width: 3.15em;
  padding: .12em .35em;
  color: var(--accent);
  background: var(--soft);
  border: 1px solid rgba(160, 170, 195, .35);
  border-radius: 999px;
  font-size: .84em;
  font-weight: 700;
  text-align: center;
}
.rapids-sets .bonus-text {
  color: #536177;
  font-size: .92em;
}
.rapids-sets .bonus-text strong {
  display: inline-block;
  padding: 0 .25em;
  color: var(--accent);
  background: var(--soft);
  border-radius: .3em;
  font-weight: 700;
}
.rapids-sets .closing-note {
  margin: 3.2em 0 1em;
  color: #7b8594;
  font-size: .88em;
  line-height: 1.75;
}
@media (max-width: 720px) {
  .rapids-sets .legend-grid {
    grid-template-columns: 1fr 1fr;
  }
  .rapids-sets .tier-grid {
    grid-template-columns: 1fr;
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
  .rapids-sets .set-section {
    padding: 1em .85em 1.15em;
    border-radius: 14px;
  }
}
/* Editorial pass: one accent, quiet surfaces, and borders that group data. */
.rapids-sets {
  --accent: #4f6f86;
  --soft: #f1f5f7;
  --surface: #ffffff;
  --ink: #293743;
  --muted: #6f7d87;
  --line: #d9e2e7;
  color: var(--ink);
}
.rapids-sets-hero {
  border: 0;
  border-left: 2px solid #A0A2A4;
  border-radius: 0 12px 12px 0;
  box-shadow: none;
}
.rapids-sets-hero .kicker,
.rapids-sets .eyebrow,
.rapids-sets a {
  color: var(--accent);
}
.rapids-sets-hero h1,
.rapids-sets .set-heading h2 {
  color: var(--ink);
}
.rapids-sets-hero p,
.rapids-sets .set-heading p,
.rapids-sets .legend-card span,
.rapids-sets .bonus-text,
.rapids-sets .closing-note {
  color: var(--muted);
}
.rapids-sets .quick-links {
  border-color: var(--line);
}
.rapids-sets .quick-links a:hover {
  color: var(--accent);
  background: var(--soft);
}
.rapids-sets .unit-note {
  color: var(--muted);
  background: var(--soft);
  border: 0;
  border-radius: 0;
}
.rapids-sets code {
  color: var(--accent);
  background: #e7eef1;
  border-radius: 2px;
}
.rapids-sets .legend-grid {
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 0 2em;
  margin: 1.4em 0 2.8em;
}
.rapids-sets .legend-card {
  padding: .9em 0 1em;
  border: 0;
  border-top: 1px solid var(--line);
  border-radius: 0;
  background: transparent;
}
.rapids-sets .legend-card strong,
.rapids-sets .tier-name,
.rapids-sets .bonus-count,
.rapids-sets .bonus-text strong {
  color: var(--accent);
}
.rapids-sets .set-section,
.rapids-sets .set-section.harmony,
.rapids-sets .set-section.origin,
.rapids-sets .set-section.valley,
.rapids-sets .set-section.wind,
.rapids-sets .set-section.river,
.rapids-sets .set-section.mist {
  --accent: #4f6f86;
  --soft: #f1f5f7;
  margin: 3.4em 0 0;
  padding: 1.4em 0 0;
  background: transparent;
  border: 0;
  border-top: 1px solid var(--line);
  border-radius: 0;
  box-shadow: none;
}
.rapids-sets .set-heading {
  margin-bottom: 1.25em;
  padding: 0 0 .9em .85em;
  border: 0;
  border-left: 3px solid var(--accent);
}
.rapids-sets .set-heading h2 {
  font-size: 1.65em;
}
.rapids-sets .set-chip {
  display: none;
}
.rapids-sets .tier-grid {
  gap: 0 2em;
}
.rapids-sets .tier-card {
  position: static;
  min-height: 0;
  padding: 1em .2em 1.15em 1em;
  background: transparent;
  border: 0;
  border-top: 1px solid var(--line);
  border-left: 2px solid var(--accent);
  border-radius: 0;
  box-shadow: none;
}
.rapids-sets .tier-card {
  --quality: var(--accent);
  border-left-color: var(--quality);
}
.rapids-sets .tier-name {
  color: var(--quality);
}
.rapids-sets .quality-mythic { --quality: #FF8080; }
.rapids-sets .quality-legendary { --quality: #FFAA00; }
.rapids-sets .quality-epic { --quality: #CC80CC; }
.rapids-sets .quality-excellent { --quality: #80B0E0; }
.rapids-sets .quality-good { --quality: #65CF65; }
.rapids-sets .quality-common { --quality: #404549; }
.rapids-sets .quality-rough { --quality: #808080; }
.rapids-sets .quality-base { --quality: var(--accent); }
.rapids-sets .tier-top {
  margin-bottom: .8em;
}
.rapids-sets .tier-level {
  color: var(--muted);
}
.rapids-sets .bonus-row + .bonus-row {
  margin-top: .35em;
  padding-top: 0;
  border-top: 0;
}
.rapids-sets .bonus-count {
  min-width: 3.15em;
  padding: 0;
  background: transparent;
  border: 0;
  border-radius: 0;
  text-align: left;
}
.rapids-sets .bonus-text strong {
  padding: 0;
  background: transparent;
}
.rapids-sets .closing-note {
  padding-top: 1em;
  border-top: 1px solid var(--line);
}
@media (prefers-color-scheme: dark) {
  .rapids-sets {
    --accent: #9ab9c5;
    --soft: #19252b;
    --surface: #111b20;
    --ink: #e4edf0;
    --muted: #a9b8bf;
    --line: #3a4a52;
  }
  .rapids-sets-hero,
  .rapids-sets .unit-note {
    background: var(--soft);
  }
  .rapids-sets code {
    color: #b4d2da;
    background: #263840;
  }
  .rapids-sets .quality-common { --quality: #DDDDDD; }
  .rapids-sets .quality-rough { --quality: #B5B5B5; }
}
@media (prefers-reduced-motion: reduce) {
  .rapids-sets .quick-links a {
    transition: none;
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
  </nav>

  ## 数值相关介绍

  <div class="legend-grid">
    <div class="legend-card"><strong>数值</strong>
    <span>固定值通常会出现在魔法相关属性，如：最大法力值、法力恢复等，或前期的套装属性。<br>含百分号则为 <code>百分比属性</code> 如：箭矢速度、移动速度、暴击伤害与经验加成。</span></div>
    <div class="legend-card"><strong>公式</strong><span>以 <code>unit</code> 标注的数值，则表示对应属性基准值。<br>如：生命恢复: +0.75 unit 表示 0.75 基准单位的生命恢复（继承自生命值）<br>参考数值：29 (Lv.10 / 普通)</span></div>
  </div>
  <section class="set-section harmony" id="harmony" style="display: none;">
    <div class="set-heading"><div><h2>和光同尘</h2><p>均衡型套装，随着品质提升强化会心、护甲穿透率与暴击伤害。</p></div></div>
    <div class="tier-grid">
       <article class="tier-card quality-legendary"><div class="tier-top"><span class="tier-name">传奇</span><span class="tier-level">Tier 3</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+25</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透率 <strong>+10%</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">暴击伤害 <strong>+35%</strong></span></div></article>
       <article class="tier-card quality-epic"><div class="tier-top"><span class="tier-name">史诗</span><span class="tier-level">Tier 2</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+20</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透率 <strong>+8%</strong></span></div></article>
       <article class="tier-card quality-excellent"><div class="tier-top"><span class="tier-name">卓越</span><span class="tier-level">Tier 1</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+10</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透率 <strong>+5%</strong></span></div></article>
    </div>
  </section>
  <section class="set-section origin" id="origin">
  <div class="set-heading"><div>

  ## 初生
  
  <p>基础成长套装，提供稳定的经验获取加成。</p></div></div>
    <div class="tier-grid">
       <article class="tier-card quality-epic"><div class="tier-top"><span class="tier-name">史诗</span><span class="tier-level">内测额外奖励</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">经验加成 <strong>+20%</strong></span></div></article>
       <article class="tier-card quality-base"><div class="tier-top"><span class="tier-name">基础套装</span><span class="tier-level">无品质分档</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">经验加成 <strong>+10%</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">经验加成 <strong>+10%</strong></span></div></article>
    </div>
  </section>
  <section class="set-section valley" id="valley">


  <div class="set-heading"><div>

  ## 峡谷
    
  <p>以会心和固定护甲穿透为核心，传奇档位额外提升箭矢与移动能力。</p></div></div>
    <div class="tier-grid">
       <article class="tier-card quality-legendary"><div class="tier-top"><span class="tier-name">传奇</span><span class="tier-level">Tier 6</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+60</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透 <strong>+60</strong> · 箭矢速度 <strong>+20%</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">移动速度 <strong>+15%</strong></span></div></article>
       <article class="tier-card quality-epic"><div class="tier-top"><span class="tier-name">史诗</span><span class="tier-level">Tier 5</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+40</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透 <strong>+40</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">箭矢速度 <strong>+20%</strong></span></div></article>
       <article class="tier-card quality-excellent"><div class="tier-top"><span class="tier-name">卓越</span><span class="tier-level">Tier 4</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+30</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透 <strong>+30</strong></span></div></article>
       <article class="tier-card quality-good"><div class="tier-top"><span class="tier-name">优秀</span><span class="tier-level">Tier 3</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+25</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透 <strong>+25</strong></span></div></article>
       <article class="tier-card quality-common"><div class="tier-top"><span class="tier-name">普通</span><span class="tier-level">Tier 2</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+20</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透 <strong>+20</strong></span></div></article>
       <article class="tier-card quality-rough"><div class="tier-top"><span class="tier-name">粗糙</span><span class="tier-level">Tier 1</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+10</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透 <strong>+10</strong></span></div></article>
    </div>
  </section>
  <section class="set-section wind" id="wind-shape">
  <div class="set-heading"><div>

  ## 风之形
  
  <p>以会心、护甲穿透和机动性为主轴，高品质档位同时强化箭矢速度。</p></div></div>
    <div class="tier-grid">
       <article class="tier-card quality-mythic"><div class="tier-top"><span class="tier-name">神话</span><span class="tier-level">Tier 7</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+90</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透 <strong>+90</strong> · 移动速度 <strong>+35%</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">箭矢速度 <strong>+35%</strong></span></div></article>
       <article class="tier-card quality-legendary"><div class="tier-top"><span class="tier-name">传奇</span><span class="tier-level">Tier 6</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+60</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透 <strong>+60</strong> · 移动速度 <strong>+25%</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">箭矢速度 <strong>+25%</strong></span></div></article>
       <article class="tier-card quality-epic"><div class="tier-top"><span class="tier-name">史诗</span><span class="tier-level">Tier 5</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+40</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">护甲穿透 <strong>+40</strong> · 移动速度 <strong>+20%</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">箭矢速度 <strong>+20%</strong></span></div></article>
       <article class="tier-card quality-excellent"><div class="tier-top"><span class="tier-name">卓越</span><span class="tier-level">Tier 4</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+30</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">移动速度 <strong>+15%</strong></span></div></article>
       <article class="tier-card quality-good"><div class="tier-top"><span class="tier-name">优秀</span><span class="tier-level">Tier 3</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">会心 <strong>+25</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">移动速度 <strong>+10%</strong></span></div></article>
    </div>
  </section>
  <section class="set-section river" id="river-gate">
  <div class="set-heading"><div>

  ## 河隘
  
  <p>围绕柔韧与魔法穿透构筑，较高档位补充法力上限与法力恢复。</p></div></div>
    <div class="tier-grid">
       <article class="tier-card quality-legendary"><div class="tier-top"><span class="tier-name">传奇</span><span class="tier-level">Tier 6</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>1.5 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>3 unit</strong> · 最大法力值 <strong>+50</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">法力恢复 <strong>+1.5 P/s</strong></span></div></article>
       <article class="tier-card quality-epic"><div class="tier-top"><span class="tier-name">史诗</span><span class="tier-level">Tier 5</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>1 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>2 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">法力恢复 <strong>+0.75 P/s</strong></span></div></article>
       <article class="tier-card quality-excellent"><div class="tier-top"><span class="tier-name">卓越</span><span class="tier-level">Tier 4</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>0.75 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>1.5 unit</strong></span></div></article>
       <article class="tier-card quality-good"><div class="tier-top"><span class="tier-name">优秀</span><span class="tier-level">Tier 3</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>0.625 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>1.25 unit</strong></span></div></article>
       <article class="tier-card quality-common"><div class="tier-top"><span class="tier-name">普通</span><span class="tier-level">Tier 2</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>0.5 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>1 unit</strong></span></div></article>
       <article class="tier-card quality-rough"><div class="tier-top"><span class="tier-name">粗糙</span><span class="tier-level">Tier 1</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>0.25 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>0.5 unit</strong></span></div></article>
    </div>
  </section>
  
  <section class="set-section mist" id="river-mist">
  <div class="set-heading">
  <div>

  ## 河雾
    
  <p>以柔韧、魔法穿透和法力循环为核心；神话档位额外提供移动速度与生命恢复。</p>
  </div>
  </div>
    <div class="tier-grid">
       <article class="tier-card quality-mythic"><div class="tier-top"><span class="tier-name">神话</span><span class="tier-level">Tier 7</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>1.5 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>4.5 unit</strong> · 最大法力值 <strong>+50</strong> · 移动速度 <strong>+20%</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">生命恢复 <strong>0.25 unit</strong> · 法力恢复 <strong>+1.5 P/s</strong></span></div></article>
       <article class="tier-card quality-legendary"><div class="tier-top"><span class="tier-name">传奇</span><span class="tier-level">Tier 6</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>1.5 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>3 unit</strong> · 最大法力值 <strong>+50</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">法力恢复 <strong>+1.5 P/s</strong></span></div></article>
       <article class="tier-card quality-epic"><div class="tier-top"><span class="tier-name">史诗</span><span class="tier-level">Tier 5</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>1 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>2 unit</strong> · 最大法力值 <strong>+30</strong></span></div><div class="bonus-row"><span class="bonus-count">5 件</span><span class="bonus-text">法力恢复 <strong>+0.75 P/s</strong></span></div></article>
       <article class="tier-card quality-excellent"><div class="tier-top"><span class="tier-name">卓越</span><span class="tier-level">Tier 4</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>0.75 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>1.5 unit</strong></span></div></article>
       <article class="tier-card quality-good"><div class="tier-top"><span class="tier-name">优秀</span><span class="tier-level">Tier 3</span></div><div class="bonus-row"><span class="bonus-count">2 件</span><span class="bonus-text">柔韧 <strong>0.625 unit</strong></span></div><div class="bonus-row"><span class="bonus-count">4 件</span><span class="bonus-text">魔法穿透 <strong>1.25 unit</strong></span></div></article>
    </div>
  </section>
  <p class="closing-note"><strong>说明：</strong>Tier 表示套装档位。套装门槛按穿着件数累计，跨品质组合时，高品质部件可向下兼容低品质部件并生效低品质套装属性。</p>
</div>
