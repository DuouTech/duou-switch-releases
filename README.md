# Duou-Switch 官方二进制发行

2026-11-17 验证快照：[Duou-Switch 4.6.3](https://github.com/DuouTech/duou-switch-releases/releases/tag/v4.6.3)，Windows x64 当前用户级安装包。

- [国内下载 CNB](https://cnb.cool/duoutech/duou-switch/-/releases/latest/download/Duou-Switch_x64-setup.exe)
- [海外下载 GitHub](https://github.com/DuouTech/duou-switch-releases/releases/latest/download/Duou-Switch_x64-setup.exe)
- 文件：`Duou-Switch_4.6.3_x64-setup.exe`，15,423,816 字节。
- SHA256：`c22c67ae764b654584174c1a7f78064853fc765ee5334921c7aa0c843a530c61`。

两平台分发同一份已签名安装器，保留原始 `.sig`、`SHA256SUMS`、版本说明和许可文件。GitHub 为正式发布主源，CNB 为国内下载镜像；不要把 Source code 压缩包或临时附件 URL 当作安装器。

客户端仍使用原有 [stable 更新清单](https://raw.githubusercontent.com/DuouTech/duou-switch-releases/main/channels/stable/latest.json)及本品牌独立公钥。本次仅调整官网下载和发布镜像，Tauri/minisign 更新签名不等于 Windows Authenticode 发布者签名。

Duou-Switch 保留独立应用身份、已有资料和协议。1.0.4 / 4.6.3 的升级及两品牌配置交接说明以各自正式 Release 为准；不要依据旧版本说明覆盖用户配置。

本仓库仅包含二进制发行相关资料和镜像维护工具，不包含应用私有源码、用户数据或密钥。保留 CC Switch 作者版权、MIT 许可与第三方署名。

## 发布维护

CNB [同步分支](https://cnb.cool/duoutech/duou-switch/-/tree/codex/github-release-sync)已提供每 30 分钟检查 GitHub 最新正式版与 stable 清单的配置；使用 CNB 自带的任务临时令牌，不依赖 GitHub Actions。仅在版本、平台、大小、SHA256、原始签名均匹配后补齐附件。同名资产冲突会失败，不覆盖或删除公开版本。

官网使用永久链接，后续正常发布无需修改官网；同步失败时 CNB 保留上一个完整正式版。可用该分支的 `api_trigger` 手动执行，或以仅限本仓库 `repo-release:rw` 的安全凭据运行 `python sync_cnb.py --product duou-switch --verify-downloads --report verified-release.json`。令牌通过 `CNB_TOKEN` 环境变量注入，不写入脚本、日志或仓库。

2026-11-16 验证：手动 CNB 流水线已成功，现有安装器跳过，缺失附件已补齐且双源匿名下载哈希一致。定时任务同步接口要求 Master 及以上角色，当前 Developer 角色被拒绝；定时启用尚未验收，不宣称全自动运行。

## 永久链接与任务状态（2026-11-17）

固定名 `Duou-Switch_x64-setup.exe` 是原签名安装器的逐字节副本，原版本文件和更新签名保留；别名校验独立保存在 `SHA256SUMS-downloads.txt`。上述大小/哈希仅对应验证快照，后续以当次正式 Release 为准。

`codex/github-release-sync` 的每小时第 7、37 分钟定时任务已观测到真实成功，负责人 `cnb.dInoEWDGgGA`，两产品各自只操作本仓库。GitHub 匿名 API 曾间歇返回 403；失败会非零退出并记录日志，不提升不完整版本，下一周期继续检查。仅手动重新注册要求 Master，不代表 Developer 的既有定时任务没有运行。

[构建记录](https://cnb.cool/duoutech/duou-switch/-/builds)。后续正式发布必须生成固定名及独立校验文件，使用共享发布工具 prepare/publish/promote；不要仅手工补当前版本。维护者需合并发布工具 PR 后再从默认流程发布新版本；当前网站接入与安装器字节不依赖该合并。
