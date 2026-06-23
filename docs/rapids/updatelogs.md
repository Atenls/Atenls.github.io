<style>
  * {
    font-family: 'PingFang SC', 'SF Pro', 'Hiragino Sans GB', '等线', 'Microsoft YaHei', '微软雅黑', 'Helvetica Neue', 'Helvetica', 'Arial', 'sans-serif';
  }

  .markdown-section {
    max-width: 1200px;
  }

  :root {
    --quality-color-legendary: #7ec5ff;
    --quality-color-unique: #ff5cf7;
    --quality-color-mythic: #ff3939;
  }

  .context {
    max-width: 1000px;
  }

  .redtext {
    color: #f84040; 
    font-weight: 600;
  }

  .quote {
    background: #fbfdff;
    color: #606974;
    border: 1px dashed #ccc;
    border-radius: 5px;
    font-size: 18px;
    padding: 5px;
    margin: 0px;
  }

  .table-container {
    overflow-x: auto;
    -webkit-overflow-scrolling: touch;
  }

  .content-container {
    border-radius: 1em;
    padding: 1em;
    background: rgb(22,7,22);
    color: rgb(222,222,224);
    text-align: left;
    border: 2px solid rgb(36, 0, 90);
    box-shadow: 0 0 8px rgba(36, 0, 90, 0.75);
  }

  .maintitle {
    font-size: 24px;
    font-weight: 800;
    margin: 0.6rem 0;
    color: #333;
    line-height: 1.8;
  }

  .box-context {
    font-size: 16px;
    font-weight: 500;
    color: #888;
    line-height: 1.35;
    text-align: left;
    margin: 12px 24px;
    padding: 12px 0;

    &:hover {
      color: transparent;
    }

    @media (max-width: 768px) {
      margin: 0;
      padding: 12px 4px;
    }

  }

  .markdown-section h1 {
    font-size: 2.5rem;
    font-weight: 800;
    text-shadow: 0 0 1px rgba(0,0,0,0.25);
    text-align: center;
    font-family: 'Times New Roman';
  }

  .markdown-section h2 {
    font-size: 30px;
    font-weight: 800;
    text-align: center;
    font-family: 'Times New Roman';
    margin: 0.6rem 0;
  }

  .markdown-section h4 {
    margin: 0.6rem 0;
  }

  .item-name-tag {
    background: #faf7f5;
    padding: 1px 4px;
    border-radius: 4px;
    margin: 4px;
    font-weight: 600;
    color: #333;
    box-shadow: 0 0 1px rgba(46, 22, 6, 0.1);
  }

  .tag-trans {
    background: #effff2;
    margin: 2px 4px;
    padding: 0px 3px;
    border-radius: 3px;
    color: #528f5b;
    font-weight: 600;
    font-size: 14px;
    align-items: center;
    border: 1px solid #67b171;
  }

  .tag-refactor {
    background: #f8efff;
    margin: 2px 4px;
    padding: 0px 3px;
    border-radius: 3px;
    color: #8a64a8;
    font-weight: 600;
    font-size: 14px;
    align-items: center;
    border: 1px solid #9067b1;
  }

  .download-btn {
    display: inline-block;
    padding: 1px 6px;
    border-radius: 6px;
    background: #7090d0;
    color: white;
    text-shadow: 0 1px 1px rgba(49, 71, 104, 0.2);
    text-decoration: none;
    font-weight: 700;

    &.green {
      background: #68ad68;

      &:hover {
        background: #5a9b5a;
        box-shadow: 0 1px 4px rgba(32, 78, 42, 0.2);
      }
    }

    &:hover {
      background: #4579bd;
      box-shadow: 0 1px 4px rgba(32, 51, 78, 0.2);
    }
  }
  
</style>

# Update Logs

---

<div class='greenbox'>
<p style="text-align: center; font-size: 16px;">为方便阅览及追踪更新，本栏内容排序将以倒序进行，并由时间作分隔。<br>
对于测试期间的更新日志，在表达上无可避免地会更偏向开发日志，敬请谅解。</p>
</div>

---

# 2026

---

## 2026 Jun.

---

#### 2026/06/23

