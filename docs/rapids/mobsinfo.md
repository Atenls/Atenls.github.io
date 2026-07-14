<style>
.mob-atlas {
  --mob-accent: #348f8a;
  --mob-accent-strong: #256f6b;
  --mob-accent-soft: #e9f5f3;
  --mob-ink: #263443;
  --mob-muted: #718092;
  --mob-line: #dce6e8;
  --mob-surface: #f7fafb;
  max-width: 980px;
  color: var(--mob-ink);
}

.mob-atlas * { box-sizing: border-box; }

.mob-atlas-hero {
  display: grid;
  grid-template-columns: minmax(0, 1.45fr) minmax(250px, .7fr);
  gap: clamp(1.5rem, 5vw, 4.5rem);
  align-items: end;
  margin: 1.2em 0 2.4em;
  padding: clamp(1.3rem, 4vw, 2.2rem);
  background: var(--mob-surface);
  border: 1px solid var(--mob-line);
  border-radius: 14px;
}

.mob-atlas .eyebrow {
  margin: 0 0 .65rem;
  color: var(--mob-accent-strong);
  font-size: .76rem;
  font-weight: 750;
  letter-spacing: .12em;
}

.mob-atlas-hero h1 {
  margin: 0 0 .55rem;
  color: #20313d;
  font-size: clamp(2.15rem, 6vw, 3.65rem);
  font-weight: 720;
  letter-spacing: -.055em;
  line-height: 1.05;
}

.mob-atlas-hero .lead {
  max-width: 38rem;
  margin: 0;
  color: var(--mob-muted);
  font-size: 1rem;
  line-height: 1.75;
}

.mob-atlas-identity {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: .9rem 1.2rem;
  margin: 0;
}

.mob-atlas-identity div {
  padding-top: .75rem;
  border-top: 1px solid var(--mob-line);
}

.mob-atlas-identity dt {
  margin-bottom: .15rem;
  color: var(--mob-muted);
  font-size: .74rem;
}

.mob-atlas-identity dd {
  margin: 0;
  color: var(--mob-ink);
  font-size: .94rem;
  font-weight: 680;
}

.mob-atlas-directory {
  display: flex;
  align-items: center;
  gap: 1rem;
  margin: 0 0 2.7rem;
  padding: .85rem 1rem;
  border-left: 3px solid var(--mob-accent);
  background: var(--mob-accent-soft);
  border-radius: 0 12px 12px 0;
}

.mob-atlas-directory strong {
  flex: 0 0 auto;
  color: var(--mob-accent-strong);
  font-size: .84rem;
}

.mob-atlas-directory a {
  color: var(--mob-ink);
  font-size: .9rem;
  font-weight: 650;
  text-decoration: none;
}

.mob-atlas-directory a:hover { color: var(--mob-accent-strong); }

.mob-profile { scroll-margin-top: 1.5rem; }

.mob-profile-header {
  margin-bottom: 1.4rem;
  padding-bottom: 1rem;
  border-bottom: 1px solid var(--mob-line);
}

.mob-profile-header h2 {
  margin: 0 0 .4rem;
  color: var(--mob-ink);
  font-size: 1.65rem;
  font-weight: 700;
  letter-spacing: -.025em;
}

.mob-profile-header p {
  max-width: 44rem;
  margin: 0;
  color: var(--mob-muted);
  line-height: 1.7;
}

.mob-threat-summary {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: .7rem;
  margin: 0 0 2.6rem;
}

.mob-threat-summary div {
  min-height: 5.4rem;
  padding: .9rem;
  background: #fff;
  border: 1px solid var(--mob-line);
  border-radius: 12px;
}

.mob-threat-summary strong {
  display: block;
  margin-bottom: .3rem;
  color: var(--mob-accent-strong);
  font-size: .88rem;
}

.mob-threat-summary span {
  color: var(--mob-muted);
  font-size: .82rem;
  line-height: 1.5;
}

