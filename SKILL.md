---
name: github-repo-design
description: GitHub 仓库设计与 README 最佳实践指南，帮助创建专业的开源项目结构
triggers:
  - github repo
  - repository design
  - readme design
  - 仓库设计
  - 项目结构
  - 开源项目
  - profile readme
  - github profile
  - readme badge
  - readme template
---

# GitHub 仓库设计与 README 最佳实践

> 基于 100+ 优秀开源项目研究总结的最佳实践指南

## 使用场景

当用户需要以下帮助时使用此 skill：
- 创建新的 GitHub 仓库
- 设计项目文件结构
- 编写 README 文件
- 配置开源项目必备文件
- 优化仓库可发现性

---

## 一、仓库核心文件结构

### 推荐的项目结构

```
project-name/
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   ├── bug_report.yml
│   │   ├── feature_request.yml
│   │   └── config.yml
│   ├── PULL_REQUEST_TEMPLATE.md
│   ├── CODEOWNERS
│   ├── FUNDING.yml
│   └── workflows/
│       └── ci.yml
├── docs/
│   └── (详细文档)
├── src/
│   └── (源代码)
├── tests/
│   └── (测试文件)
├── README.md              # 必需 - 项目说明
├── LICENSE                # 必需 - 开源许可证
├── CONTRIBUTING.md        # 推荐 - 贡献指南
├── CODE_OF_CONDUCT.md     # 推荐 - 行为准则
├── SECURITY.md            # 推荐 - 安全策略
├── CHANGELOG.md           # 推荐 - 变更日志
├── CITATION.cff           # 可选 - 引用信息
└── .gitignore             # 必需 - 忽略规则
```

---

## 二、README.md 设计指南

### README 必备内容

```markdown
# 项目名称

简短的一句话描述项目用途。

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Build Status](https://github.com/user/repo/workflows/CI/badge.svg)](https://github.com/user/repo/actions)

## 功能特性

- 特性 1：简要说明
- 特性 2：简要说明
- 特性 3：简要说明

## 快速开始

### 安装

\`\`\`bash
npm install package-name
# 或
pip install package-name
\`\`\`

### 基本用法

\`\`\`javascript
import { feature } from 'package-name';

// 示例代码
const result = feature();
\`\`\`

## 文档

详细文档请访问 [文档链接](docs/)

## 贡献

欢迎贡献！请阅读 [贡献指南](CONTRIBUTING.md)

## 许可证

本项目采用 [MIT 许可证](LICENSE)
```

### README 设计原则

| 原则 | 说明 |
|------|------|
| **简洁明了** | 开头一句话说明项目用途 |
| **快速上手** | 提供安装和基本用法示例 |
| **视觉吸引** | 使用徽章、截图、GIF 演示 |
| **结构清晰** | 使用标题层级组织内容 |
| **链接完整** | 提供文档、贡献指南等链接 |

### 常用徽章 (Badges)

```markdown
<!-- 许可证 -->
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

<!-- 构建状态 -->
[![CI](https://github.com/USER/REPO/actions/workflows/ci.yml/badge.svg)](https://github.com/USER/REPO/actions)

<!-- npm 版本 -->
[![npm version](https://badge.fury.io/js/PACKAGE.svg)](https://www.npmjs.com/package/PACKAGE)

<!-- 下载量 -->
[![Downloads](https://img.shields.io/npm/dm/PACKAGE.svg)](https://www.npmjs.com/package/PACKAGE)

<!-- 代码覆盖率 -->
[![codecov](https://codecov.io/gh/USER/REPO/branch/main/graph/badge.svg)](https://codecov.io/gh/USER/REPO)
```

---

## 三、核心配置文件

### 1. LICENSE - 开源许可证

常用许可证选择：