<div class="little-tips" style="max-width: 400px; width: fit-content;">
  <div style="font-size:24px;">📦</div>
  <div>
  <p><strong>Rapids 资源包</strong> @ 2026/06/23</p>
  <p style="color:#aaa; font-size: 13px; line-height: 1.35;">新增「峡谷」材料贴图。<br>
  </p>
  </div>
  
  <a class="download-btn green" style="color: white;padding: inherit; border-radius: 0.75em;" href="/rapids/resourcepacks/Rapids Alpha v20260623.zip" download>点击以下载</a> 
</div>

- **怪物刷新**相关：
  - 所有 `Essence` 怪物将不会被传送回出生点或移除。<br>且当有该类怪物刷新时，将对副本内所有玩家发放公告。
    <br><img src="/rapids/rapids_img/updatelogs/20260623_essbc.png" loading="lazy">
  - 所有怪物在 `Y` 轴上的回归/移除判定将更加紧密，以避免部分穿墙、飞行怪物模型飞得太远的问题。
- 新增了副本 Tier 提升提示，当你在局内达成更高 Tier 时将发放含声音的提示。
  <br><img src="/rapids/rapids_img/updatelogs/20260623_tierup.png" loading="lazy">
- 计分板信息新增 `实时分数` 
- `法杖`: 基础 `法球飞行距离`: `15` → `18` 
- 降低了通关时奖励的额外 `E` 
- 修复了部分问题。

---

#### 2026/06/22

- **攻击相关**调整：
  - `弓箭`：
    <br><span class="inline-tips">注意到弓箭尽管已有较高的攻击系数，但在面对群攻环境时仍力有不逮。做出部分调整以尝试提升它的可用性及出场率。</span>
    - 移除了箭矢的重力影响，避免了箭矢疲软的问题。
    - 新增箭矢属性 `箭矢穿透`，基础 `+2`，使得箭矢可以在完成攻击时继续穿透目标攻击射线上其他目标。
    - 新增箭矢属性 `箭矢存活时间`，基础 `20 Ticks`，箭矢在无重力后容易自由地逃离原生家庭，遂用以限制箭矢生命周期。
    - 无法再触发近战攻击。
    - 新的**箭矢技能** `箭矢索敌` (被动技能)
      - 在射出箭矢时，将获取视线范围内最近的目标。射出的箭矢将预测对方的移动位置，并以预测位置为落点射出。
      - 该技能在面对类似「幽魂」此类高机动小型目标时，能提供目前为止最佳的攻击效果。
  - `法杖`:
    - 基础 `法球飞行距离`: `20` → `15`
    - 无法再触发近战攻击。
- 优化了副本数据结构。
- 为 `宝箱` `采集物` 增加了开启提示。
- 修复了通关奖励的装备等级按批量固定的问题。
- **通关相关**调整：

  <details>
    <summary>查看详情</summary>

    - `通用`
      - 现在至少需要 `36` 击杀才能完成关卡。
      - 新增固有 `经验` `E` 奖励
      - 当达到某一 `Tier` 后，将不会下落至更低 `Tier`
    - `Tier 6`:
      - 综合分数要求调整: `200` → `192`
      - 通关时间要求：`360s` → `400s`
    - `Tier 5`:
      - 必须在 `480s` 内完成通关。
    - `Tier 4`:
      - 必须在 `400s` 内完成通关。
    - `Tier 3`:
      - 综合分数要求调整: `80` → `90`
    - `Tier 2`:
      - 综合分数要求调整: `48` → `60`

  </details>
- **怪物相关**调整:
  <details>
    <summary>查看详情</summary>

    - `风蚀尸核` (Essence)
      - 血量: `27.5` → `24` unit
      - 攻击力: `4.8` → `4` unit
      - 移动速度: `175%` → `160%`
      - 经验值: `35 + 8 * level` → `16 + 5 * level`
    - `嶙骨僵尸` (Elite)
      - 血量: `8.75` → `8` unit
      - 攻击力: `2.25` → `2` unit
      - 经验值: `15 + 4 * level` → `8 + 2 * level`
    - `峡谷幽魂`: (Elite)
      - 血量: `8` → `6` unit
      - 护甲: `4` → `2.25` unit
      - 会心: `3` → `2` unit
      - 柔韧: `3` → `2` unit
      - 经验值: `20 + 5 * level` → `10 + 2.5 * level`
    - `峡谷僵尸` (Common)
      - 经验值: `6 + 2 * level` → `3 + 1 * level`

  </details>
