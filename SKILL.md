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
---

# GitHub 仓库设计与 README 最佳实践

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

## 七、快速检查清单

创建新仓库时确认：

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
