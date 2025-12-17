# Git 上传指南 - 《指令重塑：从"对话"到"驾驭"的 AI 提示词工程实战》

## ✅ 已完成的步骤

1. ✅ 初始化 Git 仓库
2. ✅ 创建 README.md（专业的项目说明文档）
3. ✅ 创建 .gitignore（忽略临时文件）
4. ✅ 创建 LICENSE（MIT 开源协议）
5. ✅ 添加所有课程文件到 Git
6. ✅ 创建首次提交

---

## 🚀 接下来的步骤

### 方案 A：上传到 GitHub（推荐）

#### 1. 在 GitHub 创建新仓库

访问：https://github.com/new

填写信息：

- **Repository name**: `ai-prompt-engineering-course` 或 `从对话到驾驭`
- **Description**: `《指令重塑：从"对话"到"驾驭"的 AI 提示词工程实战》- 面向初学者的系统化 Prompt Engineering 课程`
- **Public/Private**: 选择 Public（公开）或 Private（私有）
- ⚠️ **不要勾选** "Add a README file"、"Add .gitignore"、"Choose a license"（我们已经创建了）

#### 2. 关联远程仓库并推送

创建仓库后，GitHub 会显示推送命令。在当前目录执行：

```bash
# 添加远程仓库（替换成你的 GitHub 用户名）
git remote add origin https://github.com/你的用户名/仓库名.git

# 或者使用 SSH（如果配置了 SSH key）
git remote add origin git@github.com:你的用户名/仓库名.git

# 推送到 GitHub
git branch -M main
git push -u origin main
```

#### 3. 验证上传成功

访问你的 GitHub 仓库页面，应该能看到：

- ✅ 完整的 README.md 展示
- ✅ 所有 10 个课程文件
- ✅ MIT License 标记

---

### 方案 B：上传到 Gitee（国内备选）

如果 GitHub 访问较慢，可以使用 Gitee：

#### 1. 在 Gitee 创建新仓库

访问：https://gitee.com/projects/new

填写类似信息

#### 2. 关联并推送

```bash
git remote add origin https://gitee.com/你的用户名/仓库名.git
git push -u origin master
```

---

### 方案 C：同时推送到多个平台

```bash
# 添加 GitHub 远程仓库
git remote add github https://github.com/你的用户名/仓库名.git

# 添加 Gitee 远程仓库
git remote add gitee https://gitee.com/你的用户名/仓库名.git

# 分别推送
git push github main
git push gitee master
```

---

## 📝 后续更新课程的命令

当你修改了课程内容后：

```bash
# 查看修改了哪些文件
git status

# 添加所有修改的文件
git add .

# 创建提交（描述你的修改）
git commit -m "📝 更新 Class X: 添加新案例"

# 推送到远程仓库
git push
```

---

## 💡 常用 Git 命令速查

| 命令                   | 说明               |
| ---------------------- | ------------------ |
| `git status`           | 查看当前状态       |
| `git add .`            | 添加所有修改       |
| `git commit -m "消息"` | 创建提交           |
| `git push`             | 推送到远程仓库     |
| `git pull`             | 从远程仓库拉取更新 |
| `git log --oneline`    | 查看提交历史       |
| `git remote -v`        | 查看远程仓库地址   |

---

## 🎨 推荐的 Commit 消息格式

使用 emoji 让提交记录更清晰：

```
🎉 初始提交
✨ 新增功能
📝 更新文档
🐛 修复错误
🎨 改进格式
♻️ 重构代码
🔥 删除代码
```

---

## ❓ 常见问题

### Q1: 如何修改仓库名称？

在 GitHub/Gitee 的仓库设置中，找到 "Repository name" 修改即可。

### Q2: 如何让 README 中的链接正常工作？

推送到 GitHub 后，相对路径链接会自动生效。

### Q3: 如何添加贡献者？

在 GitHub 仓库设置 → Collaborators 中添加。

### Q4: 推送时要求输入密码怎么办？

- 方案 1: 使用 Personal Access Token 代替密码
- 方案 2: 配置 SSH Key（推荐）

---

## 🌟 下一步建议

1. **添加 Topics 标签**：在 GitHub 仓库页面添加标签，如：

   - `prompt-engineering`
   - `ai`
   - `chatgpt`
   - `tutorial`
   - `chinese`

2. **完善 README**：可以添加：

   - 课程演示 GIF
   - 学员反馈
   - 常见问题 FAQ

3. **启用 GitHub Pages**（可选）：
   将课程变成在线网站

4. **添加 Star 徽章**：
   在 README 中展示 Star 数量

---

**准备好了吗？现在就去创建你的 GitHub 仓库，然后运行推送命令吧！** 🚀