- 「峡谷」副本相关：
  - `Traverse - (踏察)` 将适用等级调整为 `Lv.10+`，怪物等级同步至 Lv.10 ~ Lv.15
  - `Glimpse - (见闻)` 将适用等级调整为 `Lv.5+`，怪物等级同步至 Lv.5 ~ Lv.10
- 等级提升所能带来的数值有所提升：
  - 攻击：`+0.5`/`+0.6`/`+0.325` → `+0.75`/`0.9`/`0.4875`
  - 四项：`+0.5` → `+0.75`


---

#### 2026/06/21

<div class="little-tips purple">
  <div style="font-size:24px;">⛰</div>
  <div>
    <p><strong>峡谷 「Traverse - 踏察」</strong></p>
    <p style="color:#aaa; font-size: 13px; line-height: 1.35;">现已开放</span><br>
    你可获得 Lv.12 ~ Lv.20 之装备。
    </p>
  </div>
</div>

- 移除了 `宝箱` 的碰撞箱。
- 调整了通关评级相关内容：
  - 增加了 `时间` 的显示。
  - `Tier 6`:
    - 分数需求有所下降，同时要求至少击杀 `1` 个 `Essence` 怪物。
    - 必须在 `360s` 内完成通关，否则将无法达成 `Tier 6` 。
    - 结算奖励将额外包含 `1` 件 `高品质` 随机装备，至高 <span class="item-name-tag" style="color: #ffaa00;">传奇</span>。且它的随机等级为原范围 `+3` 。 
  - 将提高装备品质的门槛由 `Tier 5 +` 下降至 `Tier 4 +`
    - 除提升品质外，还将提高 `1` 级随机上限。
- 现在装备自身名字中也将包含一个 Overall 的百分比评级。
- 怪物刷新相关：
  - 提高了怪物刷新会话的管理范围，现在玩家将可以触发稍远范围的怪物刷新。
  - 提高了副本人数在 `2 ~ 6` 时的怪物刷新递增速率，以提升体验。 
  - 些微提升了怪物能行走的范围。
  - 玩家保护范围从 `6` 格减少为 `4` 格。
- 现在通关评级也将使用 `Tier` 评级名词。
  <details>
    <summary>评级详情</summary>

    - Tier 6: `Marverlous` (奇迹般的)
    - Tier 5: `Unparalleled` (无可比拟)
    - Tier 4: `Extraordinary` (非凡)
    - Tier 3: `Remarkable` (卓越)
    - Tier 2: `Unusual` (特别)
    - Tier 1: `Common` (寻常)

  </details>
- 调整了装备中副属性词条的排版。
- 现在异常的物品将会被自动清除。
- 降低了 `峡谷` 中 `碎石` 的 `二星材料` 产出
- 尝试修复了会出现异常的 `箭矢` 的问题。
- 使用了更优雅的方式预载简易方法，并提高了稳定性。
- 修复了 `DOT` 在状态更新时迭代器与Map冲突的问题。
- 优化了怪物血条的显示，优化了分发的逻辑，降低能耗。
- 优化了部分 Parser 的检测逻辑，并引入缓存，降低能耗。
- 将部分内容更改为使用短TTL快照/缓存。

---

#### 2026/06/20

<div class="little-tips blue">
  <div style="font-size:24px;">⛰</div>
  <div>
    <p><strong>峡谷 「Glimpse - 见闻」</strong></p>
    <p style="color:#aaa; font-size: 13px; line-height: 1.35;">现已开放</span><br>
    你可获得 Lv.6 ~ Lv.10 之装备。
    </p>
  </div>
</div>

- 现在，当通关 `Tier` 达到 `Tier 5` 或以上，不仅装备获取数量提高，还将提高装备品质。(`史诗` 几率提高 `7.3倍`) 
- **怪物掉落**相关：
  - 击杀 `Essence` 怪物后，将必定获得 `1` 件对应等级范围的随机装备。
  - 击杀 `Elite` 怪物后，将有 `5%` 概率获得 `1` 件对应等级范围的随机装备。
