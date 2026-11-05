# Duou-Switch 官方二进制分发

当前正式版：[Duou-Switch 4.6.1](https://github.com/DuouTech/duou-switch-releases/releases/tag/v4.6.1)。下载 [Windows x64 当前用户级安装包](https://github.com/DuouTech/duou-switch-releases/releases/download/v4.6.1/Duou-Switch_4.6.1_x64-setup.exe)。

安装包 SHA256：`93177622331a27c8262dad279abe378505d78adf1a8f3ca5ec21f9296a14319b`。公开安装器及签名已经匿名下载核对，并通过独立 Tauri/minisign 验签；[stable 更新清单](https://raw.githubusercontent.com/DuouTech/duou-switch-releases/main/channels/stable/latest.json)沿用 Duou 原签名信任链。安装器没有 Windows Authenticode 发布者证书签名，minisign 不等于 Authenticode。

4.6.1 移除继承的 CC Switch 赞助推荐、促销与返佣入口，保留官方中立模板、自定义及已保存连接，并加入防回流检查。选择性集成固定上游 v4.0.25 的 Windows、路由兼容、Codex 与 Pi MCP 等修复，并非全量合并。与 Tihu 共用核心，保留 Duou 原身份、`.duou-switch` 数据、主题、`duou-switch://` 协议和默认端口 15722。两品牌接管同一 Agent 时须先退出或释放原控制权；重新启用由用户操作。

升级前退出本地路由，保持原安装目录和当前用户范围，不删除 `.duou-switch`。旧 4.0.0 关闭了更新，需要手动覆盖安装；后续版本可使用应用内更新。各个带 Acceptance 标识的隔离验收包仅供测试，不替代日常版本。

公开 Release 仅提供安装器、对应 `.sig`、`latest.json`、`SHA256SUMS`、中文说明和 MIT `LICENSE.txt`。GitHub 自动生成的源码归档仅含本公开仓库的说明和清单，不含应用私有源码、用户数据或密钥。仅发布 Windows x64；保留 CC Switch 作者版权、MIT 许可与第三方署名。
