# Duou-Switch 官方二进制分发

当前正式版：[Duou-Switch 4.6.0](https://github.com/DuouTech/duou-switch-releases/releases/tag/v4.6.0)。下载 [Windows x64 当前用户级安装包](https://github.com/DuouTech/duou-switch-releases/releases/download/v4.6.0/Duou-Switch_4.6.0_x64-setup.exe)。

安装包 SHA256：`feb617e6892ee05cd3ca7b8823dfbdf362e4c7a61191a411e214f6b14608746d`。公开安装器及签名已经匿名下载核对，并通过独立 Tauri/minisign 验签；[stable 更新清单](https://raw.githubusercontent.com/DuouTech/duou-switch-releases/main/channels/stable/latest.json)沿用 Duou 原签名信任链。安装器没有 Windows Authenticode 发布者证书签名，minisign 不等于 Authenticode。

4.6.0 选择性适配固定上游 CC Switch v4.0.24，与 Tihu 共用核心，保留 Duou 原身份、`.duou-switch` 数据、主题、`duou-switch://` 协议和默认路由端口 15722。新快速配置移除鹈鹕专属预设，已保存的用户卡片继续保留。两个品牌接管同一 Agent 时须明确退出或释放原控制权；释放保留文件，重新启用由用户操作。

升级前退出本地路由，保持原安装目录和当前用户范围，不删除 `.duou-switch`。旧 4.0.0 关闭了更新，需要手动覆盖安装；后续版本可使用应用内更新。各个带 Acceptance 标识的隔离验收包仅供测试，不替代日常版本。

公开 Release 仅提供安装器、对应 `.sig`、`latest.json`、`SHA256SUMS`、中文说明和 MIT `LICENSE.txt`。GitHub 自动生成的源码归档仅含本公开仓库的说明和清单，不含应用私有源码、用户数据或密钥。仅发布 Windows x64；保留 CC Switch 作者版权、MIT 许可与第三方署名。
