* # 🛠️ KyleaZhu Config

  **自动化网络优化与代理配置文件集锦。**

  ### 🌟 核心功能

  - **☁️ Cloudflare 优选 (自动更新)**
    - **IP 优选**：每小时更新电信、联通、移动及三网优选 IP。
    - **域名优选**：每日更新全球高速 CF 节点域名。
  - **📺 B 站换源 (CCB)**
    - **防 PCDN**：网页端强制切换优质企业级 CDN。
    - **动态节点**：支持实时同步云端存活边缘节点（`Alive_CDN.json`）。
  - **🚀 代理配置 (AIO)**
    - **Mihomo/Clash**：集成 AI、Telegram、YouTube 专用分流规则及自动测速组。
    - **OpenClash**：支持国内直连与国际通信的自动化配置。

  ------

  ### 📥 快速链接

  - **B 站优化脚本**：[点击安装 (Tampermonkey)](https://www.google.com/search?q=https://testingcf.jsdelivr.net/gh/KyleaZhu/Config@main/Custom%20CDN%20of%20Bilibili%20-%20%E7%BD%91%E9%A1%B5%E8%A7%86%E9%A2%91-%E7%9B%B4%E6%92%AD%E6%8D%A2%E6%BA%90.user.js)
  - **CF 优选 IP**：[Raw 链接](https://www.google.com/search?q=https://raw.githubusercontent.com/KyleaZhu/Config/main/bestcf/ip.txt)
  - **CF 优选域名**：[Raw 链接](https://www.google.com/search?q=https://raw.githubusercontent.com/KyleaZhu/Config/main/bestcf/domain.txt)

  ------

  ### 📂 目录说明

  - `bestcf/`：CF 优选产出数据（`ip.txt`, `domain.txt`）。
  - `Alive_CDN.json`：直播存活边缘节点库。
  - `MihomoAIO.yaml`：Mihomo 全能配置文件。
  - `.github/workflows/`：自动化更新脚本。

  ------

  **License**: [MIT](https://www.google.com/search?q=LICENSE)
