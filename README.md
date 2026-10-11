# 谱间音频分离

免费、无需注册的离线六轨分离程序：**人声、吉他、钢琴、贝斯、鼓、其他伴奏**。

[下载安装包（GitHub Releases）](https://github.com/madongchen57-ops/-Pujian-stems-downloads/releases/tag/v0.1.0-beta.1)

| 系统 | 安装包 | 大小 |
|---|---|---|
| Windows 10/11 x64 | [下载 Windows `.exe`](https://github.com/madongchen57-ops/-Pujian-stems-downloads/releases/download/v0.1.0-beta.1/Pujian-Stems-0.1.0-beta.1-win-x64.exe) | 约 1.78 GB |
| Apple Silicon Mac，macOS 13+ | [下载 Mac `.dmg`](https://github.com/madongchen57-ops/-Pujian-stems-downloads/releases/download/v0.1.0-beta.1/Pujian-Stems-0.1.0-beta.1-mac-arm64.dmg) | 约 313 MB |

下载无需登录。运行环境、解码器和固定 Demucs `htdemucs_6s` 模型均包含在安装包中，安装后可完全离线处理。Windows 建议安装预留 8 GB，Mac 3 GB；音频处理和导出另留至少 4 GB。

## 安装与使用

1. Windows 双击 `.exe` 安装；Mac 打开 `.dmg`，将应用拖入 Applications。
2. 打开“谱间音频分离”，导入 MP3、WAV、M4A 或 FLAC。
3. 默认选择标准配置，点击“开始分离”，完成后可独奏、混音、原曲对照、波形跳转和循环试听。
4. 导出单轨 WAV 或六轨 ZIP。单文件最多 100 MB，单次片段最多 10 分钟。

[完整使用说明及测试版首次打开步骤](https://github.com/madongchen57-ops/-Pujian-stems-downloads/releases/download/v0.1.0-beta.1/Pujian-Stems-Guide.md) · [使用许可](https://github.com/madongchen57-ops/-Pujian-stems-downloads/releases/download/v0.1.0-beta.1/Pujian-Stems-License.txt)

## 测试状态

版本 `0.1.0-beta.1` 为公开测试版。Windows 与 Mac 安装包均通过对应系统的构建、真实分离和安装后界面自动测试。用户已确认本地 Windows 交付包可以安装；此页提供的是同版本云端构建。Mac 人工断网验收尚未完成，完整干净机器离线验收待补充。

## 完整性与许可

Release 提供每个平台的 SHA-256 文件和版本清单；第三方依赖许可、模型来源、版本和校验值随安装包提供。

- Windows SHA-256：`2c9a307d0b6efa74100fe1f3d305b37411d5196c65bae85b8bbc12522dd324f2`
- Mac SHA-256：`d1a4f6f308640ac3e9e6ca56f8b1ed2872cdebe9f5c8fe26710508b5fee5f7dc`

允许免费分享完整、未修改的安装包和用户文档。此仓库只分发安装包及文档，自有源码保持私有；不包含私人录音或实验数据。音频和历史任务保存在使用者本机，不上传音频。
