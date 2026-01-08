# CONTRIBUTING —— 从零开始维护WIKI：Git与GitHub完全指南

## 📚 前言：什么是PR？

**PR（Pull Request，拉取请求）** 是向开源项目贡献代码或内容的标准方式。简单说，就是：
1. **复制**项目到自己的账户
2. **修改**内容
3. **请求**原项目接受你的修改

---

## 🚀 第一章：准备工作

### 1.1 注册GitHub账号
1. 访问 [GitHub官网](https://github.com)
2. 点击 "Sign up" 注册
3. 填写用户名、邮箱、密码
4. 完成邮箱验证

### 1.2 安装Git工具
根据你的系统选择：

**Windows用户：**
- 下载 [Git for Windows](https://gitforwindows.org/)
- 双击安装，全部选默认选项
- 安装完成后，在开始菜单找到 "Git Bash"

**Mac用户：**
- 打开终端（Terminal）
- 安装Homebrew：`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
- 通过brew安装Git：`brew install git`

**Linux用户（Ubuntu为例）：**
```bash
sudo apt update
sudo apt install git
```

### 1.3 配置Git（一次性设置）
打开终端或Git Bash，依次输入：

```bash
# 设置你的用户名（用你的GitHub用户名）
git config --global user.name "你的用户名"

# 设置你的邮箱（用你的GitHub注册邮箱）
git config --global user.email "你的邮箱@example.com"

# 让Git命令输出带颜色，更容易阅读
git config --global color.ui auto

# 检查配置是否成功
git config --list
```

---

## 🛠️ 第二章：Git基础操作

### 2.1 了解Git的三个区域
```
工作区 (Working Directory) → 暂存区 (Staging Area) → 仓库 (Repository)
     修改文件                   git add                git commit
```

### 2.2 常用Git命令速查表
| 命令 | 作用 | 示例 |
|------|------|------|
| `git clone` | 下载远程仓库到本地 | `git clone https://...` |
| `git status` | 查看文件状态 | `git status` |
| `git add` | 添加文件到暂存区 | `git add 文件名` |
| `git commit` | 提交更改 | `git commit -m "描述"` |
| `git push` | 上传到远程仓库 | `git push origin 分支名` |
| `git pull` | 下载远程更新 | `git pull origin 分支名` |
| `git branch` | 查看/创建分支 | `git branch 新分支名` |
| `git checkout` | 切换分支 | `git checkout 分支名` |

---

## 📝 第三章：实战贡献流程

### 3.1 第一步：Fork（复制）项目
1. 打开 `https://github.com/Atenls/Atenls.github.io`
2. 点击右上角的 **"Fork"** 按钮
3. 等待几秒，GitHub会创建一个属于你的副本

### 3.2 第二步：克隆到本地
```bash
# 进入你的GitHub，找到你Fork的项目
# 点击绿色的 "Code" 按钮，复制HTTPS链接

# 打开终端/Git Bash，执行：
git clone https://github.com/你的用户名/Atenls.github.io.git

# 进入项目文件夹
cd 知识库名
```

### 3.3 第三步：创建新分支
```bash
# 创建并切换到新分支（分支名要有意义）
git checkout -b add-new-content

# 查看当前分支（前面带*号的是当前分支）
git branch
```

### 3.4 第四步：修改内容
#### 使用合适的编辑器：
- **VS Code**（推荐）：免费、强大
- **Cursor**：基于 VSCode 的AI编辑器
- **Typora**：优秀的Markdown编辑器
- **记事本**：也可用，但功能简单

#### Markdown基础语法：
```markdown
# 一级标题
## 二级标题
**加粗文本** *斜体文本*
- 列表项1
- 列表项2

[链接文字](https://地址)
![图片描述](图片地址)

> 引用块
```

需要注意：DP WIKI 基于 Docsify 进行文档生成，因此请勿使用 Docsify 不支持的 Markdown 语法。<br />同时，图片需要使用可靠的图床进行托管。

### 3.5 第五步：提交更改
```bash
# 1. 查看修改了哪些文件
git status

# 2. 添加所有修改的文件到暂存区
git add .

# 3. 提交更改（描述要清晰！）
git commit -m "添加了新内容：Git入门指南"

# 4. 推送到你的GitHub仓库
git push origin add-new-content
```

---

## 🔄 第四章：发起Pull Request

### 4.1 在GitHub上操作
1. 访问 **你的GitHub仓库页面**
2. 你会看到提示：`add-new-content had recent pushes`
3. 点击 **"Compare & pull request"** 按钮

### 4.2 填写PR信息
**标题格式：**
```
[类型] 简短描述
```
例如：
- `[文档] 添加Git入门指南`
- `[修复] 修正文档中的错别字`
- `[新增] 添加Python教程章节`

**描述模板：**
```markdown
## 修改说明

- 添加了Git入门教程
- 修正了第3章节的格式问题
- 补充了常见问题解答

## 关联 issue
（如果有）解决 #123

## 检查清单
- [ ] 我已阅读贡献指南
- [ ] 我的修改符合项目规范
- [ ] 我已测试过我的修改
```

### 4.3 提交并等待审核
1. 点击 **"Create pull request"**
2. 等待项目维护者审查
3. 根据反馈进行修改（如有需要）

---

## 🧩 第五章：处理反馈和更新

### 5.1 如果维护者要求修改
```bash
# 1. 回到你的本地分支
git checkout add-new-content

# 2. 修改文件...

# 3. 再次提交
git add .
git commit -m "根据反馈修改了..."

# 4. 推送到远程（会自动更新PR）
git push origin add-new-content
```

### 5.2 如果原项目有更新
```bash
# 1. 添加上游仓库（只需一次）
git remote add upstream https://github.com/Atenls/Atenls.github.io.git.git

# 2. 拉取上游更新
git fetch upstream

# 3. 合并到你的分支
git checkout main
git merge upstream/main

# 4. 更新你的分支
git checkout add-new-content
git merge main
```

---

## 💡 第六章：最佳实践与建议

### 6.1 提交信息规范
- **使用祈使句**：`"添加..."` 而不是 `"添加了..."`
- **首字母大写**：`"Fix typo"` 而不是 `"fix typo"`
- **长度限制**：标题不超过50字符，正文每行72字符

### 6.2 分支命名约定
```
类型/简短描述
```
- `docs/add-tutorial` - 文档相关
- `fix/typo-in-readme` - 修复错误
- `feature/new-section` - 新功能

### 6.3 贡献前的检查
1. ✅ 阅读项目的 `CONTRIBUTING.md`
2. ✅ 查看 `README.md` 了解项目
3. ✅ 搜索现有issue，避免重复工作
4. ✅ 从小处开始，先解决简单的issue

### 6.4 常见问题解决
```bash
# 撤销最后一次提交
git reset --soft HEAD~1

# 撤销对某个文件的修改
git checkout -- 文件名

# 查看提交历史
git log --oneline
```

---

## 🎯 第七章：完整流程示例

假设要为"Awesome-Knowledge"项目添加内容：

```bash
# 1. Fork项目（在GitHub页面操作）

# 2. 克隆到本地
git clone https://github.com/你的用户名/Atenls.github.io.git.git
cd dp_wiki

# 3. 创建分支（假设你要新增 add-git-tutorial 分支）
git checkout -b docs/add-git-tutorial

# 4. 创建新文件
echo "# Git完全入门指南" > git-tutorial.md

# 5. 编辑文件（用VS Code打开）
code git-tutorial.md

# 6. 提交更改
git add git-tutorial.md
git commit -m "docs: 添加Git完全入门指南"

# 7. 推送到GitHub
git push origin docs/add-git-tutorial

# 8. 在GitHub页面发起PR

# 9. 后续更新，添加上游项目
git remote add upstream https://github.com/Atenls/Atenls.github.io.git.git
... 参考 5.2 内容
```

---

## 📞 第八章：获取帮助

### 遇到问题怎么办？
1. **查阅文档**：`git --help` 或 `git 命令 --help`
2. **搜索引擎**：错误信息 + "git" 关键词
3. **社区求助**：
   - [GitHub Community Forum](https://github.community/)
   - [Stack Overflow](https://stackoverflow.com/)（使用git标签）
4. **项目沟通渠道**：查看项目README中的联系方式

### 学习资源推荐
- **交互式学习**：[Learn Git Branching](https://learngitbranching.js.org/)
- **官方教程**：[Git官方文档](https://git-scm.com/doc)
- **中文教程**：[廖雪峰的Git教程](https://www.liaoxuefeng.com/wiki/896043488029600)

---

## 🎉 第九章：成功贡献后

1. **庆祝你的第一次PR！** 🎊
2. 关注PR状态，学习审查意见
3. 将原项目设为星标（Star），关注更新
4. 考虑加入项目的其他贡献活动

### 进阶学习方向
```bash
# Git高级功能
git rebase        # 变基，整理提交历史
git stash         # 暂存当前修改
git cherry-pick   # 选择特定提交
git bisect        # 二分查找问题提交
```

---

## 📋 快速检查清单

开始前：
- [ ] GitHub账号已注册
- [ ] Git已安装并配置
- [ ] 已Fork目标项目
- [ ] 已克隆到本地

提交PR前：
- [ ] 创建了有意义的分支名
- [ ] 遵循了项目规范
- [ ] 提交信息清晰明确
- [ ] 已推送到自己的仓库

发起PR时：
- [ ] PR标题符合规范
- [ ] PR描述详细完整
- [ ] 关联了相关issue（如果有）
- [ ] 确认了检查清单

---

**记住：每个开源贡献者都是从第一次PR开始的！开源社区欢迎每一位认真贡献的朋友。** 

遇到困难时不要灰心，这是学习过程中的正常部分。每一次尝试都会让你更加熟练。祝你在开源贡献的道路上越走越远！✨

**有问题随时可以回来查阅这份指南，或者向社区寻求帮助。**