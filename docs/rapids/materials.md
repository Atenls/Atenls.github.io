<style>
.rapids-materials {
  max-width: 960px;
  color: #293241;
}

.rapids-materials-hero {
  margin: 1.2em 0 2.3em;
  padding: 1.7em 0 1.25em 1.5em;
  border-left: 2px solid #A0A2A4;
}

.rapids-materials-hero .kicker,
.rapids-materials .eyebrow {
  margin: 0 0 .6em;
  color: #7b8799;
  font-size: .76em;
  font-weight: 700;
  letter-spacing: .16em;
}

.rapids-materials-hero h1 {
  margin: 0 0 .35em;
  color: #202b3c;
  font-size: 2.35em;
  font-weight: 650;
  letter-spacing: -.04em;
}

.rapids-materials-hero p {
  max-width: 46em;
  margin: 0;
  color: #748094;
  font-size: 1.04em;
}

.rapids-materials .quick-links {
  display: flex;
  flex-wrap: wrap;
  gap: .55em 1.4em;
  margin: -1em 0 2.3em;
  color: #6f7b8d;
  font-size: .9em;
}

.rapids-materials a {
  color: #4f70a5;
  font-weight: 600;
}

.rapids-materials h2 {
  margin: 2.7em 0 1em;
  padding-bottom: .45em;
  color: #283852;
  border-bottom: 1px solid #dce3ec;
  font-size: 1.45em;
  font-weight: 650;
  letter-spacing: -.02em;
}

