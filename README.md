# 🎬雷神视频无声片段剪辑器 (Auto-Editor Ultimate GUI)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey.svg)

基于强大的命令行工具 `auto-editor` 打造的**全图形化、零门槛、支持显卡加速**的视频极速粗剪神器。彻底告别枯燥的命令行输入与 CPU 漫长的渲染等待！

## ✨ 核心亮点

本项目针对个人创作者和自媒体矩阵的工作流痛点进行了深度重构：

* **⚡️ 毫秒级工程导出：** 独家打通 DaVinci Resolve (达芬奇)、Premiere、剪映的 XML/FCPXML 跨软件工作流。无需二次渲染，几秒钟内生成带切割点的时间线图纸。
* **🎮 彻底解锁 GPU 硬件加速：** 完美适配 AMD (`h264_amf`) 与 NVIDIA (`h264_nvenc`) 显卡。导出实体 MP4 视频时，利用硬件编码器将速度提升数倍！
* **🖱️ 极简图形界面：** 采用单选框优化交互，彻底解决长文本下拉菜单不灵敏问题；去除多余下载步骤，一键原生调用 Windows 资源管理器直达成品文件夹。
* **📦 开箱即用 (免环境配置)：** 提供独立打包的 `.exe` 绿色免安装版，内置所需所有环境，双击即用！

## 🚀 最佳工业级工作流建议 (强烈推荐)

如果你追求极致的出片效率，请抛弃直接导出 MP4 的传统方式，尝试这套**“降维打击”**流派：

1.  将视频拖入本软件，选择导出格式为 **“达芬奇 / DaVinci Resolve (.xml)”** 或 **“剪映 / Premiere (.xml)”**。
2.  点击执行，**仅需数秒**即可完成音频分析与静音片段切割，生成 `.xml` / `.fcpxml` 纯数据图纸。
3.  打开达芬奇或剪映等专业后期软件，导入该 XML 文件。
4.  时间线上已自动剔除所有卡壳、无声的废话片段。直接加字幕、渲染，享受专业软件的极致渲染速度！

## 📥 下载与安装 (普通用户)

1. 前往右侧的 **[Releases](#)** 页面（请在这里放上你的 Releases 链接）。
2. 下载最新版本的 `雷神极速剪辑器_vX.X.zip`。
3. 解压到任意目录，**双击 `ui_auto_editor.exe`** 即可自动在浏览器中打开图形界面。

## 🛠️ 本地运行与二次开发 (开发者)

如果你想自己修改源码并运行，请确保已安装 Python 环境：

```bash
# 1. 克隆本仓库
git clone [https://github.com/你的用户名/你的仓库名.git](https://github.com/你的用户名/你的仓库名.git)
cd 你的仓库名

# 2. 安装依赖框架
pip install gradio auto-editor

# 3. 运行界面
python ui_auto_editor.py
