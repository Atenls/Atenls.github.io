<style>
.attribute-guide {
  --attr-ink: #24343f;
  --attr-muted: #647580;
  --attr-line: #dce5ea;
  --attr-surface: #f7fafb;
  --attr-accent: #4777a3;
  --attr-accent-soft: #edf4f9;
  width: 100%;
  min-width: 0;
  color: var(--attr-ink);
}

.attribute-guide * { box-sizing: border-box; }

.attribute-hero {
  display: grid;
  grid-template-columns: minmax(0, 1.5fr) minmax(15rem, .7fr);
  gap: 1rem;
  margin: .8rem 0 1.6rem;
  padding: 1.5rem;
  background: var(--attr-surface);
  border: 1px solid var(--attr-line);
  border-radius: 14px;
}

.attribute-hero h1 {
  margin: 0 0 .65rem;
  color: var(--attr-ink);
  font-size: clamp(2rem, 6vw, 3.35rem);
  font-weight: 730;
  letter-spacing: -.055em;
  line-height: 1.05;
}

.attribute-hero p {
  max-width: 42rem;
  margin: 0;
  color: var(--attr-muted);
  line-height: 1.75;
}

.attribute-baseline {
  align-self: end;
  margin: 0;
  padding: .85rem 1rem;
  background: #fff;
  border: 1px solid var(--attr-line);
  border-radius: 10px;
}

.attribute-baseline div + div { margin-top: .7rem; }

.attribute-baseline dt {
  color: var(--attr-muted);
  font-size: .75rem;
  font-weight: 700;
  letter-spacing: .06em;
}

.attribute-baseline dd {
  margin: .16rem 0 0;
  color: var(--attr-ink);
  font-size: .92rem;
  font-weight: 650;
}

.attribute-nav {
  display: flex;
  flex-wrap: wrap;
  gap: .45rem;
  margin: 0 0 2.2rem;
}

.attribute-nav a {
  padding: .42rem .7rem;
  color: var(--attr-accent);
  background: #fff;
  border: 1px solid var(--attr-line);
  border-radius: 8px;
  font-size: .82rem;
  font-weight: 650;
  text-decoration: none;
}

.attribute-guide section { scroll-margin-top: 1.5rem; }

.attribute-guide h2 {
  margin: 2.7rem 0 .45rem;
  color: var(--attr-ink);
  font-size: 1.45rem;
  letter-spacing: -.025em;
}

.attribute-guide h3 {
  margin: 1.6rem 0 .65rem;
  color: #334a59;
  font-size: 1.04rem;
}

.attribute-intro {
  max-width: 46rem;
  margin: 0 0 1rem;
  color: var(--attr-muted);
  line-height: 1.7;
}

.damage-route {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: .55rem;
  margin: 1rem 0;
  padding: 0;
  list-style: none;
  counter-reset: route;
}

.damage-route li {
  position: relative;
  min-height: 6.2rem;
  padding: .85rem;
  background: var(--attr-surface);
  border: 1px solid var(--attr-line);
  border-radius: 10px;
  counter-increment: route;
}

.damage-route li::before {
  content: counter(route, decimal-leading-zero);
  display: block;
  margin-bottom: .35rem;
  color: var(--attr-accent);
  font-size: .72rem;
  font-weight: 750;
  letter-spacing: .08em;
}

.damage-route strong { display: block; margin-bottom: .25rem; }
.damage-route span { color: var(--attr-muted); font-size: .82rem; line-height: 1.5; }

.formula-list {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: .7rem;
  margin: 1rem 0;
}

.formula-card {
  min-width: 0;
  padding: 1rem;
  background: #fff;
  border: 1px solid var(--attr-line);
  border-radius: 10px;
}

.formula-card.wide { grid-column: 1 / -1; }

.formula-card h3 { margin: 0 0 .45rem; }

.formula-card code {
  display: block;
  overflow-x: auto;
  margin: .55rem 0;
  padding: .65rem .75rem;
  color: #315a7c;
  background: var(--attr-accent-soft);
  border-radius: 7px;
  font-size: .79rem;
  line-height: 1.55;
  white-space: nowrap;
}

.formula-card p {
  margin: .4rem 0 0;
  color: var(--attr-muted);
  font-size: .85rem;
  line-height: 1.6;
}

.attribute-group {
  margin: 1rem 0;
  padding: 1rem 1.1rem;
  background: var(--attr-surface);
  border: 1px solid var(--attr-line);
  border-radius: 12px;
}

