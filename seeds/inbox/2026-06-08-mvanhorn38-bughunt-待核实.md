---
type: seed
status: review
created_at: 2026-06-08
updated_at: 2026-06-08
source_url: https://github.com/mvanhorn38/bughunt
tags:
  - GitHub
  - Repo
  - Security
  - 待核实
---

# mvanhorn38/bughunt 待核实

## 原始线索

- https://github.com/mvanhorn38/bughunt

## 当前核实状态

2026-06-08 抓取 GitHub API 时返回 `Not Found`，README endpoint 也未返回有效 README。

## 当前处理

先保存为 seed，不迁入正式 `raw/repos`。后续若拿到正确 URL，需要先判断它是 bug bounty、安全扫描、漏洞复现还是普通调试工具，再决定安全边界。
