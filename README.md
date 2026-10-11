# Trie

Vision: Talk. Recognize. Interpret. Execute. Current releases stop at placing text; they do not execute commands or send messages.

Trie is a local voice-input app for Apple Silicon Macs. It transcribes speech and can polish the result on your device, then places the text in the focused app. You decide whether to send it.

[中文](#中文) · [Website](https://trie.ai/) · [Installation](https://trie.ai/install.html) · [Privacy](https://trie.ai/en/privacy.html) · [Releases](https://github.com/TRIEAI/trie/releases)

## Release availability

Version 0.6.0 is undergoing release acceptance. This GitHub repository does not yet host downloadable app releases, and the Homebrew cask is not yet published. For the currently available version, follow the [website installation instructions](https://trie.ai/install.html). The DMG and setup-assistant workflow below describes the planned 0.6.0 delivery.

## Requirements and installation

- Apple Silicon Mac, macOS 14 or later, at least 16 GB memory and 12 GB free disk space.
- Download a published DMG from Releases, drag Trie into Applications, eject the disk image, and open Trie from Applications.
- The setup assistant prepares Python and downloads models when you choose to proceed, then guides microphone, Accessibility and Input Monitoring permissions.
- Quit the existing Trie before replacing it. Keep your configuration and model files when upgrading.
- Homebrew availability will be announced with the first verified stable cask. Until then, use a published release or the website's current installation instructions.

## Feedback

[Report a bug or suggest a feature](https://github.com/TRIEAI/trie/issues/new/choose). Include the app version, macOS version, chip/memory, installation method, reproduction steps and expected versus actual behavior. Reports here are **public**.

The app's diagnostic export is optional. Review any attachment before posting; do not upload recordings, dictated text, clipboard contents, personal mappings or credentials. Diagnostics are never uploaded automatically by Trie. Send security reports privately to [contact@trie.ai](mailto:contact@trie.ai).

## Scope and known boundaries

- Transcription and polishing run locally. Initial setup requires downloads. Checking for updates is user initiated.
- `plain`, `coding` and `chat` profiles select different prompts and terminology mappings. Per-app selection and manual selection are supported.
- Text delivery does not press Return or send messages. Focus changes and Secure Input can cause a clipboard-only fallback.
- Long text may fall back to the raw transcription when polishing times out or fails validation. Confirm the text before sending.
- Switching microphones while recording may interrupt that session; start a new recording once the device is ready.
- Release-specific known issues and acceptance status are listed in each release.

This repository hosts public documentation, release artifacts and feedback. The app source is not published here. The app is currently free to use; see [license and third-party notices](https://trie.ai/credits.html) for applicable terms.

## 中文

Trie 是 Apple Silicon Mac 上的本地语音输入工具。识别与润色在本机完成，将文字交付到输入位置后即停止；是否发送由你决定。

发布状态：0.6.0 正在完成发布验收；本 GitHub 仓库尚无可下载的应用 Release，Homebrew cask 也尚未发布。当前可用版本请以[官网安装说明](https://trie.ai/install.html)为准。下述 DMG 与设置助手流程描述待发布的 0.6.0 交付。

安装要求：macOS 14 或更新版本、至少 16 GB 内存、12 GB 可用磁盘。下载已发布的 DMG，将 Trie 拖到 Applications，推出安装磁盘，再从 Applications 启动。设置助手会按你的操作准备 Python、下载模型并引导三项权限。升级前先正常退出旧版。

[安装说明](https://trie.ai/install.html) · [隐私说明](https://trie.ai/privacy.html) · [反馈问题](https://github.com/TRIEAI/trie/issues/new/choose)

反馈在此公开展示，请提供版本、系统、设备、安装方式、复现步骤与预期结果。诊断文件由你自愿导出并检查后上传，不要公开录音、听写正文、剪贴板、个人映射表或密钥。安全问题请私信 contact@trie.ai。

本仓库用于文档、安装包和反馈，不公开客户端源码。Homebrew 通道以正式发布公告和验证结果为准。
