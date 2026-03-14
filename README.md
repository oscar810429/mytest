# OpenClaw GitHub Skill

[English](#english) | [中文](#中文)

---

## English

This repository demonstrates how to use the OpenClaw GitHub skill.

### What is OpenClaw?

OpenClaw is an open-source AI agent that can help you with various tasks, including GitHub operations.

### GitHub Skill Features

- **Issue Management**: List, view, create, and manage issues
- **Pull Requests**: Check status, view details, merge PRs
- **CI/CD Monitoring**: View workflow runs, check CI status
- **API Access**: Advanced queries using GitHub API

### Basic Commands

```bash
# List issues
gh issue list --repo owner/repo

# Create an issue
gh issue create --title "Bug" --body "Description"

# Check PR status
gh pr checks 55 --repo owner/repo

# List workflow runs
gh run list --repo owner/repo --limit 10

# View run logs
gh run view <run-id> --repo owner/repo --log-failed
```

### API Examples

```bash
# Get PR details
gh api repos/owner/repo/pulls/55 --jq '.title, .state'

# Search repositories
gh api search/repositories?q=topic:openclaw
```

### Installation

1. Install GitHub CLI:
```bash
brew install gh
```

2. Login to GitHub:
```bash
gh auth login
```

3. Configure OpenClaw with GitHub skill (optional)

---

## 中文

本仓库演示了如何使用 OpenClaw 的 GitHub 技能。

### 什么是 OpenClaw？

OpenClaw 是一个开源 AI 助手，可以帮助你完成各种任务，包括 GitHub 操作。

### GitHub 技能功能

- **问题管理**：列出、查看、创建和管理 Issues
- **拉取请求**：检查状态、查看详情、合并 PR
- **CI/CD 监控**：查看工作流运行状态、检查 CI 状态
- **API 访问**：使用 GitHub API 进行高级查询

### 基本命令

```bash
# 列出问题
gh issue list --repo owner/repo

# 创建问题
gh issue create --title "Bug" --body "描述"

# 检查 PR 状态
gh pr checks 55 --repo owner/repo

# 列出工作流运行
gh run list --repo owner/repo --limit 10

# 查看运行日志
gh run view <run-id> --repo owner/repo --log-failed
```

### API 示例

```bash
# 获取 PR 详情
gh api repos/owner/repo/pulls/55 --jq '.title, .state'

# 搜索仓库
gh api search/repositories?q=topic:openclaw
```

### 安装步骤

1. 安装 GitHub CLI：
```bash
brew install gh
```

2. 登录 GitHub：
```bash
gh auth login
```

3. 配置 OpenClaw GitHub 技能（可选）

---

## Links

- [OpenClaw Official Website](https://openclaw.ai)
- [OpenClaw GitHub](https://github.com/openclaw/openclaw)
- [GitHub CLI Documentation](https://cli.github.com)

---

*Generated with OpenClaw*
