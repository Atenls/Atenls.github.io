<style>
.rapids-dungeon-list {
  max-width: 960px;
  color: #293241;
}

.rapids-dungeon-list-hero {
  margin: 1.2em 0 2.3em;
  padding: 1.7em 0 1.25em 1.5em;
  border-left: 2px solid #A0A2A4;
}

.rapids-dungeon-list-hero .kicker {
  margin: 0 0 .6em;
  color: #7b8799;
  font-size: .76em;
  font-weight: 700;
  letter-spacing: .16em;
}

.rapids-dungeon-list-hero h1 {
  margin: 0 0 .35em;
  color: #202b3c;
  font-size: 2.35em;
  font-weight: 650;
  letter-spacing: -.04em;
}

.rapids-dungeon-list-hero p {
  max-width: 42em;
  margin: 0;
  color: #748094;
  font-size: 1.04em;
  line-height: 1.75;
}

.rapids-dungeon-list .index {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 12px;
  margin: 0 0 2.8em;
}

.rapids-dungeon-list .index a {
  display: block;
  padding: 1em 1.1em;
  color: #3d5275;
  background: #f7f8fb;
  border: 1px solid #e1e5ed;
  border-radius: 4px;
  text-decoration: none;
}

.rapids-dungeon-list .index a:hover {
  border-color: #98a9c4;
  box-shadow: 0 5px 18px rgba(61, 82, 117, .08);
}

