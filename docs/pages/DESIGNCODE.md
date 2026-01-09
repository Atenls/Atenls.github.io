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

# Design Code

<p style="border-left: 5px solid #3c547cff; color: #5777afff; padding-left: 10px;">
本文档旨在为所有志愿参与WIKI构建的玩家提供统一的设计原则、规范和最佳实践。<br>
通过明确的设计指导，我们希望能够确保产品在用户体验和视觉表现上保持一致，同时提升设计效率和质量。
</p>

<p style="border-left: 5px solid #745691ff; color: #826199ff; padding-left: 10px;">
文档最后更新于 2026/01/09 20:55<br>
贡献者: <span class="dptag tag-purple">Atenls</span>
</p>

<hr>

<div class="cards-container">
<div class="cards">

<a href="#/pages/DESIGNCODE?id=_1-标题的设计" class="card acards">
标题的设计</a>
<a href="#/pages/DESIGNCODE?id=_2-内容的设计" class="card acards">
内容的设计</a>

</div>

</div>

---

## 1. 标题的设计

### 1.1 标题的格式

标题及其内容如有明确的前后顺序，应遵从 `1.` - `1.1` - `1.1.1` 。如无明确，应不用或仅用 `1.` - `2.` - `3.` 。（中文亦可）

参考：
```MarkDown
## 1. 标题
### 1.1 子标题
#### 1.1.1 子子标题

或
## ANOTHERTITLE

### 1. SUBTITLE 1
### 2. SUBTITLE 2

## Another Title

### 1. Subtitle 1

```

### 1.2 颜色及样式

如无特别需要，在MarkDown中，标题的样式应保持一致。仅使用默认MarkDown渲染样式，不添加颜色或特殊效果。

参考：
#### 1. 标题
```MarkDown
#### 1. 标题
```

---

如有特别需要，请使用HTML标签。

参考：
#### 1. <span style="color: #eeaa10">金色标题</span>
```MarkDown
#### 1. <span style="color: #eeaa10">金色标题</span>
```


---


## 2. 内容的设计

