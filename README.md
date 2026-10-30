# 绘造 Huizao · 下载仓库

本仓库只放**发行产物与更新清单**，不含源码。客户端「检查更新」直接读这里的 `version.json`。

## 当前版本

- 版本：1.1.0
- 安装包：见 [Releases](https://github.com/guanyuefu-hub/huizao/releases/latest) 中的 `huizao-1.1.0.zip`
- 更新清单：<https://raw.githubusercontent.com/guanyuefu-hub/huizao/main/version.json>

## 安装

1. 下载 `huizao-<版本>.zip`
2. 解压到任意目录（保持 `绘造.exe` 与 `_internal/` 同级）
3. 双击 `绘造.exe`（需要 Windows 10 1809+ / 11 x64 与 WebView2 运行时）

## 校验

安装包的 SHA-256 以 `version.json` 的 `sha256` 字段为准；客户端下载后会自行校验，不一致会拒绝安装。

## 发版

本地源码仓库执行 `tools/build_exe.ps1` → `tools/make_release.py --base-url ...`，再把新 zip 作为 Release 附件上传、覆盖本仓库的 `version.json` 即可。