.rapids-materials h2.valley { border-bottom-color: #cfd5f0; }
.rapids-materials h2.river { border-bottom-color: #c5e6e2; }

.rapids-materials h3 {
  margin: 1.65em 0 .45em;
  color: var(--route);
  font-size: 1.08em;
}

.rapids-materials p,
.rapids-materials li {
  line-height: 1.75;
}

.rapids-materials .note {
  margin: 1.2em 0 1.8em;
  padding: .9em 1.1em;
  color: #59677c;
  background: #f5f7fa;
  border: 1px solid #e1e7ef;
}

.rapids-materials .source-grid {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 0;
  margin: 1em 0 1.8em;
  border-top: 1px solid #dce3ec;
  border-bottom: 1px solid #dce3ec;
}

.rapids-materials .source-item {
  padding: 1em 1.05em;
  border-right: 1px solid #dce3ec;
}

.rapids-materials .source-item:last-child { border-right: 0; }

.rapids-materials .source-item strong {
  display: block;
  margin-bottom: .3em;
  color: #415a83;
}

.rapids-materials .source-item span {
  color: #7d8796;
  font-size: .88em;
}

.rapids-materials .material-list {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 0 24px;
}

.rapids-materials .material-entry {
  --route: #5969b0;
  padding: 0 0 1.2em;
  border-bottom: 1px solid #edf0f4;
}

.rapids-materials .material-entry.valley { --route: #5969b0; }
.rapids-materials .material-entry.river { --route: #348f8a; }

.rapids-materials .material-entry h3 {
  margin-bottom: .35em;
}

.rapids-materials .material-entry .meta {
  display: flex;
  flex-wrap: wrap;
  gap: .45em 1em;
  margin-bottom: .65em;
  color: #7b8594;
  font-size: .82em;
}

.rapids-materials .rarity {
  color: #5969b0;
  font-weight: 700;
}

.rapids-materials .rarity.common { color: #4b9d6b; }
.rapids-materials .rarity.rare { color: #5969b0; }
.rapids-materials .rarity.epic { color: #a25ca2; }
.rapids-materials .rarity.legendary { color: #bd7a13; }

.rapids-materials blockquote {
  margin: 0;
  padding: .75em 1em;
  color: #667386;
  background: #fafbfc;
  border: none;
  border-radius: 4px;
  box-shadow: 0 0 2px rgba(0,0,0,.1);
  font-size: .92em;
}

.rapids-materials .usage {
  margin: .65em 0 0;
  color: #7b8594;
  font-size: .88em;
}

.rapids-materials table {
  width: 100%;
  margin: 1em 0 1.5em;
}

.rapids-materials th {
  color: #566783;
  background: #f5f7fa;
  font-weight: 650;
}

.rapids-materials td,
.rapids-materials th {
  border-color: #e1e7ef;
}

.rapids-materials .small {
  color: #7b8594;
  font-size: .9em;
}

@media (max-width: 720px) {
  .rapids-materials .source-grid,
  .rapids-materials .material-list { grid-template-columns: 1fr 1fr; }
  .rapids-materials .source-item:nth-child(2) { border-right: 0; }
  .rapids-materials .source-item:nth-child(-n+2) { border-bottom: 1px solid #dce3ec; }
}

@media (max-width: 460px) {
  .rapids-materials .source-grid,
  .rapids-materials .material-list { grid-template-columns: 1fr; }
  .rapids-materials .source-item,
  .rapids-materials .source-item:nth-child(2) { border-right: 0; border-bottom: 1px solid #dce3ec; }
  .rapids-materials .source-item:last-child { border-bottom: 0; }
}
</style>

<div class="rapids-materials">
  <div class="rapids-materials-hero">
    <p class="kicker">RAPIDS / MATERIAL ATLAS</p>
    <h1>材料图鉴</h1>
    <p>材料不是只从怪物身上来。击杀、结算、宝箱和地图采集物，分别组成一条完整的收集路线。</p>
  </div>

  <div class="quick-links">
    <a href="#/rapids/dungeon">副本流程</a>
    <a href="#/rapids/dungeonlist">副本图鉴</a>
    <a href="#/rapids/dungeonmechanics">副本机制</a>
  </div>

  <div class="note"><strong>图鉴说明：</strong>来源写的是当前副本配置中能确认的主要来源，不代表未来不会增加其他来源。<br>除本图鉴外，你也可以在游戏中通过 <code>/items</code> 查看物品大全。</div>

  <h2>四种获取方式</h2>

  <div class="source-grid">
    <div class="source-item"><strong>击杀怪物</strong><span>普通怪物掉寻常材料，Elite / Essence 的材料池更深。</span></div>
    <div class="source-item"><strong>结算领取</strong><span>消耗 AP 从本路线材料池随机抽取，评级越高越容易碰到稀有材料。</span></div>
    <div class="source-item"><strong>搜掠宝箱</strong><span>Tier I 给常规池，Tier II 给稀有池；公共箱和个人箱独立刷新。</span></div>
    <div class="source-item"><strong>采集地图物</strong><span>右键采集自然石头、水晶、碎石等外观的采集物，同时增加 5 分。</span></div>
  </div>

  <ul>
    <li>普通材料是每条路线的前三种材料。打造配方中的「寻常材料」指这三种材料的总数量，可混合缴纳。</li>
    <li>Tier 4、Tier 5 结算有机会获得稀有材料；Tier 6 结算大概率获得稀有材料，并有机会附带本路线图纸。</li>
    <li>常规宝箱的材料池会包含强化石；强化石是通用物品，不属于峡谷或河隘专属材料。</li>
  </ul>

  ## 峡谷材料

  <p class="small">峡谷材料主要用于「风之形」套装的打造，也会用于峡谷历史回响。颜色从青绿、蓝色到紫色和橙色逐步提高稀有度。</p>

  <div class="material-list">
    <article class="material-entry valley">
      <h3>崖根枯枝 <span class="rarity common">寻常</span></h3>
      <div class="meta"><span>标价 10 E</span><span>击杀 / 结算 / Tier I、Tier II 宝箱</span></div>
      <blockquote>从崖根灌木上折落的枯枝。干裂的枝节像是记录着漫长旱季。</blockquote>
      <p class="usage"><strong>用途：</strong>峡谷寻常材料；可用于历史回响与「风之形」配方。</p>
    </article>
    <article class="material-entry valley">
      <h3>风化碎石 <span class="rarity common">寻常</span></h3>
      <div class="meta"><span>标价 12 E</span><span>击杀 / 结算 / 宝箱 / 采集物</span></div>
      <blockquote>被风轻抚而从崖壁跌落的碎石。在裂痕中仿佛能看见岁月的痕迹。</blockquote>
      <p class="usage"><strong>用途：</strong>峡谷寻常材料；「峡谷碎石」采集物的主要材料池之一。</p>
    </article>
    <article class="material-entry valley">
      <h3>苔痕石片 <span class="rarity common">寻常</span></h3>
      <div class="meta"><span>标价 16 E</span><span>击杀 / 结算 / 宝箱 / 采集物</span></div>
      <blockquote>覆着浅苔的崖壁碎片。潮湿的纹路里残留着山风的气息。</blockquote>
      <p class="usage"><strong>用途：</strong>峡谷寻常材料；可用于历史回响与「风之形」配方。</p>
    </article>
    <article class="material-entry valley">
      <h3>风蚀石核 <span class="rarity rare">稀有</span></h3>
      <div class="meta"><span>标价 60 E</span><span>Elite / Essence / 结算 / Tier I、Tier II 宝箱</span></div>
      <blockquote>藏在碎石深处的坚硬石核。外层早已被风沙磨去，只剩沉默的轮廓。</blockquote>
      <p class="usage"><strong>用途：</strong>峡谷稀有材料；普通「风之形」配方需要 36 个，高阶配方需要 64 个。</p>
    </article>
    <article class="material-entry valley">
      <h3>风蚀晶簇 <span class="rarity rare">稀有</span></h3>
      <div class="meta"><span>标价 85 E</span><span>Elite / Essence / Tier II 宝箱 / 采集物 / 高阶结算</span></div>
      <blockquote>从崖壁深处剥落的浅蓝晶簇。晶面被长风打磨，映着细碎冷光。</blockquote>
      <p class="usage"><strong>用途：</strong>峡谷稀有材料；普通配方需要 6 个，高阶配方需要 18 个。</p>
    </article>
    <article class="material-entry valley">
      <h3>古崖髓石 <span class="rarity epic">史诗</span></h3>
      <div class="meta"><span>标价 200 E</span><span>Elite / Essence / Tier II 宝箱 / 采集物 / 高阶结算</span></div>
      <blockquote>凝结在古老岩层中的石髓。敲击时会传出低沉而悠远的回响。</blockquote>
      <p class="usage"><strong>用途：</strong>「风之形」高阶配方的核心材料，需要 6 个。</p>
    </article>
    <article class="material-entry valley">
      <h3>苍风琉砂 <span class="rarity epic">史诗</span></h3>
      <div class="meta"><span>标价 260 E</span><span>Tier II 宝箱 / 特殊终点掉落池</span></div>
      <blockquote>只在高崖风眼中沉积的细砂。每一粒都像封存着一缕苍白的风。</blockquote>
      <p class="usage"><strong>用途：</strong>高阶「风之形」配方；等级 15 配方需要 2 个，等级 20 配方需要 3 个。</p>
    </article>
    <article class="material-entry valley">
      <h3>断空石英 <span class="rarity epic">史诗</span></h3>
      <div class="meta"><span>标价 320 E</span><span>副本掉落来源待补充</span></div>
      <blockquote>裂隙边缘凝成的透明石英。折射出的光影仿佛被切成数段。</blockquote>
      <p class="usage"><strong>暂无获取途径</strong></p>
    </article>
    <article class="material-entry valley">
      <h3>岁痕玉髓 <span class="rarity legendary">传奇</span></h3>
      <div class="meta"><span>标价 750 E</span><span>副本掉落来源待补充</span></div>
      <blockquote>深埋于崖心的温润玉髓。内部的层纹像是漫长岁月留下的年轮。</blockquote>
      <p class="usage"><strong>暂无获取途径</strong></p>
    </article>
  </div>

  ## 河隘材料

  <p class="small">河隘材料主要用于「河雾」套装的打造，也会用于河隘历史回响。河水冲刷出的寻常材料，向渡痕、行札和沉舟遗物逐步过渡。</p>

  <div class="material-list">
    <article class="material-entry river">
      <h3>洄岸碎砾 <span class="rarity common">寻常</span></h3>
      <div class="meta"><span>标价 36 E</span><span>击杀 / 结算 / Tier I、Tier II 宝箱 / 采集物</span></div>
      <blockquote>被河水反复冲刷过的圆砾。表面仍残留着潮湿而清冷的水痕。</blockquote>
      <p class="usage"><strong>用途：</strong>河隘寻常材料；可用于历史回响与「河雾」配方。</p>
    </article>
    <article class="material-entry river">
      <h3>潮岸浮叶 <span class="rarity common">寻常</span></h3>
      <div class="meta"><span>标价 30 E</span><span>击杀 / 结算 / Tier I、Tier II 宝箱</span></div>
      <blockquote>被河水推上岸边的湿润叶片。叶脉间仍挂着未干的水光。</blockquote>
      <p class="usage"><strong>用途：</strong>河隘寻常材料；可用于历史回响与「河雾」配方。</p>
    </article>
    <article class="material-entry river">
      <h3>浅滩细贝 <span class="rarity common">寻常</span></h3>
      <div class="meta"><span>标价 42 E</span><span>击杀 / 结算 / 宝箱 / 采集物</span></div>
      <blockquote>散落在浅滩泥沙中的小贝壳。贴近耳边时，似乎还能听见细微水声。</blockquote>
      <p class="usage"><strong>用途：</strong>河隘寻常材料；可用于历史回响与「河雾」配方。</p>
    </article>
    <article class="material-entry river">
      <h3>渡痕铜片 <span class="rarity rare">稀有</span></h3>
      <div class="meta"><span>标价 160 E</span><span>击杀 / 结算 / 宝箱 / 采集物</span></div>
      <blockquote>从旧行囊中翻出的残旧铜片。边缘磨损严重，像被许多人反复握过。</blockquote>
      <p class="usage"><strong>用途：</strong>河隘稀有材料；普通「河雾」配方需要 36 个，高阶配方需要 64 个。</p>
    </article>
    <article class="material-entry river">
      <h3>水封行札 <span class="rarity rare">稀有</span></h3>
      <div class="meta"><span>标价 200 E</span><span>Elite / Essence / 结算 / Tier II 宝箱 / 采集物</span></div>
      <blockquote>被油蜡封住的旧日行札。字迹已被潮气晕开，只剩几处地名尚能辨认。</blockquote>
      <p class="usage"><strong>用途：</strong>「河雾」普通配方需要 6 个，高阶配方需要 18 个。</p>
    </article>
    <article class="material-entry river">
      <h3>沉舟漆片 <span class="rarity epic">史诗</span></h3>
      <div class="meta"><span>标价 540 E</span><span>Elite / Essence / Tier II 宝箱 / 采集物 / 高阶结算</span></div>
      <blockquote>从水下旧船残骸上剥落的漆片。暗色漆面仍残留着某个渡标的纹样。</blockquote>
      <p class="usage"><strong>用途：</strong>「河雾」高阶配方需要 6 个。</p>
    </article>
    <article class="material-entry river">
      <h3>归途残铃 <span class="rarity epic">史诗</span></h3>
      <div class="meta"><span>标价 750 E</span><span>Tier II 宝箱 / 特殊怪物掉落池</span></div>
      <blockquote>行旅曾系在包上的小铃残件。轻晃时没有铃声，只余一阵遥远的回响。</blockquote>
      <p class="usage"><strong>用途：</strong>高阶「河雾」配方；等级 35 配方需要 2 个，等级 40 配方需要 3 个。</p>
    </article>
  </div>

  ## 图纸、装备与打造台

  <p>材料图鉴也记录与材料直接相连的制作线。击杀掉落和结算领取的装备属于路线基础装备；高阶套装需要在打造台完成。</p>

  <table>
    <thead>
      <tr><th>路线</th><th>图纸</th><th>等级</th><th>特殊装备部位</th><th>常规装备部位</th></tr>
    </thead>
    <tbody>
      <tr><td>峡谷</td><td>风之形</td><td>Lv.5 ~ 20</td><td>弓、长剑</td><td>长剑、法杖、弓、头盔、护甲、护腿、靴子</td></tr>
      <tr><td>河隘</td><td>河雾</td><td>Lv.25 ~ 40</td><td>法杖</td><td>长剑、法杖、弓、头盔、护甲、护腿、靴子</td></tr>
    </tbody>
  </table>

  <h3>普通配方</h3>
  <ul>
    <li><strong>峡谷：</strong>对应等级 1 张风之形图纸、6 个风蚀晶簇、36 个风蚀石核，以及 192 个峡谷寻常材料。</li>
    <li><strong>河隘：</strong>对应等级 1 张河雾图纸、6 个水封行札、36 个渡痕铜片，以及 192 个河隘寻常材料。</li>
  </ul>

  <h3>高阶配方</h3>
  <ul>
    <li><strong>峡谷：</strong>3 张对应等级图纸、6 个古崖髓石、18 个风蚀晶簇、64 个风蚀石核，以及 512 个峡谷寻常材料；等级 15/20 还分别需要 2/3 个苍风琉砂。</li>
    <li><strong>河隘：</strong>3 张对应等级图纸、6 个沉舟漆片、18 个水封行札、64 个渡痕铜片，以及 512 个河隘寻常材料；等级 35/40 还分别需要 2/3 个归途残铃。</li>
    <li>高阶配方还需要 E，并要求对应路线的 Tier 6 通关记录；同一路线的前序配方至少打造 3 次后，才会开放「精雕细琢」配方。</li>
  </ul>

  <div class="note"><strong>收集建议：</strong>先把寻常材料当作路线通用库存，再根据想做的等级保留蓝色与紫色材料。Tier II 宝箱、Essence 和高 Tier 结算，是补齐稀有材料与图纸的主要途径。</div>
</div>