.rapids-dungeon-list .index a.valley { box-shadow: 0 0 3px #8090e060; }
.rapids-dungeon-list .index a.river { box-shadow: 0 0 3px #70d0c860; }

.rapids-dungeon-list .index strong {
  display: block;
  margin-bottom: .25em;
  font-size: 1.08em;
}

.rapids-dungeon-list .index span {
  color: #8490a1;
  font-size: .86em;
}

.rapids-dungeon-list h2 {
  margin-top: 2.5em;
  padding-bottom: .55em;
  color: #283852;
  border-bottom: 1px solid #dce3ec;
  font-size: 1.55em;
  font-weight: 650;
  letter-spacing: -.02em;
}

.rapids-dungeon-list h2.valley { border-bottom-color: #cfd5f0; }
.rapids-dungeon-list h2.river { border-bottom-color: #c5e6e2; }

.rapids-dungeon-list h3 {
  display: flex;
  align-items: center;
  gap: .65em;
  margin: 0;
  padding-top: 1.6em;
  color: #415a83;
  font-size: 1.12em;
  font-weight: 650;
}

.rapids-dungeon-entry {
  padding: 0 0 1.35em;
  border-bottom: 1px solid #edf0f4;
}

.rapids-dungeon-entry.valley {  }
.rapids-dungeon-entry.river {  }

.rapids-dungeon-entry.valley h3 { color: #5969b0; }
.rapids-dungeon-entry.river h3 { color: #348f8a; }

.rapids-dungeon-entry .meta {
  display: flex;
  flex-wrap: wrap;
  gap: .55em 1.2em;
  margin: .5em 0 .8em;
  color: #7f8998;
  font-size: .84em;
}

.rapids-dungeon-entry .status {
  color: #2d8068;
  font-weight: 700;
}

.rapids-dungeon-entry .status.soon { color: #a36f38; }

.rapids-dungeon-entry blockquote {
  margin: 0;
  padding: .85em 1.1em;
  color: #606b7b;
  background: #fafbfc;
  border-left: 2px solid #b8c4d5;
}

.rapids-dungeon-entry .detail {
  margin: .75em 0 0;
  color: #7b8594;
  font-size: .9em;
}

.rapids-dungeon-entry .detail strong { color: #596d8f; }

.rapids-dungeon-list .note {
  margin: 1.4em 0;
  padding: .9em 1.1em;
  color: #59677c;
  background: #f5f7fa;
  border: 1px solid #e1e7ef;
  border-radius: 4px;
}

@media (max-width: 620px) {
  .rapids-dungeon-list .index { grid-template-columns: 1fr; }
}
</style>

<div class="rapids-dungeon-list">
  <div class="rapids-dungeon-list-hero">
    <p class="kicker">RAPIDS / DUNGEON ATLAS</p>
    <h1>副本图鉴</h1>
    <p>此处简要记录每个副本难度的描述、推荐等级、所包含的内容。</p>
  </div>

  <div class="index">
    <a class="valley" href="#/rapids/dungeonlist#valley"><strong>峡谷</strong><span>初涉 · 见闻 · 踏察 · 破晓 · 梦魇</span></a>
    <a class="river" href="#/rapids/dungeonlist#river"><strong>河隘</strong><span>初涉 · 见闻 · 踏察 · 破晓 · 梦魇</span></a>
  </div>

  <div class="note">所有难度通过完成对应的回忆进度解锁。推荐等级是入口提示，不替代游戏内实时条件。</div>

  <h2 class="valley" id="valley">峡谷</h2>

  <p>被长风与岁月切开的峡地。</p>

  <div class="rapids-dungeon-entry valley">
    <h3>初涉 · Foray</h3>
    <div class="meta"><span class="status">当前开放</span><span>推荐等级 Lv.1</span></div>
    <blockquote>这里安宁如旧，石径、木栏与旧屋都保存完好。唯独村民们不知去向...</blockquote>
    <p class="detail">第一次踏入峡谷，从基础战斗、探索与副本评分开始。</p>
  </div>

  <div class="rapids-dungeon-entry valley">
    <h3>见闻 · Glimpse</h3>
    <div class="meta"><span class="status">当前开放</span><span>推荐等级 Lv.6</span></div>
    <blockquote>夕照落入断崖，旧屋的影子被拉得很长。那些无人提起的往事，似乎正等人听见...</blockquote>
    <p class="detail">峡谷的景象开始向更深处展开，新的路径与场景等待探索。</p>
  </div>

  <div class="rapids-dungeon-entry valley">
    <h3>踏察 · Traverse</h3>
    <div class="meta"><span class="status">当前开放</span><span>推荐等级 Lv.11</span></div>
    <blockquote>当午夜来临，被尘封的记忆席卷而来。一些血腥的证据要视而不见吗？</blockquote>
    <p class="detail"><strong>探索提示：</strong>从这一段开始，地图中会出现个人独享的采集物；采集物既能提供材料，也会增加副本分数。</p>
    <p class="detail"><strong>历史回响：</strong>可消耗合计 32 个峡谷寻常材料，于 <code>洞穴</code> 召唤 Essence 特殊怪。</p>
  </div>

  <div class="rapids-dungeon-entry valley">
    <h3>破晓 · Dawn</h3>
    <div class="meta"><span class="status">当前开放</span><span>推荐等级 Lv.16</span></div>
    <blockquote>天光刺破寒雾，沉睡的峡谷终于显出轮廓。若真相终会到来，是否也会一并带来宽恕...</blockquote>
    <p class="detail"><strong>历史回响：</strong>
      <br>可消耗合计 32 个峡谷寻常材料，于 <code>洞穴</code> 召唤 Essence 特殊怪；
      <br>可消耗合计 64 个峡谷寻常材料，于 <code>后山</code> 召唤 Final 特殊怪物 —— 旧骨。</p>
  </div>

  <div class="rapids-dungeon-entry valley">
    <h3>梦魇 · Nightmare</h3>
    <div class="meta"><span class="status">当前开放</span><span>推荐等级 Lv.20</span></div>
    <blockquote>夜色沉入旧村，连风声都像是在低语。那些被遗忘的人，真的从未离开吗？</blockquote>
    <p class="detail">峡谷的额外高阶难度。</p>
  </div>

  <h2 class="river" id="river">河隘</h2>

  <p>两山夹峙，长河自隘口奔流而过。</p>

  <div class="rapids-dungeon-entry river">
    <h3>初涉 · Foray</h3>
    <div class="meta"><span class="status">当前开放</span><span>推荐等级 Lv.21</span></div>
    <blockquote>古道沿水而行，石壁间仍有行旅留下的痕迹。前路通向山腹，似乎只是一次寻常穿行...</blockquote>
    <p class="detail">进入河隘，开始第二个副本路线的探索。</p>
  </div>

  <div class="rapids-dungeon-entry river">
    <h3>见闻 · Glimpse</h3>
    <div class="meta"><span class="status">当前开放</span><span>推荐等级 Lv.26</span></div>
    <blockquote>暮光沉入河面，崖壁上的旧痕逐渐清晰。有人曾沿这条路离开，也有人再没回来...</blockquote>
    <p class="detail"><strong>历史回响：</strong>可消耗合计 32 个河隘寻常材料，于 <code>高台</code> 召唤 Essence 特殊怪。</p>
  </div>

  <div class="rapids-dungeon-entry river">
    <h3>踏察 · Traverse</h3>
    <div class="meta"><span class="status">当前开放</span><span>推荐等级 Lv.31</span></div>
    <blockquote>夜色漫过古道，水声像在重复某段旧事。山洞深处传来的回响，真的是河声吗</blockquote>
    <p class="detail"><strong>历史回响：</strong>可消耗合计 32 个河隘寻常材料，于 <code>高台</code> 召唤 Essence 特殊怪。</p>
  </div>

  <div class="rapids-dungeon-entry river">
    <h3>破晓 · Dawn</h3>
    <div class="meta"><span class="status">当前开放</span><span>推荐等级 Lv.36</span></div>
    <blockquote>晨光从洞口照入，照见被水雾掩埋的出口。若能穿过群山，也许就能离开这段往事...</blockquote>
    <p class="detail"><strong>历史回响：</strong>可消耗合计 32 个河隘寻常材料，于 <code>高台</code> 召唤 Essence 特殊怪。</p>
  </div>

  <div class="rapids-dungeon-entry river">
    <h3>梦魇 · Nightmare</h3>
    <div class="meta"><span class="status soon">尚未推出</span><span>推荐等级 Lv.40</span></div>
    <blockquote>深夜的河水漆黑如墨，吞没了古道的尽头。若山洞不是出口，那它究竟通向何处</blockquote>
    <p class="detail">尚未开放</p>
  </div>
</div>