通常的内容，应遵从 MarkDown 及 Docsify 的默认格式。以确保内容的可阅读性、易用性并降低学习成本。<br>
详情请查看 [Docsify 官方文档](https://docsify.js.org/#/zh-cn/helpers)


### 2.1 字段的设计

#### 2.1.1 字段的格式

字段格式应保持一致。如无特别需要，请使用 MarkDown 默认的字段格式。<br>
Docsify 的渲染策略与其他 MarkDown 有所不同，在源文稿中，单次换行将不会被渲染为换行，而多行换行将被渲染成更高间隔的空行。<br>
如需要通常的换行，请使用 `<br>` 。<br>
空格的使用可以使得观感更佳，在所有字段中，当混合物品、技能、效果或多种语言时，请使用空格来进行必要的隔断。


#### 2.1.2 字段颜色及样式

字段颜色及样式应保持一致。如无特别需要，请使用 MarkDown 默认的字段颜色及样式。<br>
在需要**强调的内容**时，通过 `**` （双星号）进行，并确保只强调重点内容，尽可能避免加粗大部分字段的情况。<br>
如需要强调的内容并非概念，而是物品或类似的可交互实体（如技能、怪物），请使用 <code>`</code> （飘号键）进行。

参考：

这是**需要加粗的内容**，不要对整段文稿使用加粗。<br>
这是一个 `物品`，不要对整段文稿使用加粗或强调。

```MarkDown
这是**需要加粗的内容**，不要对整段文稿使用加粗。<br>
这是一个 `物品`，不要对整段文稿使用加粗或强调。

```



### 2.2 描述的设计

#### 2.2.1 默认的描述参考

Docsify 提供了三种描述格式：

> 默认绿边引用，语法为 `>`
```MarkDown
> 默认绿边引用
```
通常使用于正向的提示或描述性内容

---

!> 警告框引用，语法为 `!>`
```MarkDown
!> 警告框引用
```
用于警告性、重要性内容

---

?> 全绿框提示性引用，语法为 `?>`
```MarkDown
?> 全绿框提示性引用
```
通常用于长篇幅的答疑、其他地方的引用或描述性内容

---

#### 2.2.2 自定义的描述参考

除了默认的格式外，对于大部分更纯粹的描述文字，更推荐使用HTML标签自定义样式。<br>
通过 `border-left: 4px solid #bbb; color: #999; padding-left: 10px;` 来构建一个灰色的块状引用。<br>
你可以将其置于 `<p>` 或 `<span>` 中：

参考：
<p style="border-left: 4px solid #bbb; color: #999; padding-left: 10px;">这是灰色的块状引用</p>

<p style="border-left: 4px solid #bbb; color: #999; padding-left: 10px;">这是一个多行的灰色的块状引用<br>这里应该有一些内容<br>这里应该有一些内容<br>这里应该有一些内容</p>

```MarkDown
<p style="border-left: 4px solid #bbb; color: #999; padding-left: 10px;">这是灰色的块状引用</p>
<p style="border-left: 4px solid #bbb; color: #999; padding-left: 10px;">这是一个多行的灰色的块状引用<br>这里应该有一些内容<br>这里应该有一些内容<br>这里应该有一些内容</p>
```

实际上，并不限定于灰色，你可以根据需要<span style="color: transparent; background: linear-gradient(135deg, #6658e9ff, #e77fdbff) text; font-weight: bold;">自定义颜色</span>，只要确保颜色与背景色符合审美即可。


### 2.3 列表的设计

列表的格式应保持一致。如无特别需要，请使用 MarkDown 默认的列表格式或表格。<br>
列表通常使用于掉落列表、需求列表，如：
- 怪物掉落
- 图纸需求
- 多渠道
- 类似的多个项目并存的情况

如无特别需要，请勿在字段中连续使用空格隔断或其他内容来表达列表项。

#### 2.3.1 实践内容参考：

---

##### 正确实例：
掉落素材/点数：
- `林间猫尾`
- 未知装备 / 未知武器
- 林地区域探索点数 (Rep)

<span style="border-left: 4px solid #aaa; color: #999; padding-left: 10px;">由于未知武器/装备基本都会掉落，所以后文只写出有用处的材料。同时，含 `特殊标记` 的素材为悬赏任务所需之材料。</span>

---

##### 错误实例：

·掉落素材/点数：**[林间猫尾]**、[未知装备]**、**[未知武器]、林地区域探索点数（在后文中，由于未知武器/装备基本都会掉落，所以后文只写出有用处的材料。同时，将对AP任务所需求的素材进行 **[]并黑色加粗**）

---

#### 2.3.2 格式参考：


<div class="cards-container">
<div class="cards">

<div class="card" style="width: 450px;">

**有序列表：**

1. 列表项 1
2. 列表项 2
3. 列表项 3
4. ...

```MarkDown
1. 列表项 1
2. 列表项 2
3. 列表项 3
4. ...
```

</div>

<div class="card" style="width: 450px;">

**无序列表：**

- 列表项 1
- 列表项 2
- 列表项 3
- ...

```MarkDown
无序列表：
- 列表项 1
- 列表项 2
- 列表项 3
- ...
```

</div>
</div>

<div class="cards">
<div class="card" style="width: 450px;">

**表格：**

| 表头 1 | 表头 2 | 表头 3 |
| ------ | ------ | ------ |
| 列表项 1 | 列表项 2 | 列表项 3 |

```MarkDown
| 表头 1 | 表头 2 | 表头 3 |
| ------ | ------ | ------ |
| 列表项 1 | 列表项 2 | 列表项 3 |
```

</div>

<div class="card" style="width: 450px;">

**另一种表格样式：**

| 表头 1 | 表头 2 | 表头 3 |
| ------ | ------ | ------ |
| 列表项 1 | |
| 列表项 2 | |
| 列表项 3 | |

```MarkDown
| 表头 1 | 表头 2 | 表头 3 |
| ------ | ------ | ------ |
| 列表项 1 | |
| 列表项 2 | |
| 列表项 3 | |
```

</div>

</div>
</div>