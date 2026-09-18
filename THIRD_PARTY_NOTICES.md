# 第三方组件声明

本文件不是法律意见。发布包内 `licenses` 目录提供随软件分发的许可证文件与构建信息。

## FFmpeg

发布包包含独立运行的 `ffmpeg.exe` 与 `ffprobe.exe`，来自 Gyan.dev 的
`FFmpeg 9.0.1 essentials_build`。该构建启用了 GPL 组件（包括 libx264），按
GNU General Public License version 3 分发。

- 项目主页：https://ffmpeg.org/
- 构建提供方：https://www.gyan.dev/ffmpeg/builds/
- 对应源码提交：https://github.com/FFmpeg/FFmpeg/commit/bf1b838f2a
- 完整许可证：`licenses/FFmpeg-GPL-3.0.txt`
- 原始构建说明：`licenses/FFmpeg-BUILD-README.txt`

Video Asset Organizer 通过子进程调用独立的 FFmpeg 可执行文件，未将 FFmpeg
库链接进应用程序。

## pyJianYingDraft draft_crypto

`third_party/jianying_crypto/draft_crypto.py` 衍生自 pyJianYingDraft 项目的草稿
兼容模块，并进行了适配。该组件按 Apache License 2.0 使用，不是 MIT License。
完整许可证见 `licenses/pyJianYingDraft-Apache-2.0.txt`。

## Qt for Python / PySide6

界面使用 Qt for Python（PySide6）。PySide6 可在 LGPLv3、GPLv3 或商业许可下使用；
本发布包使用其动态库形式，并保留对应许可证与版权文件。项目主页：
https://doc.qt.io/qtforpython-6/

## 其他 Python 依赖

本软件还使用 Python、requests、openpyxl、keyring 及其传递依赖。各组件保留其
原始许可证；正式发布包由干净构建环境生成，不包含开发缓存、用户设置或测试数据。
