<style>
.rapids-flow {
  max-width: 960px;
  color: #293241;
}

.rapids-flow-hero {
  margin: 1.2em 0 2.3em;
  padding: 1.7em 0 1.25em 1.5em;
  border-left: 2px solid #A0A2A4;
}

.rapids-flow-hero .kicker {
  margin: 0 0 .6em;
  color: #7b8799;
  font-size: .76em;
  font-weight: 700;
  letter-spacing: .16em;
}

.rapids-flow-hero h1 {
  margin: 0 0 .35em;
  color: #202b3c;
  font-size: 2.35em;
  font-weight: 650;
  letter-spacing: -.04em;
}

.rapids-flow-hero p {
  max-width: 38em;
  margin: 0;
  color: #748094;
  font-size: 1.04em;
  line-height: 1.75;
}

.rapids-flow-steps {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 0;
  margin: 0 0 2.5em;
  border-top: 1px solid #dce3ec;
  border-bottom: 1px solid #dce3ec;
}

.rapids-flow-step {
  min-height: 8.2em;
  padding: 1.15em 1.15em 1.1em;
  border-right: 1px solid #dce3ec;
}

.rapids-flow-step:last-child { border-right: 0; }

.rapids-flow-step .number {
  display: block;
  margin-bottom: 1em;
  color: #8da0bd;
  font-size: .74em;
  font-weight: 700;
  letter-spacing: .12em;
}

.rapids-flow-step strong {
  display: block;
  margin-bottom: .35em;
  color: #344b70;
  font-size: 1.05em;
}

.rapids-flow-step span {
  color: #7d8796;
  font-size: .88em;
  line-height: 1.55;
}

.rapids-flow-note {
  margin: 1.2em 0 2em;
  padding: .9em 1.1em;
  color: #59677c;
  background: #f5f7fa;
  border: 1px solid #e1e7ef;
  border-radius: 4px;
}

