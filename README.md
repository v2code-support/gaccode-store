# GACCode Store - GAC Claude Code API 兑换码购买平台

  <div align="center">

  ![GACCode Store](https://img.shields.io/badge/GACCode-Store-blue?style=for-the-badge)
  ![Status](https://img.shields.io/badge/status-active-success?style=for-the-badge)

  **专业的 Claude Code API 密钥服务商**

  [🌐 gaccode.store](https://gaccode.store) | [🎁 免费体验](https://gaccode.store/share) | [📖 
  使用文档](https://gaccode.store/posts)

  </div>

  ## 📋 项目简介

  GACCode Store 是专业的 GAC Claude Code API 兑换码购买平台。支持日卡、月卡多种套餐，即买即用，7x24小时技术支持。

  ## ✨ 核心特性

  - 🚀 **即买即用** - 购买后立即获得可用密钥
  - 💰 **灵活套餐** - 日卡¥7.9，月卡¥279
  - 🎁 **免费体验** - 每日提供免费体验密钥
  - 🔒 **安全可靠** - 专业团队维护，99.9%可用性
  - 📚 **完整文档** - 详细安装配置教程
  - 📞 **全天支持** - 微信、Telegram客服

  ## 🚀 快速开始

  ### 1. 获取密钥
  ```bash
  # 方式1：访问官网购买套餐
  https://gaccode.store/#products

  # 方式2：获取免费体验密钥
  https://gaccode.store/share
  ```
  ### 2. 配置环境
  ```
  export ANTHROPIC_BASE_URL=https://gaccode.com/claudecode
  export ANTHROPIC_API_KEY=sk-ant-oat01-xxxxxxx

  # 自动配置Claude Code CLI
  (cat ~/.claude.json 2>/dev/null || echo 'null') | \
  jq --arg key "${ANTHROPIC_API_KEY: -20}" \
  '(. // {}) | .customApiKeyResponses.approved |= ([.[]?, $key] | unique)' > \
  ~/.claude.json.tmp && mv ~/.claude.json.tmp ~/.claude.json
   ```
  
  ### 3. 开始使用
  ```
  # 验证claude是否可用
  claude
  # 开始使用，如
  帮我创建一个React组件
  ```
  
  ## 🎯 套餐价格

  | 套餐   | 价格   | 有效期  | 适用场景      |
  |------|------|------|-----------|
  | 日卡   | ¥7.9 | 24小时 | 短期项目、功能测试 |
  | 月卡   | ¥279 | 30天  | 中长期开发项目   |
  | 免费体验 | 免费   | 每日更新 | 新用户体验     |

  ## 📖 技术文档

  - https://gaccode.store/post/what-is-gaccode - 基础概念介绍
  - https://gaccode.store/post/claude-code-cli-install-guide - 详细安装教程
  - https://gaccode.store/post/gaccode-purchase-channels - 完整购买流程
  - https://gaccode.store/post/gaccode-package-comparison - 帮助选择方案
  - https://gaccode.store/post/claude-code-api-best-practices - 使用技巧
  - https://gaccode.store/post/gaccode-faq - FAQ解答

  ## 📞 联系支持

  - 微信客服: jopanda_ (备注：gaccode)
  - Telegram: https://t.me/easy_claude_code
  - 官方网站: https://gaccode.store

  ---
  专业团队 · 稳定服务 · 即买即用

  Made with ❤️ by GACCode Store Team
