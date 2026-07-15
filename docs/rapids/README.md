<style>
.rapids-home {
  --home-ink: #263443;
  --home-muted: #718092;
  --home-line: #dde5eb;
  --home-surface: #f7f9fb;
  --home-accent: #416e9f;
  --home-accent-soft: #edf3f8;
  max-width: min(980px, 92vw);
  color: var(--home-ink);
}

.rapids-home * { box-sizing: border-box; }

.rapids-home-hero {
  margin: 1.2em 0 2.5em;
  padding: clamp(1.5rem, 5vw, 3rem);
  background: var(--home-surface);
  border: 1px solid var(--home-line);
  border-radius: 14px;
}

.rapids-home-hero .eyebrow {
  margin: 0 0 .75rem;
  color: var(--home-accent);
  font-size: .76rem;
  font-weight: 750;
  letter-spacing: .12em;
}

.rapids-home-hero h1 {
  margin: 0 0 .65rem;
  color: #20313d;
  font-size: clamp(2.4rem, 7vw, 4.2rem);
  font-weight: 730;
  letter-spacing: -.06em;
  line-height: 1;
}

.rapids-home-hero .lead {
  max-width: 39rem;
  margin: 0;
  color: var(--home-muted);
  font-size: 1.02rem;
  line-height: 1.75;
}

.rapids-home-actions {
  display: flex;
  flex-wrap: wrap;
  gap: .65rem;
  margin-top: 1.25rem;
}

.rapids-home-actions a {
  display: inline-flex;
  align-items: center;
  min-height: 2.55rem;
  padding: .55rem .9rem;
  color: #fff;
  background: var(--home-accent);
  border: 1px solid var(--home-accent);
  border-radius: 10px;
  font-size: .88rem;
  font-weight: 680;
  text-decoration: none;
}

.rapids-home-actions a.secondary {
  color: var(--home-accent);
  background: transparent;
}

.rapids-home h2 {
  margin: 0 0 .4rem;
  color: var(--home-ink);
  font-size: 1.4rem;
  font-weight: 700;
  letter-spacing: -.025em;
}

.rapids-home .section-intro {
  margin: 0 0 1.15rem;
  color: var(--home-muted);
  line-height: 1.65;
}

.rapids-home-grid {
  display: grid;
  grid-template-columns: repeat(12, minmax(0, 1fr));
  gap: .75rem;
  margin-bottom: 2.7rem;
}

.rapids-home-link {
  grid-column: span 4;
  min-height: 8.2rem;
  padding: 1rem 1.05rem;
  color: inherit;
  background: #fff;
  border: 1px solid var(--home-line);
  border-radius: 12px;
  text-decoration: none;
}

.rapids-home-link.wide { grid-column: span 6; }

.rapids-home-link strong {
  display: block;
  margin-bottom: .45rem;
  color: var(--home-ink);
  font-size: 1rem;
}

.rapids-home-link span {
  color: var(--home-muted);
  font-size: .86rem;
  line-height: 1.55;
}

.rapids-home-link.featured {
  background: var(--home-accent-soft);
  border-color: #cad9e6;
}

.rapids-home-link.featured strong { color: var(--home-accent); }

.rapids-home-footnote {
  padding-top: 1rem;
  color: var(--home-muted);
  border-top: 1px solid var(--home-line);
  font-size: .84rem;
  line-height: 1.65;
}

@media (max-width: 760px) {
  .rapids-home-link,
  .rapids-home-link.wide { grid-column: span 6; }
}

@media (max-width: 520px) {
  .rapids-home-hero { padding: 1.3rem; }
  .rapids-home-link,
  .rapids-home-link.wide { grid-column: 1 / -1; min-height: auto; }
  .rapids-home-actions a { width: 100%; justify-content: center; }
}

@media (prefers-reduced-motion: no-preference) {
  .rapids-home-actions a,
  .rapids-home-link {
    transition: transform .2s ease, border-color .2s ease, box-shadow .2s ease;
  }

  .rapids-home-actions a:active { transform: translateY(1px); }

  .rapids-home-link:hover {
    border-color: #aebfce;
    box-shadow: 0 8px 22px rgba(40, 70, 94, .08);
    transform: translateY(-2px);
  }
}
</style>

<main class="rapids-home">
  <header class="rapids-home-hero">
    <p class="eyebrow">DP IV / RAPIDS WIKI</p>
    <h1>激流</h1>
    <p class="lead">围绕副本探索、角色构筑与长期成长展开的 Minecraft RPG 服务器内容。这里集中披露玩法规则、图鉴资料与版本变化。</p>
    <div class="rapids-home-actions">
      <a href="#/rapids/dungeon">了解副本流程</a>
      <a class="secondary" href="#/rapids/updatelogs">查看最近更新</a>
    </div>
  </header>

  <section aria-labelledby="rapids-content-title">
    <h2 id="rapids-content-title">内容披露</h2>
    <p class="section-intro">从玩法概览开始，或直接进入需要查询的资料。</p>
    <div class="rapids-home-grid">
      <a class="rapids-home-link wide featured" href="#/rapids/rapids"><strong>服务器介绍</strong><span>了解 Rapids 的设计方向、测试阶段与核心玩法。</span></a>
      <a class="rapids-home-link wide" href="#/rapids/dungeon"><strong>副本流程</strong><span>进入、探索、结算与再入，一次副本的完整过程。</span></a>
      <a class="rapids-home-link" href="#/rapids/dungeonlist"><strong>副本图鉴</strong><span>查看各区域、难度、推荐等级与开放状态。</span></a>
      <a class="rapids-home-link" href="#/rapids/dungeonmechanics"><strong>副本机制</strong><span>评分、宝箱、采集物与特殊怪物规则。</span></a>
      <a class="rapids-home-link featured" href="#/rapids/mobsinfo"><strong>怪物信息</strong><span>查看怪物技能、触发条件和实战应对方法。</span></a>
      <a class="rapids-home-link" href="#/rapids/materials"><strong>材料图鉴</strong><span>材料来源、品质、用途与配方需求。</span></a>
      <a class="rapids-home-link" href="#/rapids/setattributes"><strong>套装属性</strong><span>查询套装部件、激活条件与属性效果。</span></a>
      <a class="rapids-home-link" href="#/rapids/design"><strong>设计说明</strong><span>阅读玩法目标、数值框架与开发思路。</span></a>
    </div>
  </section>

  <p class="rapids-home-footnote">披露内容会随服务器版本调整。数值与机制发生变化时，以最新更新记录和游戏内实际表现为准。</p>
</main>
