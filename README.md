# 🛠️ KyleaZhu Config

**自动化网络优化与代理配置文件集锦。**

### 🌟 核心功能

- **☁️ Cloudflare 优选 (自动更新)**
  - **IP 优选**：每小时更新三网优选 IP (`bestcf/ip.txt`)。
  - **域名优选**：每日更新全球高速 CF 节点域名 (`bestcf/domain.txt`)。
- **📺 B 站换源 (CCB)**
  - **防 PCDN**：网页端强制切换优质企业级 CDN。
  - **动态节点**：同步云端存活边缘节点库 (`data/alive-bili-cdn-nodes.json`)。
- **🚀 代理配置 (AIO)**
  - **Mihomo/Clash**：全能分流规则及自动测速组 (`proxy-configs/MihomoAIO.yaml`)。
  - **OpenClash**：国内直连与国际通信自动化配置。

------

### 📥 快速链接

- **B 站优化脚本**：[点击安装 (Tampermonkey)](https://raw.githubusercontent.com/KyleaZhu/Config/main/scripts/bilibili-cdn-switch.user.js)
- **CF 优选 IP**：[Raw 链接](https://raw.githubusercontent.com/KyleaZhu/Config/main/bestcf/ip.txt)
- **CF 优选域名**：[Raw 链接](https://raw.githubusercontent.com/KyleaZhu/Config/main/bestcf/domain.txt)

------

### 📂 目录说明

- `bestcf/`：CF 优选产出数据。
- `data/`：B 站 CDN 节点库（含存活节点与静态节点）。
- `proxy-configs/`：主流代理工具配置文件。
- `scripts/`：B 站换源等实用脚本。
- `.github/workflows/`：自动化更新脚本。

------

**License**: [MIT](LICENSE)