.attribute-group h3 { margin: 0 0 .8rem; }

.attribute-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 0 1.4rem;
  margin: 0;
}

.attribute-grid div {
  display: grid;
  grid-template-columns: minmax(7.5rem, .72fr) minmax(0, 1.28fr);
  gap: .65rem;
  padding: .62rem 0;
  border-top: 1px solid var(--attr-line);
}

.attribute-grid div:nth-child(-n + 2) { border-top: 0; }

.attribute-grid dt {
  color: #344d5d;
  font-size: .86rem;
  font-weight: 700;
}

.attribute-grid dd {
  margin: 0;
  color: var(--attr-muted);
  font-size: .84rem;
  line-height: 1.55;
}

.element-strip {
  display: grid;
  grid-template-columns: repeat(6, minmax(0, 1fr));
  gap: .45rem;
  margin: .85rem 0 1rem;
}

.element-strip span {
  padding: .55rem .35rem;
  color: #344550;
  background: #fff;
  border: 1px solid var(--element, var(--attr-line));
  border-radius: 8px;
  font-size: .82rem;
  font-weight: 700;
  text-align: center;
}

.attribute-note {
  margin: 1rem 0;
  padding: .85rem 1rem;
  color: #4f626e;
  background: var(--attr-accent-soft);
  border-left: 3px solid var(--attr-accent);
  border-radius: 0 9px 9px 0;
  font-size: .86rem;
  line-height: 1.65;
}

.attribute-note strong { color: var(--attr-ink); }

@media (max-width: 820px) {
  .damage-route { grid-template-columns: repeat(2, minmax(0, 1fr)); }
  .element-strip { grid-template-columns: repeat(3, minmax(0, 1fr)); }
}

@media (max-width: 640px) {
  .attribute-hero { grid-template-columns: 1fr; padding: 1.15rem; }
  .formula-list,
  .attribute-grid { grid-template-columns: 1fr; }
  .attribute-grid div { grid-template-columns: minmax(6.7rem, .72fr) minmax(0, 1.28fr); }
  .attribute-grid div:nth-child(2) { border-top: 1px solid var(--attr-line); }
}

@media (max-width: 420px) {
  .damage-route { grid-template-columns: 1fr; }
  .damage-route li { min-height: auto; }
  .element-strip { grid-template-columns: repeat(2, minmax(0, 1fr)); }
}