.rapids-flow-note strong { color: #344b70; }

.rapids-flow h2 {
  margin-top: 2.4em;
  padding-bottom: .45em;
  color: #283852;
  border-bottom: 1px solid #dce3ec;
  font-size: 1.45em;
  font-weight: 650;
  letter-spacing: -.02em;
}

.rapids-flow h3 {
  margin-top: 1.7em;
  color: #415a83;
  font-size: 1.08em;
}

.rapids-flow .flow-link {
  color: #4f70a5;
  font-weight: 600;
}

@media (max-width: 720px) {
  .rapids-flow-steps { grid-template-columns: repeat(2, minmax(0, 1fr)); }
  .rapids-flow-step:nth-child(2) { border-right: 0; }
  .rapids-flow-step:nth-child(-n+2) { border-bottom: 1px solid #dce3ec; }
}

@media (max-width: 460px) {
  .rapids-flow-steps { grid-template-columns: 1fr; }
  .rapids-flow-step,
  .rapids-flow-step:nth-child(2) { border-right: 0; border-bottom: 1px solid #dce3ec; }
  .rapids-flow-step:last-child { border-bottom: 0; }
}
</style>

<div class="rapids-flow">
  <div class="rapids-flow-hero">
    <p class="kicker">RAPIDS / PLAY LOOP</p>
    <h1>副本流程</h1>
    <p>一局副本的核心，是把探索、战斗与时间压缩成一次清晰的选择。</p>
  </div>

  <div class="rapids-flow-steps">
    <div class="rapids-flow-step"><span class="number">01 / ENTER</span><strong>进入</strong><span>从主城副本入口选择已解锁的内容。</span></div>
    <div class="rapids-flow-step"><span class="number">02 / RUN</span><strong>推进</strong><span>击杀、搜掠、采集，积累本局分数。</span></div>
    <div class="rapids-flow-step"><span class="number">03 / CLEAR</span><strong>结算</strong><span>达到目标后前往终点，查看本局评级。</span></div>
    <div class="rapids-flow-step"><span class="number">04 / CHOOSE</span><strong>选择</strong><span>消耗 AP 领取奖励，或再入、离开。</span></div>
  </div>

  <div class="rapids-flow-note"><strong>继续了解：</strong>前往 <a class="flow-link" href="#/rapids/dungeonlist">副本图鉴</a>查看每段回忆，或阅读<a class="flow-link" href="#/rapids/dungeonmechanics">副本机制</a>与<a class="flow-link" href="#/rapids/materials">材料图鉴</a>。</div>

  ## 如何开始

  <p>在主城进入界域传送门，选择副本与难度。所有副本难度使用统一的回忆进度解锁规则：</p>

  <ol>
    <li>进入当前已经开放的副本内容。</li>
    <li>通过击杀怪物、搜掠宝箱和收集采集物推进后续回忆。</li>
    <li>对应回忆完成后，下一段内容解锁。</li>
    <li>进入时仍需满足界面显示的等级门槛。</li>
  </ol>

  ## 副本流程

  <p>进入副本后立即开始计时。先完成基础目标，再用探索和特殊目标提高评级：</p>

  <ol>
    <li><strong>击杀至少 36 个对应怪物。</strong> 这是正常提交本局结果的基础目标。</li>
    <li><strong>搜掠地图。</strong> 宝箱与采集物既提供材料，也会提供固定分数。</li>
    <li><strong>追求速度。</strong> 击杀速度会影响击杀部分的分数。</li>
    <li><strong>挑战 Essence。</strong> Essence 怪物会随副本刷新系统自然出现，是争取 Tier 6 的必要目标；部分地图还设有消耗材料召唤的历史回响。具体机制见<a class="flow-link" href="#/rapids/dungeonmechanics">副本机制</a>。</li>
    <li><strong>前往终点。</strong> 与出口交互，提交本局结果。</li>
  </ol>

  <div class="rapids-flow-note"><strong>组队提示：</strong> 12 格内共享经验；对怪物造成超过 10% 的伤害，通常即可获得完整击杀判定。即使中途死亡，已经获得的共享击杀奖励仍会保留在个人记录中。</div>

  ### Tier 评级

  <p>评级同时看总分与时间。击杀、速度、宝箱、采集物和特殊目标共同构成分数。</p>

  | Tier | 评级 | 主要达成条件 |
  | --- | --- | --- |
  | 1 | Common | 达到基础通关要求 |
  | 2 | Unusual | 总分超过 60 |
  | 3 | Remarkable | 总分超过 90 |
  | 4 | Extraordinary | 总分超过 120，且用时不超过 400 秒 |
  | 5 | Unparalleled | 总分超过 160，且用时不超过 480 秒 |
  | 6 | Marvelous | 总分超过 192、用时不超过 400 秒，并击杀 Essence 特殊怪 |

  ## 完成后：在等待室做出选择

  <p>提交结果后会进入等待室。点击「领取奖励」打开结算界面；每次领取额外奖励消耗 10 AP。</p>

  | 选择 | 你会得到什么 |
  | --- | --- |
  | 随机装备 | 当前副本等级范围内的随机装备；Tier 越高，额外装备越多，Tier 6 另有高品质装备 |
  | 随机材料 | 当前副本材料；更高 Tier 有机会获得更好的材料、稀有材料或图纸 |
  | 回忆点数 | 用于局外兑换装备、材料和升级副本天赋 |
  | 再入 | 选择随机战斗增益，返回同一副本继续挑战；当前仍属于调整中的功能 |
  | 直接离开 | 不领取额外奖励，回到主城 |

  <p>默认 AP 上限为 200，通常每 8 分钟恢复 1 点。拥有相应 Rank 特权并满足等级要求时，可以进行 2 倍、3 倍或 4 倍领取，分别消耗 20、30、40 AP。材料与装备的具体来源，见<a class="flow-link" href="#/rapids/materials">材料图鉴</a>。</p>

  ## 中断与失败

  <ul>
    <li><strong>死亡：</strong>拥有可用的「死亡回溯」时，会回到副本起点继续本局；回溯次数耗尽后会回到主城，死亡还会扣除部分本局分数。</li>
    <li><strong>断线：</strong>短时间内重新登录会尝试回到原副本；超过约 60 秒，暂存状态会失效。</li>
    <li><strong>未达目标：</strong>击杀数未达到基础目标时，终点不会完成结算，需要继续探索。</li>
  </ul>

  <div class="rapids-flow-note"><strong>推荐记法：</strong> 进入 → 击杀与搜掠 → 争取 Tier → 终点结算 → 选择奖励。副本的完整信息与每段叙事，统一收录在<a class="flow-link" href="#/rapids/dungeonlist">副本图鉴</a>；刷新、掉落和多人规则集中在<a class="flow-link" href="#/rapids/dungeonmechanics">副本机制</a>。</div>
</div>
