# Duou-Switch 官方二进制分发

本仓库提供 Duou-Switch Windows x64 当前用户级安装包、updater 签名、哈希和发布说明。产品源码保持私有。本仓库不保存私钥、口令、用户配置、数据库、源码包或构建缓存。

正式稳定版：[Duou-Switch 4.1.0](https://github.com/DuouTech/duou-switch-releases/releases/tag/v4.1.0)。[Windows x64 安装器](https://github.com/DuouTech/duou-switch-releases/releases/download/v4.1.0/Duou-Switch_4.1.0_x64-setup.exe)已完成匿名下载、SHA256 与 minisign 验签，stable 更新频道已启用。版本 4.1.0 基于 CC Switch v4.0.9 并保留 Duou 的配置与登录保护。

v4.0.0 在旧程序中关闭了更新，首次需要手动覆盖安装。安装前退出 Duou 并关闭本地路由，保持原安装目录和当前用户范围，不删除 `.duou-switch` 数据。后续经批准的稳定包通过独立 Duou 公钥验签，在用户确认后安装；正在运行的路由会阻止安装。

[A / 4.1.0-beta.1](https://github.com/DuouTech/duou-switch-releases/releases/tag/v4.1.0-beta.1) 和 [B / 4.1.0-beta.2](https://github.com/DuouTech/duou-switch-releases/releases/tag/v4.1.0-beta.2) 是隔离验收包。它们要求带标记的独立测试目录与参数，普通启动会拒绝运行，不能替代日常安装包。A→B 已在 Windows 上实际完成匿名下载、minisign 验签、安装重启和配置完整性核对。testing 清单仅指向 B。

公开 Release 只提供安装器、对应 sig、latest.json、SHA256SUMS、中文说明及 MIT LICENSE。GitHub 自动生成的源码归档只包含本公开分发仓库的说明/清单，不含产品私有源码。minisign 是 Tauri updater 签名，不是 Windows Authenticode 证书。

目前仅承诺本轮已验收的 Windows x64 包；其他平台不作本轮实机更新承诺。保留 CC Switch 原作者版权与 MIT 许可。[stable 清单](https://raw.githubusercontent.com/DuouTech/duou-switch-releases/main/channels/stable/latest.json)已在恢复签名验证、正式发布批准和公开资产核验通过后受控投放；不会将未经审查的上游代码直接更新给用户。
