# 🎨 PluginStyler

[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011-blue)](https://www.microsoft.com/windows)
[![.NET](https://img.shields.io/badge/.NET-8.0-purple)](https://dotnet.microsoft.com/)
[![Release](https://img.shields.io/github/v/release/kasnowww147/PluginStyler)](../../releases)

[English](#english) | [中文 (Chinese)](#chinese)

---

<a name="english"></a>
## 🇺🇸 English Description

**PluginStyler** is a specialized Windows utility designed for music producers using **Bitwig Studio** and **Ableton Live**.

It leverages the **Desktop Window Manager (DWM)** and low-level Win32 APIs to modernize the appearance of floating plugin (VST/CLAP) windows. By injecting attributes such as **Mica material** (Win11) and custom accent borders, PluginStyler integrates third-party plugins visually into the DAW environment, creating a cohesive and native look.

> **Note:** This repository serves as the official distribution channel and issue tracker for PluginStyler.

### ✨ Key Features

* **🪟 Advanced Window Styling**
    * **Mica Material:** Applies Windows 11 "Mica" backdrop effects to plugin frames (Windows 11 only).
    * **Geometry Control:** Customizable corner radius (Square, Small, or Round).
    * **Minimalist Aesthetics:** Option to hide native title bar text for a cleaner workspace.
* **🎨 Dynamic Coloring**
    * **State Awareness:** Distinct visual themes for **Active** (focused) and **Inactive** windows.
    * **Rainbow Mode:** Smooth RGB color cycling for window borders with adjustable saturation.
    * **Custom Palettes:** Manage and persist custom color configurations.
* **👻 Transparency Control**
    * Independent opacity settings for active vs. inactive states.
    * "See-through" capability for unfocused plugins to improve workflow visibility.
* **⚙️ Architecture & Performance**
    * **Smart Window Filtering:** Intelligently targets plugin containers (e.g., Bitwig `pluginhost`) while strictly excluding the main DAW interface to prevent UI conflicts.
    * **Zero Audio Interference:** Utilizes **debounced WinEvent hooks** and **cached PID lookups** to ensure **negligible (~0%) CPU impact** on real-time audio processing.
    * **Robust Configuration:** JSON-based preset system for saving and loading user preferences.

### 📥 Installation

1.  Navigate to the [Releases](../../releases) page.
2.  Download the latest `PluginStyler.zip`.
3.  Extract the archive to a permanent location.
4.  Run `PluginStyler.exe`.
5.  *(Optional)* Enable "Run on Startup" in the settings.

### ⚠️ Compatibility & Limitations

* **Windows 11 (Build 22000+):** Supports full features including **Mica effects**, Corner Radius, Colors, and Transparency.
* **Windows 10 (1809+):** Supports **Custom Colors** and **Transparency**. (Mica effects are not available on Windows 10 due to OS limitations).
* **Client-Side Decoration:** Plugins that draw their own custom title bars (non-standard Windows frames) may not support DWM coloring.

### 💬 Feedback & Support

If you encounter any bugs or have suggestions for new features, please submit an issue on the [Issues](../../issues) page.

---

<a name="chinese"></a>
## 🇨🇳 中文介绍

**PluginStyler** 是一款专为 **Bitwig Studio** 和 **Ableton Live** 用户设计的 Windows 窗口美化工具。

通过调用 **桌面窗口管理器 (DWM)** 和底层 Win32 API，PluginStyler 能够让悬浮的插件窗口（VST/CLAP）拥有现代化的外观。它可以为插件注入 **Mica (云母)** 材质（仅限 Win11）以及自定义边框颜色，使第三方插件在视觉上与 DAW 完美融合。

> **说明：** 本仓库是 PluginStyler 的官方发布下载页及问题反馈中心。

### ✨ 核心功能

* **🪟 高级窗口样式**
    * **Mica 材质：** 为插件窗口启用 Windows 11 的 "Mica" 背景效果（Windows 10 仅支持纯色）。
    * **几何控制：** 可自定义窗口圆角风格（直角、小圆角或大圆角）。
    * **极简标题：** 支持隐藏原生标题栏文字，让界面更加清爽。
* **🎨 动态色彩管理**
    * **状态感知：** 分别定义 **激活 (Active)** 和 **非激活 (Inactive)** 窗口的视觉主题。
    * **RGB 彩虹模式：** 支持平滑的动态 RGB 颜色循环边框，色彩饱和度可调。
    * **色板管理：** 保存并管理您常用的自定义颜色配置。
* **👻 透明度控制**
    * 独立控制激活与非激活窗口的透明度。
    * 支持非焦点窗口半透明，提升多任务工作流的可视性。
* **⚙️ 架构与性能**
    * **智能过滤：** 精确识别插件宿主进程（如 Bitwig 的 `pluginhost`），同时严格排除 DAW 主窗口，避免界面冲突。
    * **零音频干扰：** 采用 **去抖动 (Debounce) 事件钩子** 和 **PID 缓存机制**，确保对实时音频处理 **近乎 0% 的 CPU 占用**。
    * **配置系统：** 基于 JSON 的预设管理系统，支持保存和读取用户配置。

### 📥 安装指南

1.  前往 [Releases](../../releases) 页面。
2.  下载最新的 `PluginStyler.zip` 压缩包。
3.  解压到任意永久文件夹。
4.  运行 `PluginStyler.exe`。
5.  *(可选)* 在设置中开启 "开机自启"。

### ⚠️ 兼容性与限制

* **Windows 11 (Build 22000+)：** 支持所有功能，包括 **Mica 云母材质**、圆角修改、自定义颜色和透明度。
* **Windows 10 (1809+)：** 支持 **自定义颜色** 和 **透明度**。（由于系统限制，Windows 10 无法显示 Mica 材质效果）。
* **自定义标题栏：** 部分完全自绘标题栏（非标准 Windows 边框）的插件可能无法支持 DWM 着色。

### 💬 反馈与支持

如果您在使用过程中遇到任何问题或有功能建议，请前往 [Issues](../../issues) 页面提交反馈。

---

## © Copyright

Copyright © 2025. All Rights Reserved.
