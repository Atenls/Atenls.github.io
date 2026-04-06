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

---

<p style="color: #999;"> Rapids 2026</p>