| 许可证 | 特点 | 适用场景 |
|--------|------|----------|
| **MIT** | 宽松，允许商用 | 大多数开源项目 |
| **Apache 2.0** | 专利保护，商用友好 | 企业级项目 |
| **GPL-3.0** | 强制开源衍生作品 | 希望保持开源的项目 |
| **BSD-3-Clause** | 宽松，需保留版权声明 | 学术项目 |
| **CC0** | 公共领域 | 数据集、文档 |

### 2. CONTRIBUTING.md - 贡献指南

```markdown
# 贡献指南

感谢你考虑为本项目做出贡献！

## 如何贡献

### 报告 Bug

1. 确认 bug 尚未被报告
2. 使用 Bug 报告模板创建 Issue
3. 提供详细的复现步骤

### 提交功能请求

1. 先搜索是否已有类似请求
2. 使用功能请求模板创建 Issue
3. 清晰描述需求和用例

### 提交代码

1. Fork 本仓库
2. 创建功能分支：`git checkout -b feature/amazing-feature`
3. 提交更改：`git commit -m 'Add amazing feature'`
4. 推送分支：`git push origin feature/amazing-feature`
5. 创建 Pull Request

## 代码规范

- 遵循项目现有的代码风格
- 添加必要的测试
- 更新相关文档

## 行为准则

请阅读我们的 [行为准则](CODE_OF_CONDUCT.md)
```

### 3. CODE_OF_CONDUCT.md - 行为准则

