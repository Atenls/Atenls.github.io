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

.mob-profile:not(:first-of-type) {
}

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
  max-width: 60rem;
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
  max-width: 60rem;
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
      <div><dt>当前收录</dt><dd>3 个怪物</dd></div>
      <div><dt>资料区域</dt><dd>河隘</dd></div>
      <div><dt>信息范围</dt><dd>技能与机制</dd></div>
      <div><dt>更新时间</dt><dd>2026/07/15</dd></div>
    </dl>
  </header>
  <nav class="mob-atlas-directory" aria-label="怪物索引">
    <strong>怪物索引</strong>
    <a href="#/rapids/mobsinfo?id=河雾怨魄">河雾怨魄</a>
    <a href="#/rapids/mobsinfo?id=洞渊渡者">洞渊渡者</a>
    <a href="#/rapids/mobsinfo?id=晦渊司祭">晦渊司祭</a>
  </nav>

  ## 河雾怨魂
  <article class="mob-profile" style="--mob-accent:#348f8a;--mob-accent-strong:#256f6b;--mob-accent-soft:#e9f5f3">
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

  ## 洞渊渡者
  <article class="mob-profile">
    <header class="mob-profile-header">
      <p>河隘区域的近战 Final 怪物。它会在短暂预警后连续冲刺，并在每段攻击前重新锁定目标，单次闪避不能解除后续威胁。</p>
    </header>
    <div class="mob-threat-summary" aria-label="威胁概览">
      <div><strong>连续突进</strong><span>主要技能由多段位移和范围近战伤害组成。</span></div>
      <div><strong>重复锁定</strong><span>连段中会再次转向当前目标，需要持续移动。</span></div>
      <div><strong>落点预警</strong><span>水环和标题提示会提前标出高伤攻击。</span></div>
      <div><strong>高伤收尾</strong><span>多数连段的最后一击范围更大、倍率更高。</span></div>
    </div>
    <h3>技能轮换</h3>
    <p class="mob-section-intro">每 5 秒尝试从三个主技能中选择一个。逐浪三渡、逆潮升袭、沉渊落潮的选择权重为 4:3:1，各技能仍受自身冷却限制。</p>
    <div class="mob-skill-list">
      <section class="mob-skill">
        <div class="mob-skill-heading"><h4>潮刃</h4><span>近战命中时</span></div>
        <p><strong>效果：</strong>对当前目标造成一次 100% 近战倍率的技能伤害，并产生水花效果。</p>
        <p class="counter"><strong>应对：</strong>这是它的常规近战攻击。保持移动和基础防御，不要为了等待主技能而忽略普攻。</p>
      </section>
      <section class="mob-skill">
        <div class="mob-skill-heading"><h4>逐浪三渡</h4><span>权重 4 · 10 秒冷却</span></div>
        <p><strong>预警：</strong>怪物停止行动，朝目标转向，并显示技能标题；水泡会逐渐向自身聚集。</p>
        <p><strong>效果：</strong>连续发动三次冲刺，每次都会重新锁定目标。前两击影响 4 格范围，分别造成 100% 与 120% 近战倍率伤害；最后一击扩大至 5 格，造成 160% 伤害。</p>
        <p class="counter"><strong>应对：</strong>横向移动并为第三击保留位移。躲过第一击后不要停下，它会再次转向。</p>
      </section>
      <section class="mob-skill">
        <div class="mob-skill-heading"><h4>逆潮升袭</h4><span>权重 3 · 12 秒冷却</span></div>
        <p><strong>预警：</strong>目标脚下出现约 2.6 格水环，随后怪物向上跃起。</p>
        <p><strong>效果：</strong>先从空中穿刺，命中 5 格内玩家并造成 125% 近战倍率伤害；短暂停顿并重新锁定后，再次俯冲，对 6 格内玩家造成 150% 伤害。</p>
        <p class="counter"><strong>应对：</strong>离开最初水环后继续改变方向。第二次俯冲会重新瞄准，提前停步容易被追上。</p>
      </section>
      <section class="mob-skill">
        <div class="mob-skill-heading"><h4>沉渊落潮</h4><span>权重 1 · 18 秒冷却</span></div>
        <p><strong>预警：</strong>屏幕出现高危提示，怪物身边依次扩散 2、4、6 格水环；升空后还会在目标位置显示约 3.8 格落点。</p>
        <p><strong>效果：</strong>锁定目标后高速坠落，对落地时 6 格内的玩家造成 200% 近战倍率伤害，并将玩家轻微震开。</p>
        <p class="counter"><strong>应对：</strong>这是最危险但前摇最长的技能。看到高危标题后拉开，落点水环出现时立即向圈外移动。</p>
      </section>
    </div>
    <div class="mob-timing-note"><strong>轮换说明：</strong>权重表示被随机选中的相对机会，不代表固定施放顺序。技能处于冷却或条件不满足时，实际施放间隔会延长。</div>
  </article>

  ## 晦渊司祭
  <article class="mob-profile">
    <header class="mob-profile-header">
      <p>河隘区域的远程 Final 怪物。它以魔法伤害封锁地面和追赶目标，玩家靠近时还会自动发动范围驱离。</p>
    </header>
    <div class="mob-threat-summary" aria-label="威胁概览">
      <div><strong>自动拒近</strong><span>玩家进入近身范围后会受到伤害和强力击退。</span></div>
      <div><strong>延迟落点</strong><span>连续记录目标位置，稍后引爆多个法阵。</span></div>
      <div><strong>追踪飞弹</strong><span>带明显点名提示，单靠直线后退难以摆脱。</span></div>
      <div><strong>分圈暗潮</strong><span>伤害从内圈依次扩散至 16 格外圈。</span></div>
    </div>
    <h3>技能轮换</h3>
    <p class="mob-section-intro">每 5.5 秒尝试从三个主技能中选择一个。黯星连坠、黯蚀追魂、渊门逐浪的选择权重为 4:3:1，各技能仍受自身冷却限制。</p>
    <div class="mob-skill-list">
      <section class="mob-skill">
        <div class="mob-skill-heading"><h4>黯触</h4><span>近战命中时</span></div>
        <p><strong>效果：</strong>对当前目标造成一次 90% 魔法倍率的技能伤害。</p>
        <p class="counter"><strong>应对：</strong>司祭并非没有近战能力。被逼到它身边时尽快撤离，避免同时触发驱离技能。</p>
      </section>
      <section class="mob-skill">
        <div class="mob-skill-heading"><h4>近身驱离</h4><span>每 1 秒检查 · 3 秒冷却</span></div>
        <p><strong>条件：</strong>5 格内存在玩家时发动，并经过约 0.4 秒烟雾预警。</p>
        <p><strong>效果：</strong>对 6 格内玩家造成 80% 魔法倍率伤害，并施加强力向外击退。</p>
        <p class="counter"><strong>应对：</strong>近战玩家采用短进短出，不要持续贴身。看到环形烟雾时立即后撤。</p>
      </section>
      <section class="mob-skill">
        <div class="mob-skill-heading"><h4>黯星连坠</h4><span>权重 4 · 10 秒冷却</span></div>
        <p><strong>预警：</strong>技能标题出现后，司祭连续三次记录目标当时的位置，每次间隔 0.5 秒；落点会先后出现暗色法阵。</p>
        <p><strong>效果：</strong>每个法阵在完成两段预警后爆炸，对落点 3.2 格内玩家造成 135% 魔法倍率伤害并向外震开。</p>
        <p class="counter"><strong>应对：</strong>保持连续移动，不要在第一个法阵出现后折返原路。三个落点记录的是不同时间的位置。</p>
      </section>
      <section class="mob-skill">
        <div class="mob-skill-heading"><h4>黯蚀追魂</h4><span>权重 3 · 10 秒冷却</span></div>
        <p><strong>预警：</strong>被选中的目标脚下出现紫色环并听到尖啸，约 0.8 秒后发射追踪飞弹。</p>
        <p><strong>效果：</strong>飞弹最多追踪约 3.5 秒，最远飞行 40 格。命中时造成 80% 魔法倍率伤害，并产生轻微位移。</p>
        <p class="counter"><strong>应对：</strong>被点名者利用转角、障碍物和持续变向拖过追踪时间，其他玩家让出移动路线。</p>
      </section>
      <section class="mob-skill">
        <div class="mob-skill-heading"><h4>渊门逐浪</h4><span>权重 1 · 18 秒冷却</span></div>
        <p><strong>预警：</strong>司祭停止移动，暗潮由内向外分三圈扩散。每一圈伤害前都会先显示对应半径的粒子环。</p>
        <p><strong>效果：</strong>先攻击 0-4 格内圈，造成 100% 魔法倍率伤害；随后攻击 4-8 格中圈，造成 150% 伤害；最后攻击 8-16 格外圈，造成 200% 伤害。每圈都会附带轻度向外击退。</p>
        <p class="counter"><strong>应对：</strong>不要盲目向外跑。观察当前预警圈并跨到已经爆发过的区域；空间充足时，直接离开 16 格范围最安全。</p>
      </section>
    </div>
    <div class="mob-timing-note"><strong>伤害说明：</strong>晦渊司祭的技能使用魔法攻击倍率，魔法抗性会影响实际承伤。权重只描述随机选择机会，不代表固定顺序。</div>
  </article>
</div>
