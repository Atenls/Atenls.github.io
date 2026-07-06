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

## 2026 Jul.

<div class="divider" style="margin: 2em 0;">
  <span>以下为 Beta Test 内容</span>
</div>

#### 2026/07/06

- 修复了结算时「图纸」掉率错误地受等级影响而增加。
- 你现已可打造全新的「河雾」套装部件。
  - 所有部件均有概率获得 `光属性强化` `光属性抗性` `暗属性抗性`
  - `5%` 产出含 `法球飞行速度` 的 「**微光法杖**」
  - 所有武器均含 `光属性强化` 主词条
- **「河隘」材料**相关：
  - `沉舟漆片` 调整为 `三星` (紫色)
  - 所有材料依照河隘副本平均等级进行了价值重设。
- HoloAPI 新增支持了类似信标的光柱效果，暂无实际应用。
- 修复了「河隘」`初涉` 部分碎石未正常加载的问题。

---

#### 2026/07/05

- 大幅增强了「再入」增益效果的数值。并将两个选择项修改为不会重复。
- 修复了「河雾怨魂」技能 `雾步` 对玩家距离判断不正确的问题。
- 降低了「河雾怨魂」的血量。
- 修复了「河隘」套装没有效果的问题。

---

#### 2026/07/04

<div class="divider" style="margin: 0.5em 0; --divider-color: #f3f4f5;">
  <span class="item-name-tag">晚间</span>
</div>

- **「怪物属性」**相关修改：
  - 将`河雾怨魂`技能 `雾步` (主要表现为传送) 的生效距离从 `16` 格外修改为 `20` 格外。
  - 大幅降低了`河雾怨魂`的各技能伤害系数。综合削弱约 `55%`。
  - 降低了 `河隘射手` `岩隘守尸` `河雾怨魂` 的攻击。
  - 大幅降低了 `河隘射手` 的攻击频率。

<div class="divider" style="margin: 0.5em 0; --divider-color: #f3f4f5;">
  <span class="item-name-tag">午间</span>
</div>

- 副本「河隘」`初涉` 现已开放。
  - 含四类「河隘」基准怪物，包括全新带有技能组的 `河雾怨魂` (Essence)
  - 含 `2x`/`6x` 个人独享/全局共享碎石、`13x` 个人独享宝箱
- 为拓展性需求及数据安全考虑，玩家数据相关已修改为全面数据库存储，服务器端侧不再保存任何玩家数据。
- 完善了脚本的 Bridge 转译函数，内置了更多拓展性功能并节省了性能开销。
- 优化了天赋生效的提示。

---

#### 2026/07/03

- 新增主菜单，并附新的信息披露功能「统计」。
  - 如你在副本中，你可以通过主菜单的：
    - `脱离卡死`：回到副本出生点
    - `离开副本`：回到主城
  - 你可以在「统计」中查看自己各副本的击杀数、通关次数、宝箱或采集物收集次数等内容。
- 完善了 `游泳速度` 控制。
- 再次增大了 `峡谷幽魂` 的体型。同时将其更改为 `暗属性`。
- 为「峡谷」中的部分怪物增加了元素属性抗性。
- 新增属性：
  - `投掷伤害增幅`：适用于 `三叉戟` 模型武器，增益投掷武器的造成的伤害。默认值 `200%`。
  - `重击伤害增幅`：适用于 `重锤` 模型武器，增益重锤重击的造成的伤害。默认值 `100%`。
- 优化了聊天格式，现在聊天将额外显示玩家所在区域，为保简洁，副本难度将以颜色划分，不显示难度名。
- 优化了数据库相关的部分内容。

#### 2026/07/02

- 现在经验获取将受等级差影响，在等级差超过 `10%`/`4` 时，将开始递减，在 `25%`/`8` 时（以较大值为准），将无法获得任何经验。
- 大幅降低了「升阶」的价格及材料需求。
- 在「熔铸」时，每件 `材料装备` 所能提升的词条百分比大幅提升：`5%` → `7.5%`，且在同一轮次中，堆叠每 `3` 件将获得更多的额外提升。
- 修复了副词条在进行「熔铸」时，不同组别的副词条会发生冲突并被更新成基础词条的问题。如 `魔法穿透` → `会心`。
- 优化了含范围的主词条 (`攻击`) 的相关内容：
  - 现在装备将记录 Range 各自的 random seed。
  - 修复了在「熔铸」或「升阶」时会基于同 seed 的百分比进行均值回归的问题。
  - 该修复只对新产出的装备有效。
