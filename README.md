# Vaultwarden Windows Binary

[![Build and Release](https://github.com/tangz0v0/Vaultwarden-Windows-Binary/actions/workflows/build-windows.yml/badge.svg)](https://github.com/tangz0v0/Vaultwarden-Windows-Binary/actions/workflows/build-windows.yml)

自动构建 Vaultwarden Windows 版本的二进制文件。

## 📦 下载

前往 [Releases](https://github.com/tangz0v0/Vaultwarden-Windows-Binary/releases) 页面下载最新版本。

### 版本说明

| Release 类型 | 标签格式 | 说明 |
|-------------|---------|------|
| **稳定版** | `vX.X.X-windows` | 基于官方 GitHub Release，稳定可靠 |
| **测试版** | `testing-xxxxxxx-windows` | 基于主分支最新代码，包含最新修复 |

## 🚀 快速使用

1. 从 Releases 下载 `vaultwarden-*.exe` 文件
2. 将文件放在目标目录
3. 运行即可（可以注册为 Windows 服务）

### 作为服务运行

```powershell
# 安装为 Windows 服务
sc.exe create Vaultwarden binPath="C:\path\to\vaultwarden.exe" start=auto

# 启动服务
sc.exe start Vaultwarden