推荐使用 [Contributor Covenant](https://www.contributor-covenant.org/) 模板。

### 4. SECURITY.md - 安全策略

```markdown
# 安全策略

## 支持的版本

| 版本 | 支持状态 |
|------|----------|
| 2.x  | ✅ 支持  |
| 1.x  | ❌ 不再支持 |

## 报告漏洞

如果发现安全漏洞，请：

1. **不要**公开创建 Issue
2. 发送邮件至 security@example.com
3. 包含漏洞详细描述和复现步骤

我们会在 48 小时内回复。
```

### 5. CODEOWNERS - 代码所有者

```
# 默认所有者
* @username

# 特定目录所有者
/docs/ @docs-team
/src/api/ @api-team
*.js @frontend-team

# 特定文件
package.json @maintainer
```

### 6. .gitignore - 忽略规则

```gitignore
# 依赖
node_modules/
vendor/
__pycache__/

# 构建产物
dist/
build/
*.egg-info/

# 环境配置
.env
.env.local
*.local

# IDE
.idea/
.vscode/
*.swp

# 系统文件
.DS_Store
Thumbs.db

# 日志
*.log
logs/

# 测试覆盖率
coverage/
.nyc_output/
```

---

## 四、Issue 和 PR 模板

### Bug 报告模板 (.github/ISSUE_TEMPLATE/bug_report.yml)

```yaml
name: Bug 报告
description: 报告一个 bug
labels: ["bug"]
body:
  - type: markdown
    attributes:
      value: 感谢你报告 bug！
  - type: textarea
    id: description
    attributes:
      label: Bug 描述
      description: 清晰描述这个 bug
    validations:
      required: true
  - type: textarea
    id: reproduce
    attributes:
      label: 复现步骤
      description: 如何复现这个问题？
      placeholder: |
        1. 执行 '...'
        2. 点击 '...'
        3. 看到错误
    validations:
      required: true
  - type: textarea
    id: expected
    attributes:
      label: 期望行为
      description: 你期望发生什么？
  - type: input
    id: version
    attributes:
      label: 版本
      description: 使用的版本号
```

### PR 模板 (.github/PULL_REQUEST_TEMPLATE.md)

```markdown
## 描述

简要描述这个 PR 的更改内容。

## 更改类型

- [ ] Bug 修复
- [ ] 新功能
- [ ] 文档更新
- [ ] 重构
- [ ] 其他

## 检查清单

- [ ] 代码遵循项目规范
- [ ] 已添加/更新测试
- [ ] 已更新文档
- [ ] 所有测试通过

## 相关 Issue

Fixes #(issue number)
```

---

## 五、仓库设置优化

### 1. Topics (主题标签)

添加相关主题提高可发现性：
- 技术栈：`javascript`, `python`, `react`
- 类型：`cli`, `library`, `framework`
- 领域：`machine-learning`, `web`, `devops`

### 2. 社交预览图

- 尺寸：1280 x 640 像素
- 格式：PNG, JPG, GIF
- 大小：< 1 MB

### 3. 分支保护规则

推荐为 `main` 分支启用：
- ✅ 要求 PR 审查
- ✅ 要求状态检查通过
- ✅ 要求线性历史
- ✅ 禁止强制推送

### 4. GitHub Actions CI

```yaml
# .github/workflows/ci.yml
name: CI

on:
  push:
    branches: [main]
  pull_request:
    branches: [main]

jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Setup Node.js
        uses: actions/setup-node@v4
        with:
          node-version: '20'
      - run: npm ci
      - run: npm test
```

---

## 六、发布管理

### Releases 最佳实践

1. 使用语义化版本：`MAJOR.MINOR.PATCH`
2. 编写清晰的发布说明
3. 包含变更日志链接
4. 标记重大变更 (Breaking Changes)

### CHANGELOG.md 格式

```markdown
# Changelog

## [2.0.0] - 2024-01-15

### Breaking Changes
- 移除了废弃的 API

### Added
- 新增功能 A
- 新增功能 B

### Fixed
- 修复了 bug #123

### Changed
- 优化了性能

## [1.0.0] - 2023-12-01

### Added
- 初始发布
```

---

## 七、GitHub Profile README

### 创建个人主页 README

在 GitHub 上创建与用户名同名的仓库，添加 README.md 即可显示在个人主页。

### 常用统计组件

```markdown
<!-- GitHub Stats -->
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=USERNAME&show_icons=true&theme=radical)

<!-- 语言统计 -->
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=USERNAME&layout=compact&theme=radical)

<!-- 连续贡献统计 -->
![GitHub Streak](https://streak-stats.demolab.com/?user=USERNAME&theme=radical)

<!-- GitHub Trophies -->
![Trophies](https://github-profile-trophy.vercel.app/?username=USERNAME&theme=radical&row=1)

<!-- 活动图 -->
![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=USERNAME&theme=react-dark)

<!-- 访问计数 -->
![Visitors](https://komarev.com/ghpvc/?username=USERNAME&color=blue)
```

### Profile README 模板

```markdown
# Hi there 👋

## About Me
- 🔭 I'm currently working on ...
- 🌱 I'm currently learning ...
- 👯 I'm looking to collaborate on ...
- 💬 Ask me about ...
- 📫 How to reach me: ...

## Tech Stack
![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat&logo=python&logoColor=white)
![React](https://img.shields.io/badge/-React-61DAFB?style=flat&logo=react&logoColor=black)

## GitHub Stats
![Stats](https://github-readme-stats.vercel.app/api?username=USERNAME&show_icons=true)
```

---

## 八、README 工具和生成器

### 推荐工具

| 工具 | 用途 | 链接 |
|------|------|------|
| **readme.so** | 可视化 README 编辑器 | readme.so |
| **GPRM** | GitHub Profile README 生成器 | gprm.itsvg.in |
| **readme-ai** | AI 驱动的 README 生成 | github.com/eli64s/readme-ai |
| **Shields.io** | 自定义徽章生成 | shields.io |
| **Simple Icons** | 品牌图标库 | simpleicons.org |
| **Carbon** | 代码截图美化 | carbon.now.sh |
| **Asciinema** | 终端录制 | asciinema.org |

### Shields.io 高级用法

```markdown
<!-- 自定义颜色和样式 -->
![Custom](https://img.shields.io/badge/label-message-color?style=for-the-badge&logo=LOGO)

<!-- 动态数据徽章 -->
![GitHub stars](https://img.shields.io/github/stars/USER/REPO?style=social)
![npm downloads](https://img.shields.io/npm/dm/PACKAGE)
![GitHub issues](https://img.shields.io/github/issues/USER/REPO)
![GitHub license](https://img.shields.io/github/license/USER/REPO)

<!-- 徽章样式选项 -->
<!-- style: flat, flat-square, plastic, for-the-badge, social -->
```

---

## 九、高级徽章配置

### 技术栈徽章

```markdown
<!-- 前端 -->
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Vue.js](https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vue.js&logoColor=4FC08D)

<!-- 后端 -->
![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)

<!-- 数据库 -->
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)

<!-- 云服务 -->
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)
![GCP](https://img.shields.io/badge/GCP-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
```

### 社交链接徽章

```markdown
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](URL)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](URL)
[![Discord](https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)](URL)
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](URL)
```

---

## 十、安全最佳实践

### 依赖安全

```yaml
# .github/dependabot.yml
version: 2
updates:
  - package-ecosystem: "npm"
    directory: "/"
    schedule:
      interval: "weekly"
    open-pull-requests-limit: 10

  - package-ecosystem: "github-actions"
    directory: "/"
    schedule:
      interval: "weekly"
```

### 安全扫描工作流

```yaml
# .github/workflows/security.yml
name: Security Scan

on:
  push:
    branches: [main]
  pull_request:
    branches: [main]
  schedule:
    - cron: '0 0 * * 0'  # 每周日运行

jobs:
  codeql:
    runs-on: ubuntu-latest
    permissions:
      security-events: write
    steps:
      - uses: actions/checkout@v4
      - uses: github/codeql-action/init@v3
        with:
          languages: javascript, python
      - uses: github/codeql-action/analyze@v3

  dependency-review:
    runs-on: ubuntu-latest
    if: github.event_name == 'pull_request'
    steps:
      - uses: actions/checkout@v4
      - uses: actions/dependency-review-action@v4
```

### 密钥扫描

```yaml
# .github/workflows/secrets.yml
name: Secret Scan

on: [push, pull_request]

jobs:
  trufflehog:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
        with:
          fetch-depth: 0
      - uses: trufflesecurity/trufflehog@main
        with:
          extra_args: --only-verified
```

---

## 十一、Monorepo 结构

### 推荐结构

```
monorepo/
├── .github/
│   └── workflows/
├── packages/
│   ├── core/
│   │   ├── src/
│   │   ├── package.json
│   │   └── README.md
│   ├── cli/
│   │   ├── src/
│   │   ├── package.json
│   │   └── README.md
│   └── web/
│       ├── src/
│       ├── package.json
│       └── README.md
├── docs/
├── examples/
├── scripts/
├── package.json          # 根 package.json
├── pnpm-workspace.yaml   # 或 lerna.json
├── turbo.json            # Turborepo 配置
└── README.md
```

### 工具选择

| 工具 | 特点 |
|------|------|
| **pnpm workspaces** | 高效磁盘空间，原生支持 |
| **Turborepo** | 增量构建，远程缓存 |
| **Nx** | 功能丰富，适合大型项目 |
| **Lerna** | 经典方案，版本管理 |

---

## 十二、CI/CD 高级配置

### 多平台测试

```yaml
# .github/workflows/test.yml
name: Test

on: [push, pull_request]

jobs:
  test:
    strategy:
      matrix:
        os: [ubuntu-latest, macos-latest, windows-latest]
        node: [18, 20, 22]
    runs-on: ${{ matrix.os }}
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-node@v4
        with:
          node-version: ${{ matrix.node }}
          cache: 'npm'
      - run: npm ci
      - run: npm test
```

### 自动发布

```yaml
# .github/workflows/release.yml
name: Release

on:
  push:
    tags:
      - 'v*'

jobs:
  release:
    runs-on: ubuntu-latest
    permissions:
      contents: write
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-node@v4
        with:
          node-version: 20
          registry-url: 'https://registry.npmjs.org'
      - run: npm ci
      - run: npm publish
        env:
          NODE_AUTH_TOKEN: ${{ secrets.NPM_TOKEN }}
      - uses: softprops/action-gh-release@v2
        with:
          generate_release_notes: true
```

---

## 十三、快速检查清单

### 新仓库检查清单

- [ ] README.md 包含项目说明、安装、用法
- [ ] 选择了合适的 LICENSE
- [ ] 添加了 .gitignore
- [ ] 配置了 Topics 标签
- [ ] 设置了社交预览图
- [ ] 创建了 Issue/PR 模板
- [ ] 配置了分支保护规则
- [ ] 设置了 CI/CD 工作流
- [ ] 添加了 CONTRIBUTING.md（开源项目）
- [ ] 添加了 SECURITY.md（安全敏感项目）

### README 质量检查

- [ ] 一句话说明项目用途
- [ ] 包含安装和快速开始指南
- [ ] 有代码示例
- [ ] 添加了徽章（构建状态、版本、许可证）
- [ ] 包含截图或 GIF 演示（如适用）
- [ ] 链接到详细文档
- [ ] 说明如何贡献
- [ ] 标明许可证

### 安全检查清单

- [ ] 启用了 Dependabot
- [ ] 配置了 CodeQL 扫描
- [ ] 添加了 SECURITY.md
- [ ] 无硬编码密钥
- [ ] 启用了分支保护
- [ ] 要求 PR 审查

### SEO 优化检查

- [ ] 仓库描述清晰简洁
- [ ] 添加了相关 Topics（5-10 个）
- [ ] README 开头包含关键词
- [ ] 设置了社交预览图
- [ ] 有活跃的提交历史

---

## 十四、优秀 README 案例分析

### 案例 1：React (facebook/react)

**特点：**
- 简洁的项目描述
- 清晰的文档链接
- 多种安装方式
- 贡献指南链接

### 案例 2：Vue.js (vuejs/core)

**特点：**
- 徽章展示构建状态
- 快速开始指南
- 生态系统链接
- 赞助商展示

### 案例 3：TensorFlow (tensorflow/tensorflow)

**特点：**
- 详细的安装说明
- 多平台支持说明
- 丰富的示例代码
- 社区资源链接

### README 设计模式

| 模式 | 适用场景 | 特点 |
|------|----------|------|
| **极简型** | 小型工具库 | 一屏内展示核心信息 |
| **文档型** | 框架/SDK | 详细 API 和示例 |
| **展示型** | UI 组件库 | 大量截图和演示 |
| **教程型** | 学习项目 | 步骤式指南 |

---

## 十五、国际化支持

### 多语言 README

```
project/
├── README.md           # 默认（英文）
├── README.zh-CN.md     # 简体中文
├── README.ja.md        # 日文
└── README.ko.md        # 韩文
```

### 语言切换链接

```markdown
# Project Name

[English](README.md) | [简体中文](README.zh-CN.md) | [日本語](README.ja.md)
```

---

## 十六、文档网站集成

### 推荐工具

| 工具 | 特点 | 适用场景 |
|------|------|----------|
| **Docusaurus** | React 驱动，功能丰富 | 大型项目文档 |
| **VitePress** | Vue 驱动，轻量快速 | Vue 生态项目 |
| **MkDocs** | Python 驱动，Material 主题 | Python 项目 |
| **GitBook** | 在线编辑，协作友好 | 团队文档 |
| **Nextra** | Next.js 驱动 | Next.js 项目 |

### GitHub Pages 部署

```yaml
# .github/workflows/docs.yml
name: Deploy Docs

on:
  push:
    branches: [main]

jobs:
  deploy:
    runs-on: ubuntu-latest
    permissions:
      pages: write
      id-token: write
    environment:
      name: github-pages
      url: ${{ steps.deployment.outputs.page_url }}
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-node@v4
        with:
          node-version: 20
      - run: npm ci && npm run docs:build
      - uses: actions/upload-pages-artifact@v3
        with:
          path: docs/.vitepress/dist
      - uses: actions/deploy-pages@v4
        id: deployment
```

---

## 十七、版本管理策略

### 语义化版本 (SemVer)

```
MAJOR.MINOR.PATCH

MAJOR: 不兼容的 API 变更
MINOR: 向后兼容的功能新增
PATCH: 向后兼容的问题修复
```

### 预发布版本

```
1.0.0-alpha.1
1.0.0-beta.1
1.0.0-rc.1
1.0.0
```

### 自动版本管理

```yaml
# 使用 semantic-release
# .releaserc.json
{
  "branches": ["main"],
  "plugins": [
    "@semantic-release/commit-analyzer",
    "@semantic-release/release-notes-generator",
    "@semantic-release/changelog",
    "@semantic-release/npm",
    "@semantic-release/github"
  ]
}
```

### Conventional Commits

```
feat: 新功能
fix: 修复 bug
docs: 文档更新
style: 代码格式
refactor: 重构
perf: 性能优化
test: 测试
chore: 构建/工具
```

---

## 十八、代码质量工具

### Linting 配置

```json
// .eslintrc.json (JavaScript/TypeScript)
{
  "extends": ["eslint:recommended", "prettier"],
  "env": { "node": true, "es2022": true }
}
```

```toml
# pyproject.toml (Python)
[tool.ruff]
line-length = 88
select = ["E", "F", "I"]

[tool.black]
line-length = 88
```

### Pre-commit Hooks

```yaml
# .pre-commit-config.yaml
repos:
  - repo: https://github.com/pre-commit/pre-commit-hooks
    rev: v4.5.0
    hooks:
      - id: trailing-whitespace
      - id: end-of-file-fixer
      - id: check-yaml
      - id: check-added-large-files

  - repo: https://github.com/astral-sh/ruff-pre-commit
    rev: v0.1.9
    hooks:
      - id: ruff
        args: [--fix]
      - id: ruff-format
```

### EditorConfig

```ini
# .editorconfig
root = true

[*]
indent_style = space
indent_size = 2
end_of_line = lf
charset = utf-8
trim_trailing_whitespace = true
insert_final_newline = true

[*.md]
trim_trailing_whitespace = false

[*.py]
indent_size = 4
```

---

## 十九、社区建设

### Discussion 分类

推荐启用 GitHub Discussions 并设置分类：
- 📣 Announcements - 公告
- 💡 Ideas - 功能建议
- 🙏 Q&A - 问答
- 🙌 Show and tell - 展示

### 贡献者认可

```markdown
## Contributors

感谢所有贡献者！

<!-- ALL-CONTRIBUTORS-LIST:START -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

[![All Contributors](https://img.shields.io/github/all-contributors/USER/REPO)](CONTRIBUTORS.md)
```

### 赞助支持

```yaml
# .github/FUNDING.yml
github: [username]
patreon: username
open_collective: project-name
ko_fi: username
custom: ["https://example.com/donate"]
```

---

## 二十、常见问题

### Q: README 应该多长？

**A:** 取决于项目复杂度。小型工具库保持简洁（一屏），大型框架可以更详细。关键是让用户快速找到需要的信息。

### Q: 应该用什么许可证？

**A:**
- 希望最大程度开放：MIT 或 Apache 2.0
- 希望衍生作品也开源：GPL-3.0
- 企业项目：Apache 2.0（有专利保护）

### Q: 如何提高仓库可见度？

**A:**
1. 添加相关 Topics
2. 写好 README 和描述
3. 保持活跃更新
4. 参与社区讨论
5. 在社交媒体分享

### Q: Issue 模板用 YAML 还是 Markdown？

**A:** 推荐 YAML 格式（.yml），支持表单验证和下拉选择，用户体验更好。