- 修复了「精雕细琢」配方制作时不会扣除稀有材料的问题。
- 在主城木桩旁新增了 `DPS 指示器`
- 修复了部分问题。
- 将背包数据迁移至数据库存储，数据基于 Rapids 物品管理器。并使用了先进且优雅的方法，理论上玩家不会感觉到任何不同。
- 新的天赋 `宝藏眷顾`，激活天赋后，你可从 `宝箱` 中获得更多物资。
  <br><img src="/rapids/rapids_img/updatelogs/20260702_lootbonus.png" loading="lazy">
- 略微降低了 `搜掠本能` Tier 1 的回忆点数需求，并降低了所有 Tier 的冷却时间以提高效用。
- 调整了副本结算时 `直接离开` 的按钮位置，避免误触。
- 降低了「峡谷 `梦魇`」中 `Essence` 怪物的刷新几率。


---

#### 2026/07/01

- 现在，当你在副本内离线时，如你在 `60s` 内重新登录，将可自动返回副本。
- 为优化较少人数时的副本体验，现在怪物所能行走的距离大幅增加。
- 现在「再入」将提供两条增益选择，你将可以更自由地决定。
- 略微提高了 `Tier 5` 所能获得的材料数量。
- 略微提高了 `强化石` 的产出。
- 得益于 Rapids 的全流程管理，移除了部分旧有属性管线的不必要判定，减少了性能浪费。
- 修复了部分解释器未能正常生效的问题。
- 调整了「洞穴」中「Reminiscence」的位置，以减少误触。
- 将怪物的血量数值刷新时间更改为实时。
- 修改了更合理的实时伤害。
- 你现可于 `副本天赋台` 中使用 `回忆点数` 提升天赋。
  - 你现可将各难度的 `回忆点数` 按一定比例兑换为 `回望` 点数，并用以升级天赋。
  - 「搜掠本能」：进入副本时，重置所有 `个人宝箱` 或 `采集物` （冷却及范围依照等级）

---

## 2026 Jun.

---

#### 2026/06/30

- `宝箱` 现已支持一键搜掠功能，同时，如 `QS` 已满，点击物品亦将直接进入背包，无需拖动。
  - 为顺应效率变更，开启宝箱的保护时间将降低至 `1.5s`
- 新增 `峡谷宝箱` Tier 2，每个场景各有一个，且位置不同。将有概率开出 `苍风琉沙`，并有更高的概率获得 `古崖髓石`。
- 「风之形」精雕细琢配方现将需求 `苍风琉砂`。
- 完成了数据库统一 Lib，并为多个插件完成了迁移。
- 聊天现已支持 `屏蔽` 功能，你可通过 `/ignore <ID>` 屏蔽对应玩家。
  - 当屏蔽时，你将无法收到或发送对方的私聊，且公屏和世界中也将忽略对方。
- 修复了在交互方块时能触发需 `左键` 使用的武器技能之问题。
- 增大了 `峡谷幽魂` 的体型，以便更好地被攻击。
- 提高了 `风蚀晶簇` 的综合产出。
- 新增「Reminiscence」功能，你可于 `踏察` 及之后的副本中消耗 `寻常材料` 召唤 `Essence` 或 `Final` 怪物。
  - 你现可于 「峡谷 `破晓`」召唤 `旧骨` (Final)，它将有较高概率掉落图纸、高稀有材料。
- 你现可前往 「峡谷 `梦魇`」，惟在 `破晓` 达成 Marvelous 通关，且击杀 `旧骨` 后才能前往。
- 现已开放「再入」功能，你可以通过 `再入` 无限地堆叠增益，以获取更轻松的副本体验。并可获取 `75%` 回忆点数。
- 现已在测试中启用 `AP` 系统，所有结算后选择的额外奖励将消耗 `AP` 进行。
- 你现可于「副本天赋台」中通过 `回忆点数` 兑换对应副本之装备。
- 「拆解台」现已支持合并拆解。
- 修复了部分问题，优化了部分描述。
- 在早期场景中增加了部分副本资讯。

---

#### 2026/06/29

- 调整了 `品质` `品级` 的补正系数，降低了品质间差距。
  <details>
    <summary>查看详情</summary>

    **品质**:

    - **神话**: `2.75` → `2.375`
    - **传奇**: `2.25` → `2.0`
    - **史诗**: `1.75` → `1.6875`
    - **卓越**: `1.5` → `1.4375`

    **品级**:

    - **最上级**: `1.4` → `1.35`
    - **上级**: `1.2` → `1.15`
    - **最下级**: `0.75` → `0.8`

  </details>