.mob-profile h3 {
  margin: 2.2rem 0 .45rem;
  color: var(--mob-ink);
  font-size: 1.28rem;
  font-weight: 700;
}

.mob-section-intro {
  max-width: 46rem;
  margin: 0 0 1.1rem !important;
  color: var(--mob-muted);
  line-height: 1.65;
}

.mob-skill-list {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: .85rem;
}

.mob-skill {
  padding: 1.1rem 1.15rem;
  background: #fff;
  border: 1px solid var(--mob-line);
  border-radius: 12px;
}

.mob-skill:last-child:nth-child(odd) { grid-column: 1 / -1; }

.mob-skill-heading {
  display: flex;
  flex-wrap: wrap;
  gap: .45rem .8rem;
  align-items: baseline;
  justify-content: space-between;
  margin-bottom: .65rem;
}

.mob-skill-heading h4 {
  margin: 0;
  color: var(--mob-ink);
  font-size: 1.05rem;
  font-weight: 720;
}

.mob-skill-heading span {
  color: var(--mob-accent-strong);
  font-size: .76rem;
  font-weight: 700;
}

.mob-skill p {
  margin: .35rem 0;
  color: #536273;
  font-size: .9rem;
  line-height: 1.65;
}

.mob-skill p strong { color: #314657; }

.mob-skill .counter {
  margin-top: .75rem;
  padding-top: .7rem;
  color: var(--mob-accent-strong);
  border-top: 1px solid var(--mob-line);
}

.mob-timing-note {
  margin: 1.2rem 0 0;
  padding: .9rem 1rem;
  color: #5d6c7b;
  background: var(--mob-surface);
  border: 1px solid var(--mob-line);
  border-radius: 12px;
  font-size: .86rem;
  line-height: 1.65;
}

.mob-timing-note strong { color: var(--mob-ink); }

@media (max-width: 760px) {
  .mob-atlas-hero { grid-template-columns: 1fr; }
  .mob-threat-summary { grid-template-columns: repeat(2, minmax(0, 1fr)); }
}

@media (max-width: 560px) {
  .mob-atlas-hero { padding: 1.2rem; }
  .mob-atlas-directory { align-items: flex-start; flex-direction: column; gap: .3rem; }
  .mob-skill-list { grid-template-columns: 1fr; }
  .mob-skill:last-child:nth-child(odd) { grid-column: auto; }
}

@media (prefers-reduced-motion: no-preference) {
  .mob-atlas-directory a,
  .mob-skill {
    transition: color .2s ease, border-color .2s ease, transform .2s ease;
  }

  .mob-skill:hover {
    border-color: #b9d4d3;
    transform: translateY(-2px);
  }
}
</style>

<div class="mob-atlas">
  <header class="mob-atlas-hero">
    <div>
      <p class="eyebrow">RAPIDS / 怪物档案</p>
      <h1>怪物信息</h1>
      <p class="lead">了解怪物的攻击方式、触发条件与应对方法。技能描述以当前服务器配置为准。</p>
    </div>
    <dl class="mob-atlas-identity">
      <div><dt>当前收录</dt><dd>1 个怪物</dd></div>
      <div><dt>资料区域</dt><dd>河隘</dd></div>
      <div><dt>信息范围</dt><dd>技能与机制</dd></div>
      <div><dt>更新时间</dt><dd>2026/07/15</dd></div>
    </dl>
  </header>

  <nav class="mob-atlas-directory" aria-label="怪物索引">
    <strong>怪物索引</strong>
    <a href="#/rapids/mobsinfo?id=河雾怨魄">河雾怨魄</a>
  </nav>

  ## 河雾怨魄
  <article class="mob-profile" id="河雾怨魄" style="--mob-accent:#348f8a;--mob-accent-strong:#256f6b;--mob-accent-soft:#e9f5f3">
    <header class="mob-profile-header">
    <p>河隘区域的 Essence 怪物。它擅长减速、贴近与聚拢玩家，距离过远或站位过密都会给它创造进攻机会。</p>
    </header>
    <div class="mob-threat-summary" aria-label="威胁概览">
      <div><strong>持续减速</strong><span>普攻和多数范围技能都会施加缓慢。</span></div>
      <div><strong>远距贴近</strong><span>目标离开 20 格后，它会尝试传送追击。</span></div>
      <div><strong>范围牵引</strong><span>12 格内的玩家可能被连续拉向怪物。</span></div>
      <div><strong>低血爆发</strong><span>生命低于 35% 后，受击会触发范围爆雾。</span></div>
    </div>
    <h3>技能详解</h3>
    <p class="mob-section-intro">伤害倍率以河雾怨魄自身的近战攻击为基准。范围均以怪物为中心计算。</p>
    <div class="mob-skill-list">
      <section class="mob-skill">
        <div class="mob-skill-heading"><h4>怨触</h4><span>近战命中时</span></div>
        <p><strong>效果：</strong>对当前目标造成一次 80% 近战倍率的技能伤害，并施加 2 秒缓慢 II。</p>
        <p class="counter"><strong>应对：</strong>不要与它长时间贴身换血。被命中后优先拉开，避免减速期间接上范围技能。</p>
      </section>
      <section class="mob-skill">
        <div class="mob-skill-heading"><h4>寒雾</h4><span>每 4 秒尝试 · 12 秒冷却</span></div>
        <p><strong>效果：</strong>6 格内的玩家受到 75% 近战倍率的技能伤害；其中 5 格内的玩家还会受到 3 秒缓慢 II。</p>
        <p class="counter"><strong>应对：</strong>看到水花与云雾扩散时立即离开近身范围。保持 6 格以上距离可避开伤害。</p>
      </section>
      <section class="mob-skill">
        <div class="mob-skill-heading"><h4>雾步</h4><span>每 6 秒检查 · 8 秒冷却</span></div>
        <p><strong>条件：</strong>当前目标不在 20 格以内时才会发动。</p>
        <p><strong>效果：</strong>传送到目标附近，落点会在水平方向产生最多约 2 格偏移。</p>
        <p class="counter"><strong>应对：</strong>远距离并不等于安全。它消失时及时转身确认落点，不要停在狭窄地形边缘。</p>
      </section>
      <section class="mob-skill">
        <div class="mob-skill-heading"><h4>回潮牵引</h4><span>每 8 秒尝试 · 10 秒冷却</span></div>
        <p><strong>条件：</strong>12 格内存在玩家时才会发动。</p>
        <p><strong>效果：</strong>将 12 格内玩家拉向自身，1.25 秒后再次牵引，并施加 2.5 秒缓慢 II。第二次牵引后，3 格内玩家还会受到 135% 近战倍率的技能伤害。</p>
        <p class="counter"><strong>应对：</strong>第一次位移后立刻向外移动。队伍应分散站位，避免同时被拖入 3 格伤害区。</p>
      </section>
      <section class="mob-skill">
        <div class="mob-skill-heading"><h4>濒死爆雾</h4><span>生命低于 35% · 20 秒冷却</span></div>
        <p><strong>触发：</strong>生命低于 35% 后，每次受击都有机会触发；触发后进入冷却。</p>
        <p><strong>效果：</strong>8 格内玩家受到 135% 近战倍率的技能伤害、2.5 秒失明 I，以及 3.5 秒缓慢 III。</p>
        <p class="counter"><strong>应对：</strong>进入低血阶段后预留位移手段。近战玩家不要集体抢攻，爆雾出现时先撤出 8 格范围。</p>
      </section>
    </div>
    <div class="mob-timing-note"><strong>计时说明：</strong>“每 X 秒尝试”代表怪物会按该频率检查一次技能；只有满足距离、目标与冷却条件时才会真正施放，因此实际间隔可能更长。</div>
  </article>
</div>
