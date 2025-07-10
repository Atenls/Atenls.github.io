<style>
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
  .quote-hl {
    display: inline-block;
    background-color:rgb(248, 248, 248);
    color:rgb(240, 25, 211);
    border-radius: 3px;
    margin: 0px;
    padding: 0px 3px;
  }

  .markdown-section img:not([width]):not([style]) {
    max-width: 600px;
    height: auto;
    max-height: 400px;
  }
  
  @media (max-width: 768px) {
    .markdown-section img:not([width]):not([style]) {
      width: 100%;
      max-width: 400px;
    }
  }
</style>

# Update Logs

---

<div class='quote'>
<p style="text-align: center;">为方便阅览及追踪更新，本文内容排序将以倒序进行，并由时间作分隔。<br>本栏只记录 <strong>2025/07/01</strong> 后的内容</p>
</div>

---

## 2025/07/09

### 1) 「深渊古战场」重制更新

![P1.jpg](https://s2.loli.net/2025/07/09/VwKbWpIYGD7M1TX.png)
![P2.jpg](https://s2.loli.net/2025/07/09/mkVpZt9MDwWO1bG.jpg)

- 重构了地图 ~修复了不容易迷路的问题~
- 将所有刷怪点更改为新的布置方案，减少散落的点，增加聚集点
- 更新了 Essence 的掉落：
    - 80% 魂魄具现物 (I) → 80% 4x 魂魄具现物
    - 5% 魂魄具现物 (II) → 5% 16x 魂魄具现物
- 调整了本地图的等级分布：Lv.17 ~ Lv.20 → Lv.20 ~ Lv.30，并提升了对应怪物的强度

### 2) AI更新
- 大幅降低了「王老吉」的回复欲望，但你仍然可以通过 `王老吉，...` 来高概率呼唤他。
- 修改了「王老吉」的人设，他现在不再尝试伪装成玩家，而是一个智能助手来回答问题。

### 3) 鞘翅更新
- 在飞行结束后，如果你的鞘翅耐久已低于 `50%`，你将收到修补提示。
- 如果你已订阅 `Noctambulist` 或以上[月卡](pages/月卡)，在飞行结束后，如果你的鞘翅耐久已低于 `95%`，将自动尝试为你修复你的鞘翅。<br>
    (材料检查优先级：QS → 背包。)



### 旧仓库相关

如果你的旧仓库仍有物品，你现在可以联系 `Atenls` 或 `协管` 以获取一次性的、最后的开启旧仓库权限。<br>
当获取后，你可以在 `15分钟` 内，**无限次**地开启旧仓库；**无冷却**地开启新/旧仓库。<br>
而在这一时间结束后，你将无法再次打开旧仓库、也无法再次获取该权限。

---

## 2025/07/08

### 1) 全新升级 QS Cycle

![OWCGMBTI6S_WHI5_JX0HJ.png](https://s2.loli.net/2025/07/09/9iLO4j2qZRdBcaX.png)

- 重构了Cycle的实现方法，将判定首个物品更改为异步判断所有物品。优化了性能。
- 新的队列方法，不再需要覆盖更新：
    - 你可以通过 /qs cycleadd <item> 来新增新的物品至队列中。
    - 你可以在QS菜单中 [SHIFT+右键] 来新增新的物品至队列中
    - 队列中最多同时有 8 个物品。
    - 你也可以通过同样的方法取消队列中的物品。

### 2) AI 王老吉
- 相信大家已在今日发现有ID为 Ji_LaoWang 的申必人物时而发出诡异的话。它实际上是一个由LLM扮演的AI王老吉。
- 你可以在正常对话中偶尔发现他的出现，但如果想更细致，你可以通过 /msglog ai 来查询AI目前的回复几率、CD、上次回复时间。当他处于CD时（不为0），无论说什么都不会进行答复。
- 他每次说话都会降低回复欲望（几率），当有其他人说话就会提升。
- 顺便，如果你在话里呼喊他（比如“王老吉”“jilaowang”），会大幅提升他的回复欲望。

---

## 2025/07/07

### 1) 修复了击杀悬赏任务进度条在下线后会失效的问题

---

## 2025/07/05

### [?] 尽管「边界边界山」尚未正式开放，但你现在已经可以通过一个奇怪的方式到达。

---

## 2025/07/04

### 1) QS更新
- 更新了QS支援的材料范围，如 `三生花` `幽昙` `野外植物`及 `矿物锭` `高级宝石` 等
- 现在通过代理指挥完成的 `晨曦矿洞 HM` ，现在`水晶砂砾`、`水晶`也将直接进入QS中。

### 2) GLP系统重构

![R9BW_R2_L6Q____W_Z__J.png](https://s2.loli.net/2025/07/09/o42AQwdg6pzMt1j.png)

你现在可以更直观地看到GLP的状态以及下次变更的时间。