- 调整了「风之形」打造配方的需求。
  <br>风之形套装部件的强度过高，以至于积攒材料 All in 成为了唯一的优解，这不仅不利于装备的多样性，也使得玩家强度更多依赖打造跃迁。
  <br>因此，除品质系数的调整外，还进行了配方打造前置的限制，并提高了材料需求。
  - `标准` 制作现也将需求同等级关卡的 `Marvelous` 通关。
  - `精雕细琢` 配方现在将需求下一等级关卡的 `Marvelous` 通关。即 `Lv.5` 需要「见闻」，以此类推。
    <br>同时，在开始 `精雕细琢` 前，至少需完成 `3` 次 `标准` 配方的打造。
  - 现在通过 `精雕细琢` 打造的装备将无法上架交易所。
- 略微降低了 `风蚀石核` 的产出。
- 提高了结算奖励中 `E` 的产出。
- 优化了部分描述。
- 补全了「峡谷」`破晓` `梦魇` 的宝箱和收集物。
- 在拆解台获得 `晶髓碎片` 现在将直接进入 `QS`。
- 现在，在打开 `宝箱` 时，附近怪物将在 `3s` 内忽略你。


<div class="divider" style="margin: 2em 0;">
  <span>以下为 内部测试 内容</span>
</div>

#### 2026/06/28

- **材料相关**调整：
  - `风蚀石核` 品质修改为 `二星 (蓝色)`，价值提升至 `60`
  - `古崖髓石` 品质修改为 `三星 (紫色)`，价值提升至 `200`
  - 「峡谷(寻常材料)」定义范围修改为 `崖根枯枝` `风化碎石` `苔痕石片`
  - 几率进行了相应的调整
- 打造「风之形」套装部件的材料需求进行了相应调整。
- 调整了怪物经验公式，提高了前期的提升速度。
- 在「峡谷」 `初涉` `见闻` 增加了多个简易搜寻可得的 `个人独享` 宝箱。
- 略微提高了宝箱及收集物的刷新 CD。
- 调整了装备价值的公式，使得高品质装备具备更高的价值。
- 副本结算奖励新增了「回忆点数」。

---

#### 2026/06/27

- **怪物属性**相关：
  - 调整了怪物的属性公式，以适合更完备的装备成长系统。并略微降低了前期难度。
  - 略微降低了 `Elite` `Essence` 的期望伤害，并由固定值更改为随机值。
  - 现在，除 `Essence` 怪物将受 `局内` 所有玩家影响外，所有其余怪物也将随 `场景内` 人数动态上升血量。且统一为每玩家 `+15%`。
    <br>场景通常为一个小的刷怪空间，但其激活范围大约在 `64x64`，因此实际上会出现场景互相覆盖的情况。
- 添加了部分场景内提示、指引。
- 为市场进行了更完善的迁移适配。
- 修复了在持有 `弓` 或 `法杖` 类武器时，无法正常打开 `宝箱` 的问题。 
- 新增 `升阶台` 与 `拆解台`：
  <br><img src="/rapids/rapids_img/updatelogs/20260627_leveluptable.png" loading="lazy">
  <br><img src="/rapids/rapids_img/updatelogs/20260627_equipdecompose.png" loading="lazy">
  - 你可以通过 `升阶台` 消耗 `材料碎片` (暂定命名) 及 `E` 来有限度地提升你的装备等级。该价格还将取决于装备品质。
  - 你可以通过 `拆解台` 获取 `材料碎片`
- 「峡谷」`Dawn - 破晓` 现已开放，并新增多个场景，含新的高精英怪刷新率场景「后山」。
  <br><img src="/rapids/rapids_img/updatelogs/20260627_d104.png" loading="lazy">


<div class="divider" style="margin: 2em 0;">
  <span>以下为 Alpha Test 内容</span>
</div>

#### 2026/06/26