- 现在，所有对怪物造成超过 `10%` 生命值的伤害的玩家均能在怪物死亡后获得击杀判定。
- 调整了通关奖励相关内容：
  - 通关 `Tier` 判定由单一 `Kills` 判定改为多维度综合判定：
    - `Kills`: 仍作为主要因素参与判断。
    - `Times`: 与 `Kills` 计算得出 `KPS` 并对判定中的击杀分数造成偏移。
    - `Treasure`: 无论是宝箱还是采集物，现也将作为分数判定的一部分。
  - 现在通关时至少会有 `1` 件随机装备奖励。
  - 由于时间因素变得难以判断 Tier，现已在计分板处同步增加现在的 `Tier` 信息。
- 将部分 `Tiny` 类别宝箱由 `全局共享` 更改为 `个人独享`，现将能更好地在同图多玩家的情况下搜掠宝箱。
- 在通过 `近战` `弓` 途径进行攻击时，现已不会受目标的受伤害冷却影响。
- 现在可以通过 `+1` 来快速复读上一条消息。
- 提升了 `优秀` `卓越` `史诗` 的品质属性增幅。
- 为大部分交互操作补充了提示音，提升了交互体验。
- 补完了 `弓箭` 的 `eDPS` 信息

- 修复了 `Essence` `Elite` 怪物不计入副本击杀数的问题。
- 修复了当怪物死亡时，如有多个玩家获取经验，提示会重复生成的问题。
- 修复了装备染色异常的问题。
- 修复了部分其他问题。

---

#### 2026/06/19

- 完成了怪物掉落处理函数。
- 为 `副本会话管理器` 增加了动态 Interval 逻辑，以应对可能存在的单副本多玩家压力。
- 完成了群组结构部署。
- 添加了登录服务器，并进行了对应的配置及优化。
- 修复了部分问题。

---

#### 2026/06/18

- 完成了基本的数值曲线设计。
- 完成了「峡谷 `Foray`」的怪物及相关刷新设计。
  <details>
    <summary><strong>怪物详情</strong></summary>

    - <span class="item-name-tag" style="color: #60AA60">峡谷僵尸</span> `Common` | 刷新概率：`94.79%`
      - 中等体型
      - 移动速度 `125%` | 击退抗性 `60%`
      - 攻击 `12` + `level * 4`
      - 生命 `60` + `level * 10`
      - 护甲 `level * 20`
      - 经验值 `6` + `level * 2`
    - <span class="item-name-tag" style="color: #FF6060">嶙骨僵尸</span> `Elite` | 刷新概率：`4.74%`
      - 偏大体型
      - 移动速度 `150%` | 击退抗性 `80%`
      - 攻击 `18` + `level * 8`
      - 生命 `150` + `level * 30`
      - 护甲 `level * 40`
      - 经验值 `15` + `level * 4`
    - <span class="item-name-tag" style="color: #60E0E0">风蚀尸核</span> `Essence` | 刷新概率：`0.47%`
      - 大体型
      - 移动速度 `175%` | 击退抗性 `100%`
      - 攻击 `24` + `level * 16`
      - 生命 `480` + `level * 75`
      - 护甲 `level * 80`
      - 经验值 `level * 60`
    

  </details>

- **宝箱**相关：
  - 优化了 `宝箱` 的显示效果，优化了 `宝箱` 的搜略体验，现在所有素材可以直接进入 `QS`。
  - 完成了基本的 `宝箱` 配置与「峡谷 `Foray`」的放置。<br>宝箱将沿袭 DP 传统，位置将以刁钻难找为主要目标。
    <br><img src="/rapids/rapids_img/updatelogs/lootchest-preview.png" loading="lazy">
- 查询属性指令独立为 `/info`，你现可以更快地查询实时怪物属性。对于玩家，更推荐通过 `/stats` 查询属性。
- 新增了 `eDPS` 概念，现在 `DOT` 的伤害系数将基于 `eDPS` 来计算。
  <br>同时，当你处于战斗场景时，也可以在信息栏查看到到当前 `DPS`。
  - `eDPS` 仅为基于 rawDmage 与 攻击速度/施法速度 进行计算得出的期望数值，不包含会心/命中/元素等后续判断。
  - `rDPS` 为最近 `5s` 造成的秒均伤害。
