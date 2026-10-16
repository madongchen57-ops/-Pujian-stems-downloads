# 谱间音频分离

免费、无需注册的离线六轨分离程序：**人声、吉他、钢琴、贝斯、鼓、其他伴奏**。新版增加离线 BPM 和基础和弦识别。

[公开下载网页](https://pujian-six-stems.madongchen57.chatgpt.site) · [0.2.0-beta.1 安装包与文档](https://github.com/madongchen57-ops/-Pujian-stems-downloads/releases/tag/v0.2.0-beta.1)

| 系统 | 下载 | 大小 |
|---|---|---|
| Windows 10/11 x64 | [安装程序 .exe](https://github.com/madongchen57-ops/-Pujian-stems-downloads/releases/download/v0.2.0-beta.1/Pujian-Stems-0.2.0-beta.1-win-x64.exe) | 约 1.84 GB |
| Windows，便于转发 | [分享 ZIP](https://github.com/madongchen57-ops/-Pujian-stems-downloads/releases/download/v0.2.0-beta.1/Pujian-Stems-0.2.0-beta.1-windows-x64-share.zip) | 约 1.84 GB |
| Apple Silicon Mac，macOS 13+ | [安装镜像 .dmg](https://github.com/madongchen57-ops/-Pujian-stems-downloads/releases/download/v0.2.0-beta.1/Pujian-Stems-0.2.0-beta.1-mac-arm64.dmg) | 约 383 MB |

下载无需登录。运行环境、解码器和固定 Demucs `htdemucs_6s` 模型均包含在安装包中，首次运行无需下载组件。Windows 建议安装预留 8 GB，Mac 3 GB；音频处理和导出另留至少 4 GB。

## 安装与使用

1. Windows 双击 .exe 安装；Mac 打开 .dmg，将应用拖入 Applications。
2. 打开“谱间音频分离”，导入 MP3、WAV、M4A 或 FLAC。单文件最多 100 MB，单次片段最多 10 分钟。
3. 点击“开始分离”，完成后可独奏、混音、原曲对照、跳转和循环试听，导出单轨 WAV 或六轨 ZIP。
4. 分离后自动识别 BPM 和和弦；旧任务点击“补充分析”，无需重新分离。支持半速/倍速候选、手动校正、恢复自动结果及 TXT/CSV 导出。

和弦支持大、小三和弦，属七、大七、小七，sus2、sus4 及稳定低音支持的转位，例如 C/E。N.C. 表示无和弦，? 表示待校对。自动估计需要结合试听校正，算法得分不代表准确率。

[完整使用说明及首次打开步骤](https://github.com/madongchen57-ops/-Pujian-stems-downloads/releases/download/v0.2.0-beta.1/Pujian-Stems-Guide.md) · [使用许可](https://github.com/madongchen57-ops/-Pujian-stems-downloads/releases/download/v0.2.0-beta.1/Pujian-Stems-License.txt)

## 测试状态

版本 `0.2.0-beta.1` 为公开测试版。Windows 与 Apple Silicon Mac 均通过各自原生 CI 的冻结引擎测试、真实分离与分析、原生安装后的界面自动测试。Windows 本机打包程序另外通过 22 项界面检查；分析前后六轨音频校验值保持不变。升级沿用原有用户数据目录，继续显示历史任务。

上述为自动验证结果。新版两平台的人工听辨、干净机器断网安装验收仍待补充；Mac 首版使用 CPU。复杂和声、弱鼓、失真和自由速度都可能需要人工校对。

## 完整性与许可

Release 提供 SHA-256 文件和版本清单；第三方依赖许可、模型来源、版本和校验值随安装包提供。

- Windows SHA-256：`4ef167791d0f2867e94e14a21be4b8600a5d11c504e90f24c204a5b2fb2c9d54`
- Mac SHA-256：`6be43d8b6d796588191ab58b463f21b7378ad7c2ba7149f5c66aa8d59cc738c2`
- Windows 分享 ZIP SHA-256：`8bffd62ecd28a3ec2d015c56da10247fa3a218a85e77c07810d16d750488b00c`

允许免费分享完整、未修改的安装包和用户文档。此仓库只分发安装包及文档，自有构建源码保持私有；不包含私人录音或实验数据。音频、分析结果和历史任务保存在使用者本机，不上传音频。