- **Alpha Test 圆满结束！**
  <br>我们已得到了较多反馈，相信这将使得 Rapids 变得更好，期待与你在 Beta Test 中的会面。感谢所有参与测试的玩家！
  <br>在 Alpha Test 中提供了较好反馈且有意愿参与下轮测试的玩家，我们已审慎地激活他们于 Beta Test 的优先访问权限。
  <br>同时，我们也将在 Beta Test 中以更低的要求提供更多的访问席位。

  <details>
    <summary>查看优先激活名单 (排名不分前后)</summary>

    该名单基于 `Alpha Test` 中的个人进度进行审批。
    <br>如有填写意见问卷，亦另遵个人意愿及意见参考价值进行审批。
    <br>此批次玩家将在 `Beta Test` 获得优先访问权限，除此之外，还将获得更高数值的新手武器以便快速跳过 Intro 阶段。

    - DragonKing
    - AnthoGScorp_
    - Jeng_Die
    - Fawn_Hua
    - Leaf_ll
    - DuanDuan86
    - Cutesansui
    - yan_sui
    - before_sakura
    - WaningMoon7312
    - AnkaGroay
    - Dxxxxx
    - Cytzis
    - AZES

  </details>


- 修复了部分情况下会导致本轮 `Tier` 未同步至结算信息预览的问题。（奖励正常）
- 修复了在怪物生成的极早期阶段可以被秒杀的问题。
- 现已开放 `熔铸` 功能：
    <br><img src="/rapids/rapids_img/updatelogs/20260626_attrup.png" loading="lazy">
  - 通过收集 `同类型` 且 **相同或更高** `品质` 的装备，可以提升目标装备的词条百分比。
  - 通过此途径进行的词条提升，至高可提升至 `95%`
- 正在开发 `拆解` 及 `升等` 功能，届时将可以通过：
  - 拆解低等级、低品质装备，收集通用 `装备材料`
  - 提升自己的核心装备 `装备等级` （受上限约束）
- 现在 `Essence` 怪物将随着副本内玩家总数获得生命值提升，每 `1` 人将增加 `10%` 的生命值。
- 修复了部分问题。
- 新增 `综合材料` 处理方法，现部分打造将支持多来源的材料，并依照它们各自的库存进行扣除。
  - `「风之形」套装部件` 打造之「精雕细琢」配方做出部分调整：
    - `风蚀晶簇`: 6x → **12x** 
    - 移除 36x `风蚀石核` 需求
    - 移除 256x `苔痕石片` 需求
    - 新增 **384x** `「峡谷」寻常材料` 需求

---

#### 2026/06/25

- 现已开放 `强化` 功能。
- 优化了装备后调整系统的部分底层功能，为登场做准备。
- 将通关机制更改为更可选择的模式，你在通关后除固定的经验和 `E` 外，将可以在新的等待房中自选奖励，并决定是否再入副本。
  - 作为初个版本，你现可选择 `材料` 作为通关奖励。基于通关 `Tier` 获得对应的材料，如为 `Marvelous` 则有概率获得 `「风之形」图纸`。
- 新增了「宝箱搜寻器」
- 优化了「即时性消息」的发送逻辑。现在如处于 UI 打开状态，则将不会再尝试发送即时性消息。
- 优化了 `QS` 的消息提示。


---

#### 2026/06/24

- 将「峡谷(踏察)」中的一个碎石更改为 `个人独享` 收集物，并新增了 `3` 个。 
- 修复了掉落判断异常的问题。
- 调整了打造「风之形」套装部件的材料需求，并增加了预览时库存物品的显示。
- 略微提升了局内特殊掉落获取上限：`4` → `5`
- 调整了普通材料掉落的等级增益倍率。
- 提升了「峡谷」中 `Elite` 怪物对应 `风蚀石核` 的基准掉率：`5%` → `10%`。
- 现在局内累计获得的普通掉落数量也将受数量限制，当达到 `120` 个后，将无法获取新的普通掉落。此举用以限制长时挂机。
  <br><span class="inline-tips">参考数值：大约相当于「峡谷(踏察)」内 `458` 综合累计击杀。</span>
- 你现可从「峡谷宝箱 Tier 1」中获取 `风蚀石核` 及 `强化石`
- 你现可打造「精雕细琢」级别的 `风之形` 套装部件。
- 降低了通过击杀 `风蚀尸核` 以获取对应等级的 `「风之形」图纸` 之概率。
- 修复了部分问题

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
- 为「峡谷」套装追加了部分套装效果。
- 补全了「风之形」套装效果。
- 你现可通过击杀 `风蚀尸核` 以概率获取对应等级的 `「风之形」图纸`。
- 你现可于打造台中打造 `「风之形」` 套装部件。
- 新增了单局内可获取的装备或图纸数量上限，以限制长时挂机。

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


<div class="divider" style="margin: 2em 0;">
  <span>以下为 内部测试 内容</span>
</div>

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