- 新增了 Rapids 独有的 `计分板` 实现。完成了基本的信息设置。
  <br><span class="inline-tips">注：此处 AP 并非 Achievement Points，而是 Action Points， 即 PS (体力值)。但 Alpha Test 暂且用不到。</span>
  <br><div style="display: flex; gap: 1em; flex-wrap: wrap;align-items: center;"><img src="/rapids/rapids_img/updatelogs/scoreboard-default.png" loading="lazy"><img src="/rapids/rapids_img/updatelogs/scoreboard-combat.png" loading="lazy"></div>
- 完成了怪物击杀后的 `范围经验获取` 功能。暂定范围为 `12` 格。
- 优化了部分系统间的互通信链路。
- 现在，`强化` 所提升的属性将仅有 `三系攻击` `护甲` `生命值` 这类基础属性。副词条亦不参与提升。


---

#### 2026/06/17

- 完成了 Rapids 独有的 `聊天` 实现。支持消息中含 `%i` 以展示手上物品，不再支持快捷键展示。
- 优化了 `ItemManager` 的多个方法的实现。
- 新增了 `分解` 功能。<br>但通常来说，玩家不会在背包中持有材料，如想分解材料，你可以于 `QS` 中 `SHIFT + 右键` 进行分解。<br><img src="/rapids/rapids_img/updatelogs/qs-decompose.png" loading="lazy"></img>
- 新增了装备相关的处理管线： (但预计不会于 `Alpha Test` 推出)
  - 全新制作了 `拆解` 功能，用以将装备分解为对应的通用材料（如 `强化石` 等）
  - 全新制作了 `重构` 功能，用以刷新属性不如人意的高稀有装备。
  - 全新制作了 `强化` 功能，体验更好，全适配 `QS`，不再需要费心拖动物品。
- 新增了全新的、性能更佳、体验更好的 `副本会话管理器`，它将妥善地统一生成副本怪物。
- 完成了地图相关时间设定，副本中时间不会流逝。
  - `Foray` 对应 `11:00`
  - `Glimpse` 对应 `17:00`
  - `Traverse` 对应 `23:00`
  - `Dawn` 对应 `05:00`
- 现在装备如包含随机属性，将在属性值后披露对应的随机百分比。<br><img src="/rapids/rapids_img/updatelogs/random-percent-display.png" loading="lazy"></img>

---

#### 2026/06/16

- `QS` 以更强大、更易用的方式加入 Rapids。<br>与 DP 不同的是，它将向所有玩家开放。
- 新增了基于新 `ItemManager` 的独特物品存储功能。主要为 `武器`、`装备` 进行存储。
- 新增了基于新 `ItemManager` 的 `宝藏箱` 功能。
- 优化了悬浮字显示。


---

#### 2026/06/15

- 修复了材料仍会预算 seeds 导致不可堆叠的问题。

  <img src="/rapids/rapids_img/view/d01-preview.png" loading="lazy"></img><br>
- 完成了地图相关的部分工作。暂定每张地图分为四个难度/阶段：
  - `Foray` 初涉
  - `Glimpse` 见闻
  - `Traverse` 踏察
  - `Dawn` 破晓
- 新增了第一张地图「峡谷」，并进行了适用于 Rapids 的风格化改造。
  - 完成了初步的怪物设定。
  - 完成了对应的材料。
- 新增了物品大全功能，你可通过 `/items` 查看所有材料的相关信息。

---

#### 2026/06/14

- 修复了 DOT Manager 部分问题。
- 修复了 Health Regen 部分问题，进而修复了因此引起的假死问题。
- 现在死亡后会立即复活。
- 增加了基于同 UID 同属性范围的的属性重算方法。
- `法杖法球` 现可以穿透花、草、海草、藤蔓等常见可穿透方块。

---

#### 2026/06/13

- 完善了新物品管理器的功能，现所有物品都将基于同一物品管理器。
- 优化了装备技能检测/传递的逻辑。

---

#### 2026/06/12

