# Nobita Skills

> 这里收集了我日常使用 Claude Code 时开发的各类 Skill。

## 📚 Skills 列表

### [Draw.io 图表生成](./Draw.io图表生成/)

根据文本内容自动生成 draw.io 可直接导入的 XML 图表文件。

**支持类型：**
- 系统架构图
- 流程图
- 时序图
- 层次结构图
- 思维导图
- 网络拓扑图

**使用方式：** 触发词 `drawio`

**特色功能：**
- 内置各大厂商图标库（Kubernetes、阿里云、AWS、Azure、GCP 等）
- 自动布局与配色
- 一键导入 draw.io 编辑

### [Git 提交](./git-commit/)

智能生成结构化 commit message 并提交代码。

**使用方式：** `/git-commit` 或说"提交代码"、"commit"、"提交一下"

**特色功能：**
- 自动分析变更内容，生成三段式 commit message（概述 + 文件树 + 详细说明）
- 从 git log 学习项目的类型前缀和分隔符风格
- 敏感文件检测（.env、密钥、凭证等自动拦截）
- 提交前确认，提交后询问是否推送
- 支持中文/英文，自动匹配项目语言

---

## 🚀 如何使用

这些 Skill 是为 [Claude Code](https://claude.com/claude-code) 设计的。使用方式：

**安装方式：**

```bash
# 1. 克隆本仓库
git clone https://github.com/NobitaYuan/nobita-skills.git

# 2. 复制需要的 Skill 到你的项目
cp -r nobita-skills/Draw.io图表生成 你的项目/.claude/skills/
cp -r nobita-skills/git-commit 你的项目/.claude/skills/
```

**使用方式：**
- Claude 会自动识别并加载已安装的 Skill

## 📝 贡献

欢迎提交 Issue 或 PR 来完善现有 Skill 或添加新的 Skill！

## 📄 许可

MIT License
