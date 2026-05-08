<style>
  * {
    font-family: 'PingFang SC', 'SF Pro', 'Inter', 'Hiragino Sans GB', '等线', 'Microsoft YaHei', '微软雅黑', 'Helvetica Neue', 'Helvetica', 'Arial', 'sans-serif';
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

  .tooltip {
    position: relative;
    cursor: pointer;
  }

  .tooltip .tooltip-text {
    visibility: hidden;
    padding: 8px;
    border-radius: 10px;
    position: absolute;
    z-index: 1;
    opacity: 0;
    transition: opacity 0.35s;
    text-shadow: 0.5px 0.5px 1px rgba(0, 0, 0, 0.25);
  }

  .tooltip-top .tooltip-text {
    bottom: 50%;
    left: 50%;
    transform: translateX(-50%);
    font-size: 48px;
  }

  .tooltip-top .tooltip-text::after {
    top: 100%;
    left: 50%;
    transform: translateX(-50%);
    border-color: white transparent transparent transparent;
  }

  .tooltip:hover .tooltip-text {
    visibility: visible;
    color: #555;
    opacity: 1;
  }

  .redbox {
    background: #fdf4f4;
    color: #85553e;
    box-shadow: 0 0 6px #441313a0;
    border-radius: 18px;
    font-size: 20px;
    font-weight: 600;
    text-align: center;
    padding: 20px;
    margin: 0px;
  }

  .greenbox {
    background: #f4fdf7;
    color: #3e854f;
    border: 1px solid #40924e;
    border-radius: 18px;
    font-size: 20px;
    font-weight: 600;
    text-align: center;
    padding: 20px;
    margin: 0px;
  }

  .bluebox {
    background: #f2faff;
    color: #466fa1;
    border: 1px solid #5b9abe;
    border-radius: 18px;
    font-size: 20px;
    font-weight: 600;
    text-align: center;
    padding: 20px;
    margin: 0px;
  }

  .yellowbox {
    background: #fff9f1;
    color: #c5985c;
    border: 1px solid #cfae8f;
    border-radius: 18px;
    font-size: 20px;
    font-weight: 600;
    text-align: center;
    padding: 20px;
    margin: 0px;
  }

  .quote-hl {
    display: inline-block;
    background-color:rgb(248, 248, 248);
    color:rgb(240, 25, 211);
    border-radius: 3px;
    margin: 3px;
    padding: 0px 3px;
  }

  .markdown-section img:not([width]):not([style]) {
    max-width: 600px;
    height: auto;
    max-height: 400px;
    border-radius: 8px;
    box-shadow: 0 0 4px rgba(0,0,0,0.25);
    overflow: hidden;
  }

  .markdown-section h4 {
    margin: 0.6rem 0;
  }

  .markdown-section figure, .markdown-section p {
    margin: 0;
  }

  .little-tips {
    max-width: 360px;
    padding: 1em;
    box-shadow: 0 0 4px #3f9c4380;
    background: #f8fffa;
    border-radius: 6px;
    font-size: 14px;
    margin: 8px 0;
    display: flex;
    gap: 1em;
    align-items: center;
  }

  .little-tips-blue {
    box-shadow: 0 0 4px #5d8cb6a0;
    background: #f7fcff;
  }
  
  .little-tips-purple {
    box-shadow: 0 0 4px #a45db6a0;
    background: #fef7ff;
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

  .sha {
    font-size: 14px;
    color: #aaa;
  }

  .highlight-purple {
    font-weight: 600;
    color: rgba(0,0,0,0.75);
    padding: 0 4px;
    border-radius: 20px 20px 10px 10px; 
    background: linear-gradient(
      to bottom, 
      transparent, 
      transparent 30%, 
      rgba(228, 212, 248, 0.6) 50%, 
      rgba(192, 180, 220, 0.5) 100%
    );
  }

  details[open] {
    margin: 0 -1em;
    transition: margin 0.25s ease-in-out;
    background: rgba(200, 199, 224, 0.2);
    box-shadow: 0 0 8px rgba(0,0,0,0.25);
    padding: 0.5em 1.5em;
    border-radius: 2em;
    display: inline-block;
  }

  details {
    transition: margin 0.25s ease-in-out;
  }
  
  @media (max-width: 768px) {
    .markdown-section img:not([width]):not([style]) {
      width: 100%;
      max-width: 400px;
    }
  }
</style>


# DPMarket - 交易所玩家指南

DPMarket 是服务器的交易所 / 环球市场。<br>
你可以在这里出售材料、收购材料、购买别人上架的物品，也可以交易装备、带特殊属性的物品或其他非常见物品。<br>
市场的所有操作通过 UI 完成，无需指令。

---

## 快速开始

你可以在:

- 天泽港
- 晨曦港
- 元央城
- 格里佛斯城
- 傲林镇

找到交易所，通过点击木牌可以进入交易主菜单。

### 二级界面

主菜单里一般会有三个入口：

- **材料市场**：查看和交易标准材料。
- **交易**：查看自己的交易栏位、领取成交内容、取消未完成交易，或从空栏位创建新交易。
- **散货市场**：查看装备、特殊物品、其他非常见物品。

<img src="/pages/dp_img/market_main.png" loading="lazy"></img>

---

## 材料市场
材料市场用以交易标准材料，你可以在 `/dpitem` 来查看所有材料。

材料市场不是普通商店，而是类似订单市场：

- 有人挂卖单时，你可以购买最低价的卖单。
- 有人挂买单时，你可以把材料卖给最高价的买单。
- 同一种材料、同一种货币会合并显示，方便比较价格。
- 成交按价格优先、时间优先处理。

进入材料市场后，点击某个材料，会进入该材料的详情页。

<img src="/pages/dp_img/market_materials.png" loading="lazy"></img>


### 材料详情页

材料详情页可以做这些事：

- 调整本次想买入或卖出的数量。（左侧一列按钮）
- 切换货币类型。（右侧绿宝石）
- 查看当前材料的买单列表。（右上箱子）
- 查看当前材料的卖单列表。（右下箱子）
- 直接购买最低卖单。（蓝色玻璃板）
- 直接出售给最高买单。（粉色玻璃板）

<img src="/pages/dp_img/market_materials_detail.png" loading="lazy"></img>

如果没有买单或卖单，对应按钮可能不会显示。

### 买入材料

你可以用三种方式直接买材料：

- 在材料详情页点击“购入最低卖单”。
- 进入卖单列表，选择某个具体卖单购买。
- 创建一个买单，并等待其他玩家出售。

购买后，材料不会直接塞进背包，而是进入 **「交易」**。这样可以避免背包满导致物品丢失。

购买完成后，回到主菜单打开最中间的 **「交易」** (末影箱) 按钮。

点击带有“可领取”提示的交易，就可以领取买到的材料。

### 出售材料

你可以用三种方式卖材料：

- 在材料详情页点击“出售给最高买单”。
- 进入买单列表，选择某个具体买单出售。
- 创建一个卖单，并等待其他玩家购买。

如果成交成功，货币收益会进入 **「交易」** 等待领取。卖家所得会扣除市场税费。

---

## 撮合交易

### 创建材料买单

买单表示：「我愿意用某种价格收购这种材料。」<br>
创建买单时，市场会先冻结完整预算。如果订单没有完全成交，到期或取消后，未使用的货币会退回到你的 **「交易」** 里。

创建材料买单的方式是在 **「交易」** 里创建：

1. 打开 **「交易」** 。
2. 点击一个空白交易栏位。
3. 在自己的背包里点击想要交易的材料。
4. 在创建交易界面里把方向切换为买单。
5. 设置数量、单价、货币、截止时间和单次最低交易数量。
6. 点击中间的物品确认创建。

<img src="/pages/dp_img/market_emptyslot.png" loading="lazy"></img>

<details>
<summary style="color: #404248; font-weight: 700; margin-top: 0.5em;">详细图例</summary>

- **设置数量**:<br><img src="/pages/dp_img/market_createorder_setamount.png" loading="lazy"></img>
- **设置价格**:<br><img src="/pages/dp_img/market_createorder_setprice.png" loading="lazy"></img>
- **设置最小交易数量**:<br><img src="/pages/dp_img/market_createorder_setmintrade.png" loading="lazy"></img>
- **设置时间**:<br><img src="/pages/dp_img/market_createorder_settime.png" loading="lazy"></img>
- **设置方向**:<br><img src="/pages/dp_img/market_createorder_setside.png" loading="lazy"></img>
- **设置货币**:<br><img src="/pages/dp_img/market_createorder_setcurrency.png" loading="lazy"></img>

</details>

### 创建材料卖单

卖单表示：「我把这些材料托管到市场里，等待别人购买。」<br>
创建卖单时，市场会立刻从你的背包扣除对应材料并托管。订单到期或取消后，未卖出的材料会退回到 **「交易」**。

在 **「交易」** 里创建：

1. 打开 **「交易」**。
2. 点击空白交易栏位。
3. 在背包里点击要出售的材料。
4. 确认方向为卖单。
5. 设置数量、单价、货币、截止时间和单次最低交易数量。
6. 点击中间的物品确认上架。

<p style="
display: inline-block; background: #e8effdb0; box-shadow: 0 0 4px rgba(0,0,0,0.15); border-radius: 1em;
color: #4b4b50; padding: 0.5em 1em; margin: 1em -0.5em; font-weight: 500;
"><span style="color: #282930; font-weight: 700;">特别注意：</span><br>
物品单价为 1 个物品的价格，而非「最低交易数量」的价格。<br>
参考：如果你想将某材料以<span style="color: #282930; font-weight: 600;">「5000 dPe / 组」</span>的价格出售，应设置单价为 <span style="color: #282930; font-weight: 600;">5000/64 → 78</span> (4992/组)，而非 5000。
</p>

图例参考 同 **创建材料买单**。

---

## 散货市场

散货市场用于交易非常见物品，例如：

- 装备。
- 每日副本材料、箱子。
- 部分特殊材料。

如果同一种装备，但属性不同，仍会被视为不同物品。完全一致的散货会聚合显示，买家可以一次购买多个。

### 出售散货

在 **「交易」** 里创建：

1. 打开 **「交易」**。
2. 点击空白交易栏位。
3. 在背包里点击想出售的装备或特殊物品。
4. 如果它不是标准材料，会进入散货创建界面。
5. 设置单价、数量、货币、截止时间和单次最低购买数量。
6. 点击中间的物品确认上架。

散货**只支持卖单**，不支持玩家挂收购装备的买单。

### 购买散货

进入 **交易所**，点击 **散货市场**，再点击你想购买的物品。

在购买确认界面中可以：

- 调整购买数量。
- 查看单价。
- 查看购买总价。
- 查看可购买数量。
- 查看单次最低购买限制。
- 点击确认购买。

购买后，物品需要在 **「交易」** 里领取。

<img src="/pages/dp_img/market_equipment_detail.png" loading="lazy"></img>

---

## 进行中的交易

**「交易」** 是玩家最常用的界面。

这里可以看到：

- 正在出售的订单。
- 正在收购的订单。
- 已成交后可领取的内容。
- 取消或到期后可领取的退还内容。
- 空白交易栏位。

不同状态会用不同颜色或不同物品展示：

- 空白栏位：可以点击创建新交易。<br><img src="/pages/dp_img/market_emptyslot.png" loading="lazy"></img>
- 进行中：点击可取消订单并退回剩余内容。<br><img src="/pages/dp_img/market_trade_trading.png" loading="lazy"></img>
- 可领取：点击领取成交内容、收益或退还物。<br><img src="/pages/dp_img/market_trade_done.png" loading="lazy"></img>


---

## 领取物品和货币

成交后，市场不会直接把内容放进背包，而是先放入 **「交易」** 对应的可领取记录。<br>
这样做是为了防止：

- 背包满导致物品消失。
- 掉线时奖励发放失败。
- 交易过程中出现重复领取或刷物品。

然后点击带有“可领取”的项目。<br>
如果背包空间不足，领取会失败，记录会保留。清理背包后再领取即可。

## 货币说明

市场支持多种货币。你可以使用货币按钮切换对应的货币。

### 数值货币

目前仅支持 dPe

### 实体货币

目前仅支持 LegendaryToken

实体货币是背包里的物品货币，一个货币组可能由大面额和小面额组成：

购买时，系统会自动从背包扣除合适的货币物品。如果需要找零，找零会直接回到你的背包。

---

## 税费说明

市场成交时，税费从卖家的成交所得中扣除。

例如一笔交易总价是 `1000`，税率是 `5%`，卖家最终收到 `950`，税额是 `50`。

`月卡` 或 `Rank` 可以减免你的税率，两者并不叠加，以更低者优先。

税费只影响卖家所得，不会让买家额外多付。

## 截止时间和订单取消

创建订单时需要设置截止时间。

如果不输入时间，默认通常是 `3d`，也就是 3 天。服务器可能限制最短和最长挂单时间。

订单到期后：

- 未卖出的材料或散货会退回 **「交易」**。
- 买单未使用的冻结货币会退回 **「交易」**。
- 已成交内容仍然可以领取。

你也可以在 **「交易」** 中点击进行中的订单主动取消。取消后，剩余内容会进入 **「交易」** 等待领取。

## 单次最低交易数量

部分订单可能设置了“单次最低购买/出售数量”。

这个功能用于避免一个大订单被拆成很多很小的成交记录。

例如：

- 订单总量是 `640`。
- 单次最低是 `64`。
- 其他玩家每次至少要买或卖 `64` 个，除非订单剩余数量已经低于这个限制。

如果你交易的数量低于该订单限制，市场会提示无法成交。

---

## 常见问题

- **为什么我买到的物品没有直接进背包？**<br>
为了可靠性和防止背包满造成丢失，购买结果会进入 **「交易」** 。打开 **「交易」** 后点击可领取项目即可领取。

- **为什么创建买单时会立刻扣钱？**<br>
买单需要先冻结完整预算，这样别人卖给你时才能立即成交。未成交部分会在取消或过期后退回。

- **为什么创建卖单时物品被拿走了？**<br>
卖单需要先托管物品。这样买家付款后，市场才能保证物品一定存在，避免交易纠纷和复制问题。

- **为什么我的散货和别人看起来一样，却没有合并？**<br>
散货会比较完整 ItemStack。只要附魔、NBT、Lore、耐久、名字等数据不同，就会被视为不同物品。

- **为什么无法购买某个订单？**<br>
  可能原因包括：

  - 你的货币不足。
  - 背包里的实体货币不足或没有可用面额。
  - 购买数量低于订单的单次最低限制。
  - 订单已经被别人买走。
  - 你正在尝试购买自己的订单。

- **为什么卖出后收到的货币少于成交总价？**<br>
市场会从卖家所得中扣税。实际所得会在成交提示和 **「交易」** 领取内容中显示。

- **订单到期了怎么办？**<br>
到期订单会自动处理。未成交物品或未使用货币会进入 **「交易」** ，打开 **「交易」** 领取即可。<br>
但如果一个订单到期超过 14 天，而物资仍未领取，则将被销毁。



---