- 全新的伤害类型：`DOT`
  - DOT 是一种持续伤害类型，其按照固定的间隔，在持续时间内进行重复的额外伤害。
  - 其伤害取决于开始或刷新时的快照伤害，惟受Boss易伤或副本增伤实时影响。

  <img src="/rapids/rapids_img/updatelogs_dot.png" loading="lazy">

  - 由于 MC 原版没有较好的适用于DOT的表现形式，制作了专用的 Mod 以直观地显示 DOT 的状态及对应的持续时间、层数、跳伤时间及伤害。
    - <a class="download-btn" style="color: white;" href="/rapids/mod/dpdothelper-1.0.0.jar" download>点击以下载</a> `DP DOT 辅助显示 Mod` v1.0.0
  - 更多信息披露，请期待后续更新的战斗系统专栏。
- 完成了更精确的怪物经验控制、及对应的浮空字经验提示。
- 完成了新的任务管理器。

---

#### 2026/06/11

- 将所有攻击类型抽离为单独的上下文并分别传递处理。
- 调整了元素属性的强化逻辑。<br>
  此前的旧逻辑在属性强化未达标准时，面对相应的怪物**绝对无法**破防，这使得一个阶段中对属强的依赖过高，并造成了不健康的等级压制。<br>
  在本改动后，不仅消除了这一情况，也大幅减弱了高数值后的不同属性造成的数值差距。
  <details>
    <summary><strong>查看详情</strong></summary>
    <div style="display: flex; align-items: stretch; margin: 0.75em 0;">
    <div style="background: #99999f; border-radius: 1em 0 0 1em; width: 48px; min-height: 60px; color: white; display: flex; align-items: center; justify-content: center; font-weight: 800;">旧</div>

    <div style="background: #cccccc40; border-radius: 0 1em 1em 0; color: #99999f; padding: 0.75em 1em; flex: 1;">

    计算公式：`(属性强化_A - 属性抗性_B) / 1000`

    即每 `1000` 属性强化提升 `100%` 属性攻击伤害。

    如受击方属性抗性高于攻击方属性强化，则造成负数伤害。

    |攻击方 `属性强化` |防御方 `属性抗性` |实际伤害增幅
    |:-:|:-:|:-:|
    | 1000  | 0        | +100%
    | 1000  | 1000     | 0%
    | 1000  | 2000     | -100% (无伤害)
    | 1000  | 3000     | -200% (给目标回血)

    </div>
    </div>

    <div style="display: flex; align-items: stretch; margin: 0.75em 0;">
    <div style="background: rgb(114, 186, 214); border-radius: 1em 0 0 1em; width: 48px; min-height: 60px; color: white; display: flex; align-items: center; justify-content: center; font-weight: 800;">新</div>

    <div style="background: #bdc7ce40; border-radius: 0 1em 1em 0; color: #717fa7; padding: 0.75em 1em; flex: 1;">

    计算公式：`(属性强化_A - 属性抗性_B) / (1000 + 属性抗性_B)`

    即所有属性强化提升的数值还将基于受击方属性抗性进行计算。

    |攻击方 `属性强化` |防御方 `属性抗性` |实际伤害增幅
    |:-:|:-:|:-:|
    | 1000  | 0        | +100%
    | 1000  | 1000     | 0%
    | 1000  | 2000     | -33%
    | 1000  | 3000     | -50%
    | 10000 | 5000     | +83.33%
    | 10000 | 15000    | -31.25%

    </div>
    </div>

  </details>

- 完成了部分基于新物品管理器的模板配置及随机项配置。
- 完成了属性插件对通过新物品管理器生成物品的专项属性计算。
- 使用了全新的怪物属性加载路径。<br>
  移除了怪物出生时的无敌时间。
- 更新了更好的伤害显示及血量恢复显示、更好的怪物血条。

---

#### 2026/06/09

- 合并了部分重复功能的模块。

---

#### 2026/06/08

- 制作了全新的、更强大的物品管理器。
- 完成了 Trial 系统的初步实现。

---

#### 2026/06/01

- 同步了多个性能优化。
- 重写了更适用于 `1.21.11` 的物品管理器反序列化部分。

---

## 2026 May

---

#### 2026/05/28

- 增加了部分安全措施。
- 现在开始禁止非中国大陆地区的 IP 访问 Rapids。
- 修复了部分情况下因竞态引起的相关问题。
- 因部分原因，重新制作了 `副本传送门`

