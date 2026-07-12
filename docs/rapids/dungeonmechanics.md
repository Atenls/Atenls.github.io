<style>
.rapids-mechanics {
  max-width: 960px;
  color: #293241;
}

.rapids-mechanics-hero {
  margin: 1.2em 0 2.3em;
  padding: 1.7em 0 1.25em 1.5em;
  border-left: 3px solid #8090e0;
}

.rapids-mechanics-hero .kicker,
.rapids-mechanics .eyebrow {
  margin: 0 0 .6em;
  color: #7b8799;
  font-size: .76em;
  font-weight: 700;
  letter-spacing: .16em;
}

.rapids-mechanics-hero h1 {
  margin: 0 0 .35em;
  color: #202b3c;
  font-size: 2.35em;
  font-weight: 650;
  letter-spacing: -.04em;
}

.rapids-mechanics-hero p {
  max-width: 46em;
  margin: 0;
  color: #748094;
  font-size: 1.04em;
}

.rapids-mechanics .quick-links {
  display: flex;
  flex-wrap: wrap;
  gap: .55em 1.4em;
  margin: -1em 0 2.3em;
  color: #6f7b8d;
  font-size: .9em;
}

.rapids-mechanics a {
  color: #4f70a5;
  font-weight: 600;
}

.rapids-mechanics h2 {
  margin: 2.7em 0 1em;
  padding-bottom: .45em;
  color: #283852;
  border-bottom: 1px solid #dce3ec;
  font-size: 1.45em;
  font-weight: 650;
  letter-spacing: -.02em;
}

.rapids-mechanics h3 {
  margin: 1.7em 0 .55em;
  color: #415a83;
  font-size: 1.08em;
}

.rapids-mechanics p,
.rapids-mechanics li {
  line-height: 1.75;
}

.rapids-mechanics .note {
  margin: 1.2em 0 1.8em;
  padding: .9em 1.1em;
  color: #59677c;
  background: #f5f7fa;
  border: 1px solid #e1e7ef;
  border-left: 3px solid #8090e0;
}

.rapids-mechanics .flow {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  margin: 0 0 1.8em;
  border-top: 1px solid #dce3ec;
  border-bottom: 1px solid #dce3ec;
}

.rapids-mechanics .flow-item {
  min-height: 7.5em;
  padding: 1em 1.1em;
  border-right: 1px solid #dce3ec;
}

.rapids-mechanics .flow-item:last-child { border-right: 0; }

.rapids-mechanics .flow-item .number {
  display: block;
  margin-bottom: .8em;
  color: #8da0bd;
  font-size: .74em;
  font-weight: 700;
  letter-spacing: .12em;
}

.rapids-mechanics .flow-item strong {
  display: block;
  margin-bottom: .3em;
  color: #344b70;
}

.rapids-mechanics .flow-item span {
  color: #7d8796;
  font-size: .88em;
}

.rapids-mechanics table {
  width: 100%;
  margin: 1em 0 1.5em;
}

.rapids-mechanics th {
  color: #566783;
  background: #f5f7fa;
  font-weight: 650;
}

.rapids-mechanics td,
.rapids-mechanics th {
  border-color: #e1e7ef;
}

.rapids-mechanics .route-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 14px;
  margin: 1em 0 1.6em;
}

.rapids-mechanics .route-card {
  padding: 1em 1.15em;
  background: #fafbfc;
  border: 1px solid #e1e7ef;
  border-top: 2px solid var(--route);
}

