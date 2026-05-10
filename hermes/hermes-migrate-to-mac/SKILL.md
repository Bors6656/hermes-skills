---
name: hermes-migrate-to-mac
description: "Hermes Agent 迁移脚本 — 从 Windows/WSL/Linux 迁移到 macOS"
version: 1.0.0
tags: [hermes, migration, macos, backup]
platforms: [macos, linux, windows]
---

# Hermes 迁移到 macOS 脚本

## 脚本位置

`/tmp/hermes-migrate-to-mac.sh`

## 功能

- **导出模式（源机器）**：将 Hermes 配置打包，排除 sessions/logs/pycache
- **导入模式（目标 Mac）**：解压并验证关键文件

## 使用方法

### 源机器（WSL/Linux）导出：

```bash
# 标记为可执行
chmod +x /tmp/hermes-migrate-to-mac.sh

# 运行导出
/tmp/hermes-migrate-to-mac.sh --export --output ~/hermes-backup/
```

### 目标 Mac 导入：

```bash
# 1. 先把备份文件拷贝到 Mac（比如 ~/Downloads/）
# 2. 运行导入
chmod +x hermes-migrate-to-mac.sh
./hermes-migrate-to-mac.sh --import --input ~/Downloads/
```

## 迁移内容

| 文件 | 说明 |
|------|------|
| `config.yaml` | 主配置 |
| `.env` | API 密钥和凭证 |
| `auth.json` | OAuth 令牌 |
| `skills/` | 技能目录 |
| `profiles/` | 多配置文件 |

**排除**：sessions/, logs/, __pycache__, *.log

## 验证

```bash
hermes doctor
hermes status
hermes skills list
```
