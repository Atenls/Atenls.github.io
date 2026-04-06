<style>
.dptag {
  color: #f0f0f0;
  background-color: #538aec;
  text-shadow: 0.5px 1px 0.5px rgba(0, 0, 0, 0.25);
  padding: 2px 3px;
  margin: 0 2px;
  border-radius: 2px;
  font-family: 等线;
  font-weight: 500;
}

* {
  --force-text-fill-color: #6080b6;
  font-family: 'SFPro', 'PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', 'WenQuanYi Micro Hei', 'Helvetica Neue', 'Helvetica', 'Arial', 'sans-serif';
}

.tag-gold {
  background: #eeaa10;
  color: #efffef;
}

.tag-yellow {
  background: #efbe40;
  color: #efffef;
}

.tag-green {
  background: #279027;
}

.tag-red {
  background: #ef8080;
  color: #ffffff;
}

.tag-red-blue {
  background: linear-gradient(135deg,#ef8080,#538aec);
  color: #f8ffef;
}

.tag-pink-gold {
  background: linear-gradient(135deg,#ff9b1a, #ff80f0);
  color: #f8ffef;
}

.tag-purple {
  background: #7a31aa;
}

.tag-gray {
  background: #989899;
}

.tag-cyan {
  background: #9999cc;
}

.cards-container {
  display: flex;
  max-width: 1000px;
  flex-direction: column;
  gap: 20px;
}

.cards {
  display: flex;
  gap: 20px;
}

.card {
  background: transparent;
  font-size: 15px; 
  border-radius: 8px;
  min-width: 150px;
  min-height: 100px;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15);
  text-shadow: 0.5px 0.5px 0.5px rgba(60, 60, 60, 0.05); 
  padding: 20px;
  transition: all 0.3s ease;
  overflow: hidden;
}

.acards {
  text-align: center;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  text-decoration: none; 
  color: transparent; 
  --force-text-fill-color: transparent;
  background: linear-gradient(135deg, oklch(0.7838 0.1381 225), oklch(0.6973 0.247 335)) text; 
  text-shadow: 0 0 1px oklch(0.8309 0.0197 312.88 / 0.2);  
  font-size: 20px; 
  font-weight: bold;
}

.markdown-section a {
    color: var(--force-text-fill-color, --theme-color, #538aec)
}

.card:hover {
  box-shadow: 0 12px 30px rgba(0, 0, 0, 0.4);
  color: linear-gradient(135deg, #91e5f2, #f1c4eb);
}


@media (max-width: 768px) {
  .cards {
    flex-direction: row;
    flex-wrap: wrap;
  }

  .card {
    width: 100%;
  }

}

</style>

# Rapids - 激流

<p style="border-left: 4px solid #ccc; color: #aaa; padding-left: 10px;">Rapids 取名灵感自 Intel 4th Xeon Scalable (Sapphire Rapids) 及此后的架构命名</p>
<p style="border-left: 5px solid #745691ff; color: #826199ff; padding-left: 10px; font-family: 'SFPro', 'PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', 'WenQuanYi Micro Hei', 'Helvetica Neue', 'Helvetica', 'Arial', 'sans-serif';">
目前的测试阶段: <span class="dptag tag-purple" style="font-family: CONSOLA">Alpha</span>
</p>

## 简介

Rapids 是一个基于 Minecraft `1.21.11` 的 Prototype 服务器。<br>
其核心内容为 `Atenls` 打造的现代 `RPG` 服务器。<br>
Rapids 的诞生旨在试验前沿的技术，创造更好的游戏体验。<br>
也因此，除反响极其良好外，它将不会使用 LTE 运营模式，它的正式运营预期寿命不会超过 180 天。

---

## 开放性

Rapids 目前暂且处于早期测试阶段，所有玩家通过申请准入。<br>


### 对于 DP 玩家

所有 `DP4` 玩家在达到 `100` AccountValue 后，<br>
可通过提交 `32LT` 押金以申请核实 `Rapids Alpha 测试资格`，在通过后，你将获准在 Alpha 测试期间进入 Rapids。<br>
该押金将在测试期结束后退回。

### 对于其他玩家

很遗憾，我们暂时不接受非 DP 玩家的申请。

---

## Alpha 测试

Rapids 的 Alpha 测试大约将在 `2026/05` 开始。<br>
此时将处于极早期的测试阶段，游戏体验或将不如预期，敬请悉知。<br>
测试期间，Rapids 将会处于 Frequent Update 状态，并针对系统、生物、玩家交互等内容进行测试。<br>
或将出现较多不可知的问题，并引发较差的游戏体验，我将在收到反馈后尽可能早的时间内完成修复。<br>
测试期间结束后，如存在下一轮测试，较好表现的玩家将自动获得测试资格。


---

## 技术优势

### 性能

Rapids 的核心系统将由 Atenls 完全自主编写，通过于 `DP4` 积攒的多项成功优化经验，及高版本更优良的性能、特性。<br>
在面对极高数量实体、长链复杂判断等场景时，仍能保持较高的性能表现。

### 体验

Rapids 的游戏体验完全由 Atenls 设计，你将能获得一如既往的全局细节把控、无间隙的多系统联动、一以贯之的排版设计。<br>
得益于完全自主开发的系统，Rapids 可以轻松地处理所有信息。你在游戏过程中将不会收到任何不应存在的错误提示、系统日志。

### 系统

Rapids 将沿袭部分 DP 的核心系统，也有新开发的独有系统。

- **战斗**：<br>仍将以 ZA 为核心，简洁、易用、快速。
- **物品**：<br>初步考虑仍将沿用 `仓库` 存储大宗材料，`QS` 存储少量可供快捷取用的物品。<br>也可能转为全 `QS` 模式。
- **地图**：<br>为追求多场景的可控化，Rapids 将**不再采用** `大世界` 模式，而是转变为 `箱庭` 副本模式。<br>
这也使得地图探索更加易于上手，也有助于玩家于统一的主城交流。
- **其他**：<br>多个自主开发的子系统有部分将因版本更迭被放弃，少部分仍将发光发热。<br>及 Rapids 在开发过程中也有独有的子系统。

---

## Q&A

1. **Rapids 是 DP 的续作 (DP V) 吗？**<br>
不是，Rapids 是一个 Prototype 测试服务器。但它所产生的技术、经验将在未来作为 DP V 的基础。

2. **为什么不直接全量公开测试？**<br>
测试服务器的测试目的在于验证技术、体验、系统，而不是作为 DP V 前作的全量公开测试。<br>

3. **DP4 玩家是否可以直接进入测试服务器？**<br>
测试服务器不直接对 DP4 玩家开放，但 DP4 玩家可以通过申请获得测试资格。<br>
高 AccountValue 玩家可以通过信任担保来让亲友获得测试资格。

4. **测试的要求太高了，能不能降低一点？**<br>
目前处于极早期的测试阶段，注定无法承载太多的玩家。因此要求较高，但在下一轮测试，要求将会放宽。

5. **测试时间将会是多久？**<br>
视乎具体 Rapids 的进程而定。待到我们认为开放的时机成熟，将会转入正式公开测试 或 正式运营。

6. **测试结束会删档吗？测试玩家有什么奖励？**<br>
测试结束会删档。表现优异的测试玩家将在正式服获得称号、部分起步物资等奖励。

7. **Rapids 会继承 DP4 的某些内容吗？**<br>
不会，Rapids 完全独立于 DP4。

---

<p style="color: #999;"> Rapids —— 开发测试内容不代表实际品质</p>