.rapids-mechanics .route-card.valley { --route: #8090e0; }
.rapids-mechanics .route-card.river { --route: #70d0c8; }

.rapids-mechanics .route-card h3 {
  margin: 0 0 .5em;
  color: var(--route);
}

.rapids-mechanics .route-card p {
  margin: 0;
  color: #667386;
  font-size: .92em;
}

.rapids-mechanics .small {
  color: #7b8594;
  font-size: .9em;
}

.rapids-mechanics .muted {
  color: #7d8796;
}

@media (max-width: 720px) {
  .rapids-mechanics .flow { grid-template-columns: repeat(2, minmax(0, 1fr)); }
  .rapids-mechanics .flow-item:nth-child(2) { border-right: 0; }
  .rapids-mechanics .flow-item:nth-child(-n+2) { border-bottom: 1px solid #dce3ec; }
  .rapids-mechanics .route-grid { grid-template-columns: 1fr; }
}

@media (max-width: 460px) {
  .rapids-mechanics .flow { grid-template-columns: 1fr; }
  .rapids-mechanics .flow-item,
  .rapids-mechanics .flow-item:nth-child(2) { border-right: 0; border-bottom: 1px solid #dce3ec; }
  .rapids-mechanics .flow-item:last-child { border-bottom: 0; }
}
</style>

<div class="rapids-mechanics">
  <div class="rapids-mechanics-hero">
    <p class="kicker">RAPIDS / SYSTEM NOTES</p>
    <h1>副本机制</h1>
    <p>副本是一套持续运行的探索场：怪物会自然补位，人数会改变战斗节奏，搜掠和击杀共同决定最终评级。</p>
  </div>

  <div class="quick-links">
    <a href="#/rapids/dungeon">副本流程</a>
    <a href="#/rapids/dungeonlist">副本图鉴</a>
    <a href="#/rapids/materials">材料图鉴</a>
  </div>

  <div class="note"><strong>阅读提示：</strong>以下内容按当前副本配置整理。入口提示、奖励界面和服务器后续更新优先于本文；“自然刷新”与“历史回响召唤”是两套并行机制。</div>

  <h2>一局如何运作</h2>

  <div class="flow">
    <div class="flow-item"><span class="number">01 / ENTER</span><strong>进入副本</strong><span>选择已解锁的回忆段落，计时从进入后开始。</span></div>
    <div class="flow-item"><span class="number">02 / EXPLORE</span><strong>探索地图</strong><span>沿路线推进，寻找宝箱、采集物和特殊房间。</span></div>
    <div class="flow-item"><span class="number">03 / SCORE</span><strong>累积评分</strong><span>击杀速度、宝箱、采集物与 Essence 都会影响分数。</span></div>
    <div class="flow-item"><span class="number">04 / EXIT</span><strong>终点结算</strong><span>达到基础击杀要求后，在终点提交本局结果。</span></div>
  </div>

  <h2>进入与解锁</h2>

  <ul>
    <li>所有副本难度统一通过完成对应的<strong>回忆进度</strong>解锁。击杀怪物、搜掠宝箱、采集地图中的采集物，都可能推进下一段回忆。</li>
    <li>推荐等级是入口提示，不是对战斗结果的保证；装备、队伍配合和地图熟悉度同样重要。</li>
    <li><strong>峡谷·梦魇已推出。</strong> <strong>河隘·梦魇尚未推出</strong>，图鉴中的条目仅用于保留路线位置。</li>
    <li>每次成功提交都会记录本段通关与 Tier；更高难度的入口状态以游戏内当前提示为准。</li>
  </ul>

  <h2>自然刷新：副本不是静态波次</h2>

  <p>副本由多个房间刷新点共同维护。房间会在附近有玩家时周期检查，场上数量低于房间上限就会补充怪物；因此清掉一批怪物后，地图仍可能继续出现新的敌人。Essence 也在这套自然刷新池中，不需要玩家先手动召唤才会出现。</p>

  <table>
    <thead>
      <tr><th>敌人类型</th><th>遇见方式</th><th>玩家向说明</th></tr>
    </thead>
    <tbody>
      <tr><td>普通怪物</td><td>各路线的基础刷新池</td><td>构成主要击杀数，稳定提供基础材料。</td></tr>
      <tr><td>Elite</td><td>自然刷新</td><td>更强的精英敌人；有概率掉落本路线装备，并提供更高质量的材料池。</td></tr>
      <tr><td>Essence</td><td>自然刷新；部分地图还可通过历史回响召唤</td><td>击杀会给予额外进度，是 Tier 6 的必要条件；有较高概率掉落装备，也可能掉落图纸。</td></tr>
      <tr><td>特殊终点怪</td><td>特定地图的历史回响</td><td>峡谷·破晓的旧骨属于额外挑战，不是普通刷新波次。</td></tr>
    </tbody>
  </table>

  <div class="route-grid">
    <div class="route-card valley">
      <h3>峡谷：从僵尸到风蚀回响</h3>
      <p>初涉、见闻以峡谷僵尸和嶙骨僵尸为主；踏察、破晓开始加入峡谷幽魂类 Elite。梦魇使用独立的梦魇怪物配置，精英幽魂权重更高。</p>
    </div>
    <div class="route-card river">
      <h3>河隘：水路上的远近混战</h3>
      <p>初涉、见闻会同时出现河隘行尸、河隘射手与岩隘守尸；踏察、破晓加入逐流溺魂，并在高台、洞穴、仓储等区域布置更高的局部刷新上限。</p>
    </div>
  </div>

  <h3>多人规模如何影响刷新</h3>

  <p>副本不会简单地按队伍人数复制一份怪物。系统会同时调整刷新节奏、附近怪物强度和房间/全图上限：</p>

  <ul>
    <li>人数达到 2、4、6、10、16 人时，刷新周期会依次缩短约 20%、32%、45%、60%、80%。</li>
    <li>怪物血量会根据附近玩家数量提高；多人聚在同一战斗区时，处理速度和承伤压力都会上升。</li>
    <li>常规房间通常最多维持 4 只怪物，洞穴、高台、后山等特殊房间通常为 5～6 只；全图上限按难度配置为 24 或 30 只。</li>
    <li>刷新点只在有效范围内维持。离开区域太远时，怪物不会被当作整张地图的永久库存。</li>
  </ul>

  <h2>共享规则与评分</h2>

  <div class="note"><strong>组队很重要：</strong>12 格内的经验会共享；对怪物造成超过 10% 伤害，通常即可获得完整的个人击杀判定。即使中途死亡，已经产生的共享击杀奖励仍会保留。</div>

  <p>评分由击杀分、搜掠分和额外分数组成。击杀部分会看击杀速度：速度越快，单位击杀带来的评分越高；系统会将速度倍率限制在约 0.5～1.25 之间。</p>

  <table>
    <thead>
      <tr><th>行为</th><th>评分影响</th></tr>
    </thead>
    <tbody>
      <tr><td>击杀目标怪物</td><td>按击杀数与击杀速度动态计算。</td></tr>
      <tr><td>搜掠 Tier I 宝箱</td><td>每个固定增加 3 分。</td></tr>
      <tr><td>搜掠 Tier II 宝箱</td><td>每个固定增加 5 分。</td></tr>
      <tr><td>采集地图采集物</td><td>每个固定增加 5 分，同时获得采集物奖励。</td></tr>
      <tr><td>Essence 或其他额外目标</td><td>通过特殊目标或额外分数计入本局评级。</td></tr>
    </tbody>
  </table>

  <p>正常提交本局至少需要 36 个击杀或满足特殊目标带来的替代条件。Tier 4、Tier 5、Tier 6 还分别受总分与时间限制；Tier 6 需要总分超过 192、用时不超过 400 秒，并至少击杀一只 Essence。</p>

  <table>
    <thead>
      <tr><th>Tier</th><th>公开名称</th><th>门槛摘要</th></tr>
    </thead>
    <tbody>
      <tr><td>1</td><td>Common</td><td>达到基础通关要求。</td></tr>
      <tr><td>2</td><td>Unusual</td><td>总分超过 60。</td></tr>
      <tr><td>3</td><td>Remarkable</td><td>总分超过 90。</td></tr>
      <tr><td>4</td><td>Extraordinary</td><td>总分超过 120，且不超过 400 秒。</td></tr>
      <tr><td>5</td><td>Unparalleled</td><td>总分超过 160，且不超过 480 秒。</td></tr>
      <tr><td>6</td><td>Marvelous</td><td>总分超过 192、不超过 400 秒，并击杀 Essence。</td></tr>
    </tbody>
  </table>

  <h2>Essence 与历史回响</h2>

  <p>Essence 的自然刷新是副本基础机制；历史回响则是地图中额外设置的主动挑战。两者都会计入 Essence 击杀记录，区别在于是否需要消耗材料。</p>

  <ul>
    <li><strong>峡谷·踏察、峡谷·破晓：</strong>可在洞穴区域消耗合计 32 个峡谷寻常材料，召唤 Essence。</li>
    <li><strong>河隘·见闻、河隘·踏察、河隘·破晓：</strong>可在高台区域消耗合计 32 个河隘寻常材料，召唤 Essence。</li>
    <li>上述历史回响有约 5 分钟的召唤冷却；自然刷新不等同于这个召唤冷却。</li>
    <li><strong>旧骨：</strong>峡谷·破晓的额外终点挑战，召唤需要合计 64 个峡谷寻常材料，同样有约 5 分钟冷却。</li>
  </ul>

  <h2>掉落与装备</h2>

  <p>击杀掉落按敌人类型和等级分别抽取。副本内的普通掉落有每局默认 120 件的上限；装备和图纸等特殊掉落默认最多 5 件，相关副本天赋可以提高上限。</p>

  <table>
    <thead>
      <tr><th>来源</th><th>奖励规则</th></tr>
    </thead>
    <tbody>
      <tr><td>普通怪物</td><td>主要掉落寻常材料；等级差会影响掉落概率。</td></tr>
      <tr><td>Elite</td><td>有约 5% 概率掉落一件本路线随机装备，并额外抽取材料。</td></tr>
      <tr><td>Essence</td><td>约 84% 概率掉落本路线随机装备，约 16% 概率掉落对应等级图纸，并额外抽取材料。</td></tr>
      <tr><td>旧骨等特殊终点怪</td><td>会抽取装备与图纸，并掉落更高阶材料池中的物品。</td></tr>
      <tr><td>结算界面</td><td>消耗 AP 后，可在随机装备、随机材料、回忆点数等选项中选择；Tier 越高，装备与材料池越好，Tier 6 另有高品质装备。</td></tr>
    </tbody>
  </table>

  <p>本路线装备包括长剑、法杖、弓、头盔、护甲、护腿和靴子。高阶套装不是普通击杀掉落：峡谷对应“风之形”，河隘对应“河雾”，需要在打造台用图纸、路线材料与 E 制作。具体材料清单见<a href="#/rapids/materials">材料图鉴</a>。</p>

  <h2>宝箱与采集物</h2>

  <ul>
    <li><strong>Tier I 宝箱：</strong>常规材料池，通常每 10 分钟刷新一次。</li>
    <li><strong>Tier II 宝箱：</strong>稀有材料池，通常每 30 分钟刷新一次。</li>
    <li><strong>采集物：</strong>常以自然石头、水晶或碎石的外观出现，不一定有浮空提示；常规冷却约 12 分钟。</li>
    <li>宝箱分为公共箱与个人箱：公共箱共享刷新状态，个人箱只对自己独立刷新。宝箱与采集物都同时提供材料和评分。</li>
    <li>常规宝箱可能包含通用强化石；路线材料的完整清单与来源请查阅<a href="#/rapids/materials">材料图鉴</a>。</li>
  </ul>

  <h2>死亡、断线与结算状态</h2>

  <ul>
    <li><strong>死亡：</strong>有可用死亡回溯时回到本副本起点，回溯次数由对应副本天赋决定；次数用尽则返回主城。每次死亡还会按死亡次数递增扣除本局额外分数（第 1 次扣 10 分、第 2 次扣 20 分，依此类推）。</li>
    <li><strong>断线：</strong>短时间内重新登录会尝试回到原副本，允许恢复的窗口约为 60 秒；超过窗口后本局暂存状态会失效。</li>
    <li><strong>到达终点：</strong>未达到基础要求时不会完成结算；成功提交后进入等待室，领取一次奖励会结束本局奖励状态。直接离开则不会领取额外结算奖励。</li>
  </ul>

  <div class="note"><strong>一句话：</strong>先让刷新系统持续为你提供目标，再用宝箱和采集物补分，最后以速度、Essence 和特殊挑战把评级推高。</div>
</div>