@media (prefers-reduced-motion: no-preference) {
  .attribute-nav a { transition: color .18s ease, border-color .18s ease, background .18s ease; }
  .attribute-nav a:hover { color: #315b7e; background: var(--attr-accent-soft); border-color: #b9cedd; }
}
</style>

<main class="attribute-guide">
  <header class="attribute-hero">
    <div>
      <h1>属性介绍</h1>
      <p>属性决定角色的生存、输出、行动效率与元素克制。本文按当前战斗实现说明每项属性的用途，并给出真正参与结算的公式与顺序。</p>
    </div>
    <dl class="attribute-baseline">
      <div><dt>面板入口</dt><dd>主菜单 → 个人属性</dd></div>
      <div><dt>数值口径</dt><dd>固定值直接相加，百分比按标注参与乘算</dd></div>
      <div><dt>时间单位</dt><dd>20 ticks = 1 秒</dd></div>
    </dl>
  </header>

  <nav class="attribute-nav" aria-label="属性介绍目录">
    <a href="#/rapids/attributes?id=伤害如何结算">伤害结算</a>
    <a href="#/rapids/attributes?id=核心公式">核心公式</a>
    <a href="#/rapids/attributes?id=生存与通用">生存与通用</a>
    <a href="#/rapids/attributes?id=物理与箭矢">物理与箭矢</a>
    <a href="#/rapids/attributes?id=魔法与法力">魔法与法力</a>
    <a href="#/rapids/attributes?id=元素属性">元素属性</a>
    <a href="#/rapids/attributes?id=持续伤害">持续伤害</a>
  </nav>

  <section id="伤害如何结算">
    <h2>伤害如何结算</h2>
    <p class="attribute-intro">一次常规攻击会依次经过基础伤害、元素、暴击与防御，最后才应用全局修正、灵魂攻击和单次承伤上限。</p>
    <ol class="damage-route">
      <li><strong>生成基础伤害</strong><span>在攻击下限与上限间随机，并乘对应攻击增幅。</span></li>
      <li><strong>判断攻击结果</strong><span>近战与箭矢检查命中、闪避和暴击。魔法不经过这一步。</span></li>
      <li><strong>处理元素与防御</strong><span>先计算元素强化与抗性，再由护甲或魔抗减伤。</span></li>
      <li><strong>应用最终修正</strong><span>全系加成后追加灵魂攻击，再处理副本调配与承伤上限。</span></li>
    </ol>
    <div class="attribute-note"><strong>简化总式：</strong>常规部分 = 随机基础伤害 × 攻击增幅 × 元素倍率 × 暴击倍率 × 防御倍率 × 全系倍率。随后追加灵魂攻击，再乘副本伤害与承伤调配，最后检查最大受击伤害。</div>
  </section>

  <section id="核心公式">
    <h2>核心公式</h2>
    <p class="attribute-intro">以下公式中的等级均取受击方等级。所有概率最终都会限制在标明的区间内。</p>
    <div class="formula-list">
      <article class="formula-card">
        <h3>命中率</h3>
        <code>命中率 = 1 - 闪避 ÷ (命中 + 1.5 × 闪避 + 12 × 等级系数)</code>
        <p>等级系数 = 等级 × 1.0375<sup>等级</sup> + 10。最终命中率最低 50%，最高 100%。仅近战与箭矢使用。</p>
      </article>
      <article class="formula-card">
        <h3>暴击率</h3>
        <code>暴击率 = 0.75 × 会心 ÷ (会心 + 柔韧 + 16 × 等级系数)</code>
        <p>最终暴击率限制在 0% 至 75%。暴击伤害倍率 = 1 + max(0, 暴击伤害 - 暴击减免) ÷ 100。</p>
      </article>
      <article class="formula-card">
        <h3>护甲与魔抗</h3>
        <code>有效防御 = 防御 × (1 - 百分比穿透 ÷ 100) - 固定穿透</code>
        <code>减伤率 = 有效防御 ÷ (有效防御 + 8 × 等级系数)</code>
        <p>百分比穿透先算，固定穿透后算。有效防御不大于 0 时，减伤率为 0。物理与箭矢使用护甲，魔法使用魔法抗性。</p>
      </article>
      <article class="formula-card">
        <h3>元素倍率</h3>
        <code>元素倍率 = 1 + (属性强化 - 属性抗性) ÷ (1000 + 属性抗性)</code>
        <p>只有攻击携带对应元素时才结算。抗性越高，继续堆叠强化所获得的相对收益越平缓。</p>
      </article>
      <article class="formula-card">
        <h3>基础攻击与期望 DPS</h3>
        <code>平均攻击 = (攻击下限 + 攻击上限) ÷ 2 × (1 + 攻击增幅 ÷ 100)</code>
        <code>面板 DPS = 平均攻击 × 每秒攻击次数</code>
        <p>近战与箭矢使用攻击速度，魔法使用施法速度。面板期望不包含命中、暴击、目标防御、元素克制与灵魂攻击。</p>
      </article>
      <article class="formula-card">
        <h3>最终修正与承伤上限</h3>
        <code>阶段伤害 = 常规伤害 × (1 + 全系伤害加成 ÷ 100) + 灵魂攻击</code>
        <code>结算伤害 = min(最大受击伤害, 阶段伤害 × 副本伤害倍率 × 副本承伤倍率)</code>
        <p>最大受击伤害为 0 时不设上限。灵魂攻击是固定追加值，不经过护甲、魔抗、元素和全系伤害加成。</p>
      </article>
      <article class="formula-card wide">
        <h3>生命偷取</h3>
        <code>恢复量 = min(本次结算伤害, 目标最大生命) × 生命偷取 ÷ 100</code>
        <p>单次恢复最多为自身最大生命的 50%。基础触发间隔为 4 秒，生命偷取间隔按百分比修正：实际间隔 = 4 秒 × (1 + 间隔修正 ÷ 100)。</p>
      </article>
    </div>
  </section>

  <section id="生存与通用">
    <h2>生存与通用</h2>
    <div class="attribute-group">
      <dl class="attribute-grid">
        <div><dt>最大生命</dt><dd>角色可拥有的生命上限。最终生命 = 固定生命总和 × (1 + 生命百分比 ÷ 100)。</dd></div>
        <div><dt>生命恢复</dt><dd>每秒恢复的生命点数，不能超过最大生命。</dd></div>
        <div><dt>生命偷取</dt><dd>按本次有效伤害的一定比例恢复生命，并受触发间隔与单次恢复上限约束。</dd></div>
        <div><dt>生命偷取间隔</dt><dd>对基础 4 秒间隔作百分比修正。负值缩短间隔，最低可降至 0。</dd></div>
        <div><dt>移动速度</dt><dd>相对基础移动速度的百分比变化。面板显示为 100% 加该属性，最高增幅限制为 400%。</dd></div>
        <div><dt>最大受击伤害</dt><dd>限制单次属性伤害的最终值。数值为 0 时不启用限制。</dd></div>
        <div><dt>全系伤害加成</dt><dd>在元素、暴击与常规防御结算后，提高近战、箭矢和魔法的常规伤害。</dd></div>
        <div><dt>灵魂攻击</dt><dd>全系伤害加成结算后追加的固定伤害，不经过元素、暴击、护甲和魔抗。</dd></div>
        <div><dt>额外经验</dt><dd>先在基础经验上增加固定值，再乘百分比增幅：round((基础经验 + 固定值) × (1 + 百分比 ÷ 100))。</dd></div>
        <div><dt>自然馈赠</dt><dd>传递给战利品结算的幸运值。个人属性面板同时以 自然馈赠 ÷ 200 显示倍率参考。</dd></div>
      </dl>
    </div>
  </section>

  <section id="物理与箭矢">
    <h2>物理与箭矢</h2>
    <div class="attribute-group">
      <h3>输出与行动</h3>
      <dl class="attribute-grid">
        <div><dt>近战攻击</dt><dd>近战的伤害下限与上限，可再叠加近战攻击百分比增幅。</dd></div>
        <div><dt>箭矢攻击</dt><dd>箭矢的伤害下限与上限，可再叠加箭矢攻击百分比增幅。</dd></div>
        <div><dt>攻击速度</dt><dd>每秒可执行的近战或箭矢攻击次数。攻击间隔 = 1 ÷ 攻击速度 秒。</dd></div>
        <div><dt>投掷伤害增幅</dt><dd>以近战攻击为基础，提高长矛等投掷攻击的伤害。</dd></div>
        <div><dt>重击伤害增幅</dt><dd>以近战攻击为基础，提高钉头锤下落重击的伤害。</dd></div>
        <div><dt>近战攻击范围</dt><dd>范围 = (基础范围 + 固定范围) × (1 + 范围百分比 ÷ 100)，最低 1.5 格。</dd></div>
        <div><dt>近战攻击目标数</dt><dd>目标数 = floor((基础目标数 + 固定目标数) × (1 + 目标数百分比 ÷ 100))，最低 1 个。</dd></div>
        <div><dt>箭矢速度</dt><dd>箭速 = 1.5 × (1 + 箭矢速度 ÷ 100)，同时影响箭矢抵达目标所需时间。</dd></div>
        <div><dt>箭矢穿透</dt><dd>箭矢命中后可继续攻击射线上的其他目标。取四舍五入后的整数，范围 0 至 127。</dd></div>
        <div><dt>箭矢存活时间</dt><dd>箭矢最多存在的 ticks 数，取四舍五入后的整数，最低 1 tick。</dd></div>
      </dl>
    </div>
    <div class="attribute-group">
      <h3>命中、暴击与防御</h3>
      <dl class="attribute-grid">
        <div><dt>命中</dt><dd>对抗目标闪避，提高近战和箭矢攻击成功命中的概率。</dd></div>
        <div><dt>闪避</dt><dd>对抗攻击者命中，降低近战和箭矢攻击成功命中的概率。</dd></div>
        <div><dt>会心</dt><dd>对抗目标柔韧，提高近战和箭矢的暴击概率。</dd></div>
        <div><dt>柔韧</dt><dd>对抗攻击者会心，降低受到近战和箭矢暴击的概率。</dd></div>
        <div><dt>暴击伤害</dt><dd>暴击时增加的伤害百分比，先扣除目标的暴击减免。</dd></div>
        <div><dt>暴击减免</dt><dd>直接抵消攻击者的暴击伤害，最低只会将额外暴击伤害降至 0。</dd></div>
        <div><dt>护甲</dt><dd>降低近战与箭矢伤害。收益随数值提高逐渐平缓。</dd></div>
        <div><dt>护甲穿透</dt><dd>先按百分比削减目标护甲，再扣除固定穿透值。</dd></div>
      </dl>
    </div>
  </section>

  <section id="魔法与法力">
    <h2>魔法与法力</h2>
    <div class="attribute-group">
      <dl class="attribute-grid">
        <div><dt>魔法攻击</dt><dd>魔法的伤害下限与上限，可再叠加魔法攻击百分比增幅。</dd></div>
        <div><dt>魔法抗性</dt><dd>降低魔法伤害，使用与护甲相同的减伤曲线。</dd></div>
        <div><dt>魔法穿透</dt><dd>先按百分比削减目标魔抗，再扣除固定穿透值。</dd></div>
        <div><dt>施法速度</dt><dd>每秒可施放的魔法次数。实际计算时最低按 0.05 次/秒处理。</dd></div>
        <div><dt>法力上限</dt><dd>角色可储存的法力最大值。</dd></div>
        <div><dt>法力恢复</dt><dd>每秒恢复的法力点数，不能超过法力上限。</dd></div>
        <div><dt>法力消耗</dt><dd>每次施法需要支付的法力。当前法力不足时不能施法。</dd></div>
        <div><dt>法球伤害半径</dt><dd>魔法投射物命中检测的半径，最低按 0.01 格处理。</dd></div>
        <div><dt>法球飞行速度</dt><dd>每 tick 前进的格数，最低 0.01，并受系统速度上限限制。</dd></div>
        <div><dt>法球飞行距离</dt><dd>法球最多飞行的距离，并受系统最大距离限制。</dd></div>
      </dl>
    </div>
    <div class="attribute-note"><strong>魔法结算差异：</strong>当前魔法攻击不会检查命中、闪避、会心、柔韧、暴击伤害与暴击减免。它仍会结算元素属性、魔法抗性、魔法穿透、全系加成、灵魂攻击和最终承伤限制。</div>
  </section>

  <section id="元素属性">
    <h2>元素属性</h2>
    <p class="attribute-intro">攻击可携带一种元素。对应强化提高该次伤害，目标的同元素抗性会抵消强化。无属性攻击不使用元素倍率。</p>
    <div class="element-strip" aria-label="六种元素">
      <span style="--element:#d9c449">光</span>
      <span style="--element:#8d5aa8">暗</span>
      <span style="--element:#65b8ca">冰</span>
      <span style="--element:#d36c64">火</span>
      <span style="--element:#73985d">地</span>
      <span style="--element:#668fc0">雷</span>
    </div>
    <div class="attribute-group">
      <dl class="attribute-grid">
        <div><dt>六系属性强化</dt><dd>光、暗、冰、火、地、雷各自独立，只提高同元素攻击。</dd></div>
        <div><dt>六系属性抗性</dt><dd>光、暗、冰、火、地、雷各自独立，只抵抗同元素攻击。</dd></div>
        <div><dt>全属性强化</dt><dd>同时加入六种属性强化，等同于六系分别获得相同数值。</dd></div>
        <div><dt>全属性抗性</dt><dd>同时加入六种属性抗性，等同于六系分别获得相同数值。</dd></div>
      </dl>
    </div>
  </section>

  <section id="持续伤害">
    <h2>持续伤害</h2>
    <p class="attribute-intro">燃烧、中毒等持续效果会在施加时记录伤害、间隔与持续时间。是否启用某项修正由该持续效果自身定义。</p>
    <div class="attribute-group">
      <dl class="attribute-grid">
        <div><dt>持续伤害加成</dt><dd>每跳伤害 × (1 + 持续伤害加成 ÷ 100)。</dd></div>
        <div><dt>持续伤害加速</dt><dd>间隔 = round(基础间隔 ÷ (1 + max(0, 加速) ÷ 100))，并受系统最短间隔限制。</dd></div>
        <div><dt>持续时间加成</dt><dd>持续时间 = round(基础时长 × (1 + 持续时间加成 ÷ 100))，且至少覆盖一个触发间隔。</dd></div>
        <div><dt>持续承伤调配</dt><dd>目标每跳承伤 × (1 + 持续承伤调配 ÷ 100)。负值降低承伤，正值提高承伤。</dd></div>
      </dl>
    </div>
    <div class="attribute-note"><strong>系统调配属性：</strong>副本系统伤害调配、副本系统承伤调配与持续承伤调配主要用于副本、怪物或特殊效果的平衡控制。它们参与最终乘算，但通常不是常规装备的主要构筑目标。</div>
  </section>
</main>
