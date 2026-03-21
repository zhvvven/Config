# 📺 Custom CDN of Bilibili (CCB) - 网页视频/直播换源

![Version](https://img.shields.io/badge/Version-3.4.0-blue.svg) ![License](https://img.shields.io/badge/License-MIT-green.svg) ![Author](https://img.shields.io/badge/Author-KyleaZhu-orange.svg)

> **极简、纯净的 B 站防 PCDN 与强制换源油猴脚本。**

## 📝 项目简介

本项目是基于开源项目 [Custom CDN of Bilibili (CCB)](https://github.com/Kanda-Akihito-Kun/ccb) 进行精简与重构的版本。

针对网页端视频与直播的不同业务特性，本脚本采用了 **“静态中心源 + 动态边缘源”** 的混合架构：
* **视频点播**：剥离外部网络依赖，将精选的国内优质企业级 CDN（阿里、腾讯、华为等）直接硬编码在脚本内部，实现快速加载。
* **直播换源**：支持动态拉取机制，实时同步云端托管的存活下沉边缘节点（`Alive_CDN.json`）。通过直观的 “**运营商 ➔ 地名 ➔ 节点**” 三级联动 UI，方便手动匹配同城宽带，解决直播卡顿与 PCDN 上传问题。

## ✨ 核心特性

* **🚀 混合架构**：视频与直播模块彻底解耦，静态高速池与动态测速池互不干扰。
* **⚡ 动态边缘节点 (Live)**：无缝对接云端 `Alive_CDN.json` 节点库。支持按“电信/联通/移动/广电/教育网”及“具体地名”进行三级级联筛选。
* **💎 精选私有池 (Video)**：内置官方 CDN 节点，无需请求第三方 API，轻量纯净。
* **⚙️ 底层拦截**：完美 Hook 底层 `window.fetch`、`XMLHttpRequest` 及 `Worker`、`Blob` 运行环境，确保换源指令全局生效。
* **📊 状态显示**：油猴菜单实时显示双端状态（如 `配置 B 站换源 (视频: mirrorali | 直播: cq-bcdn)`），方便查看当前路由。

---

## 📦 安装指南

请确保你的浏览器已安装 [Tampermonkey (油猴)](https://www.tampermonkey.net/) 扩展程序。

点击下方任意一个链接即可唤起安装界面。根据你的网络环境，选择加载速度最快的链接：

* 🔗 **[TestingCF CDN 加速链接](https://testingcf.jsdelivr.net/gh/KyleaZhu/Config@main/Custom%20CDN%20of%20Bilibili%20-%20网页视频-直播换源.user.js)**
* 🔗 **[JSDelivr CDN 备用链接](https://cdn.jsdelivr.net/gh/KyleaZhu/Config@main/Custom%20CDN%20of%20Bilibili%20-%20网页视频-直播换源.user.js)**
* 🔗 **[GitHub 原始链接](https://raw.githubusercontent.com/KyleaZhu/Config/main/Custom%20CDN%20of%20Bilibili%20-%20网页视频-直播换源.user.js)**

---

## 💻 使用说明

1. 安装脚本后，打开任意 [Bilibili 视频](https://www.bilibili.com/video/) 或 [直播间](https://live.bilibili.com/) 页面。
2. 点击浏览器右上角的 **Tampermonkey** 扩展图标。
3. 在弹出的菜单中，点击 **`配置 B 站换源 (视频: xxx | 直播: yyy)`**。
4. 在呼出的控制面板中进行配置：
   * **网页视频换源**：直接在下拉菜单中选择你偏好的官方优质节点（如 `阿里云 CDN (mirrorali)`）。
   * **直播换源**：等待 1 秒钟加载云端节点库后，依次选择你的「**宽带运营商**」➔「**所在省市**」➔「**同城节点**」。
5. 点击底部的 **“应用并刷新”** 按钮即可。

## 🤝 鸣谢与许可

* **Original Author**: [鼠鼠今天吃嘉然](https://github.com/Kanda-Akihito-Kun/ccb) 
* **Modified & Rebuilt By**: KyleaZhu
* **License**: 本项目基于 **[MIT License](LICENSE)** 开源。