---

#### 2026/05/26

- <span class="tag-trans">迁移</span> 完成了 **采掘系统** 的迁移工作。

---

#### 2026/05/14

- **生命偷取** 计算的最大伤害不再高于怪物最大血量。
- 近战攻击现已转变为「范围攻击」

---

#### 2026/05/10

- 修复/同步了部分问题


---

#### 2026/05/08

- <span class="tag-trans">迁移</span> 完成了 **交易所** 的迁移工作。

---

#### 2026/05/03

- 优化了 `即时性消息` 的处理逻辑，增加了数据类聚合信息功能、新增了数据类缓冲区。

---

#### 2026/05/02

- 修改了部分内容的预加载优先级，提升了稳定性。

---

#### 2026/05/01

- 增加了更自由的箭矢类底层方法。
- 套装效果支持基于等级的公式驱动。
- 方块交互功能优化。

---

## 2026 Apr.

---

#### 2026/04/30

- 新增属性 `箭矢速度`<br>
  该属性将影响射出箭矢的飞行速度，也将间接影响射出箭矢的射程。<br>
  此前默认的 **3.0x** 下调至 **1.5x**，同时 1.5x 将作为新的 `100%` 数值。
- 完成了大量基础建设

---

#### 2026/04/29

- 优化了套装功能，现在 `/stats` 中会显示已生效的所有套装效果。
- 完成了部分物品系统的基础建设。

---

#### 2026/04/28

- 制作了统一的 **ColorUtils** 以方便跨系统同步词条配色。

---

#### 2026/04/27

- **套装**支持多品质套装混合使用，优先生效更高品质的套装效果。<br>
  <div style="background: #e7e9eb; box-shadow: 0 0 8px rgba(127,127,127,0.3); color: #707073; padding: 1em; margin: 8px 0; border-radius: 1em; display: inline-block;">
  <p style="font-size: 16px;"><strong>参考</strong></p>
  <p>
  穿了 3 件 「和光同尘」(传奇) + 2 件 「和光同尘」(史诗) <br>
  此时共生效 5 件 「和光同尘」套装：</p>
  <p>
  <span style="padding-left: 8px; border-left: 4px solid #FFDDBB;"></span>生效 <span style="color: #FFAA00">传奇</span> 两件套效果<br>
  <span style="padding-left: 8px; border-left: 4px solid #C9ACC9;"></span>生效 <span style="color: #CC80CC">史诗</span> 四件套效果
  </p>
  </div>

---

#### 2026/04/26

- 增加了在快捷栏上方提示消息的功能，即时性内容将更多地迁移至此，以避免消息污染。<br>
  <img class="content-container" style="padding: 0; margin: 0.5em; overflow: hidden;" src="/rapids/rapids_img/20260426_hotbarmsg.png" loading="lazy"></img>
- 完成了对于装备的价格评定系统

---

#### 2026/04/25

- 增加了**套装功能**<br>
  <img class="content-container" style="padding: 0; margin: 0.5em; overflow: hidden;" src="/rapids/rapids_img/20260425_wuqi.png" loading="lazy"></img>

---

#### 2026/04/13

- <span class="tag-refactor">重构</span> 重新制作了**技能系统**
  <details>
    <summary style="color: #999 ;">制作了一些含技能的样品</summary>
    <img class="content-container" style="padding: 0; margin: 0.5em; overflow: hidden;" src="/rapids/rapids_img/20260413_san.png" loading="lazy"></img>
    <img class="content-container" style="padding: 0; margin: 0.5em; overflow: hidden;" src="/rapids/rapids_img/20260413_armor.png" loading="lazy"></img>
    <img class="content-container" style="padding: 0; margin: 0.5em; overflow: hidden;" src="/rapids/rapids_img/20260413_weaponskillmsg.png" loading="lazy"></img>
  </details>

---

#### 2026/04/11

- 恢复了 `法杖` 的施法音效，同时为 `射箭` 也添加了音效。<br>法杖施法音效在此前因过于吵闹被取消，现在已变更为更轻量的射箭音效。
- 调整了切换武器冷却保护的逻辑 (俗称卡法杖)，现在切换武器后不再立即清除冷却，而是将异常长的时间转为 `750ms` 冷却。

---

#### 2026/04/10

- 现在法杖也将会在快捷栏中显示施法冷却。

---

#### 2026/04/09


<div class="little-tips" >
  <div style="font-size:24px;">📜</div>
  <div>
    <p><strong>排版设计</strong></p>
    <p style="color:#aaa; font-size: 13px; line-height: 1.35;">正在进行适用于 Rapids 的全新美观设计<br>
     你可于<a href="#/rapids/design">设计</a>查看详情
    </p>
  </div>
</div>

- <span class="tag-refactor">重构</span> 重新制作了**属性词条计算系统**
- 制作了新手武器<br><img src="/rapids/rapids_img/20260409_introbow.png" loading="lazy"></img>
- 修改了箭矢射出的逻辑，现在箭矢在射出时的 `起始点` 之偏移位置会增加玩家自身的矢量<br>弓箭战斗系统增加了对「弩」的支持。
- 正在重新设计属性成长公式
  <details>
      <summary style="color: #999 ;">点击以查看详情</summary>
      <p style="color: #aaa; margin-left: 3px; padding-left: 12px; border-left: 3px solid #ccc;">
      1. 「近战 / 箭矢 / 魔法」攻击的划分现在更加明确，它们的期望 DPS 现遵从 100 : 90 : 70。
      </p>
  </details>

---

#### 2026/04/08

- <span class="tag-refactor">重构</span> 重新制作了**物品管理系统**<br>版本差异过大，迁移问题多多，无法满足需求
- 修复了**数据管理器**的 MySQL 连接异常的问题
- 补充了部分内容的新版本特性

---

#### 2026/04/07

- 新增 `个性签名` 功能，在查看个人属性时可进行修改。它人在查询属性时，也将显示于个人资料中。
- 新增 **木桩** `N1` `N2` 于主城广场


---

#### 2026/04/06

- <span class="tag-trans">迁移</span> 完成了**属性系统**的迁移
  - 制作了内嵌的属性查询功能，并优化了排版<br>![stats](/rapids_img/20260406_stats.png)
    - 通过 `/stats` 查看个人属性
    - 通过 `SHIFT + 右键` 查看他人属性
  - 重新设计了属性对应颜色
  - 现在 `左键` 也可以使用法杖
  - 采用了更健壮的写法
  - 修复了版本更迭导致的差异内容
  - 将部分依赖转译的信息显示更改为原生计算
- 重新调整了基础属性和等级提升属性
- <span class="tag-refactor">重构</span> 重新制作了**等级系统**
  - 现在等级系统不再独立存在，而内嵌于属性系统
  - 使用了性能更佳的写法
  - 重新设计了 `经验加成` 的生效方法，现在将不会存在不同经验加成乘区*（经验券x装备）*。
- 重新调整了经验公式
- <span class="tag-trans">迁移</span> 完成了**物品管理**的迁移
- <span class="tag-trans">迁移</span> 完成了**数据系统**的迁移
- <span class="tag-refactor">重构</span> 重新制作了**方块交互系统**
- <span class="tag-refactor">重构</span> 重新制作了**会话管理系统**
- <span class="tag-refactor">重构</span> 重新制作了**伤害显示系统**
- <span class="tag-refactor">重构</span> 重新制作了**记录系统**
- <span class="tag-refactor">重构</span> 重新制作了**背包管理系统**
- <span class="tag-trans">迁移</span> 完成了**仓库系统**的迁移

- 尝试选择了新的排版，并制作了第一把武器 `不止歇的激流` <br>![](/rapids_img/20260406_不止歇的激流.jpg)


---

#### 2026/04/05

<img src="/rapids/rapids_img/20260405_spawn.jpg" loading="lazy"></img>
- 完成了 **服务端** 的基础框架
  - 完成了适用于 RPG 的规则/参数设置
- 完成了 **主城** 的选定
  - 进行了适用于 Rapids 的风格化改造
- <span class="tag-refactor">重构</span> 重新制作了**世界保护系统** (含玩家交互控制)
- <span class="tag-trans">迁移</span> 开始了**属性系统**的迁移

---

<p style="color: #999;"> 本栏只记录 <strong>2026/04/05</strong> 后的内容 </p>
