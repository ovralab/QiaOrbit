# QiaOrbit

**设置 Mac 的流量分流，查清每条连接走了哪里。**

QiaOrbit 把配置管理、流量规则和网络诊断放在同一个 macOS 应用里。

[![下载 macOS 版](https://img.shields.io/badge/%E4%B8%8B%E8%BD%BD%20macOS%20%E7%89%88-0059C7?style=for-the-badge)](https://github.com/ovralab/QiaOrbit/releases/latest)
[![官方网站](https://img.shields.io/badge/%E5%AE%98%E6%96%B9%E7%BD%91%E7%AB%99-384657?style=for-the-badge)](https://minovra.app/zh-CN/products/qiaorbit)

macOS 14 或更高版本 · Apple 芯片 | [English](README.md)

![QiaOrbit 控制台展示节点选择、流量和网络诊断](assets/screenshots/dashboard.png)

## 查清每条连接的去向

打开「连接记录」，就能看到访问是直连、走代理还是被拦截，以及命中的规则。

[![连接记录展示直连、代理和命中的规则](assets/screenshots/history-zh-CN.png)](assets/screenshots/history-zh-CN.png)

**按需设置分流**
导入 ClashMeta / Mihomo 订阅或本地配置，可按域名、IP 或应用设置规则。

**选择接管方式**
系统代理适用于遵循 macOS 代理设置的应用。需要接管系统流量时，可开启虚拟网卡（TUN）。

**比较节点质量**
比较节点的延迟和稳定性，并在控制台检查 DNS 和节点连通性。

## 安装与使用

1. 下载 DMG，将 QiaOrbit 拖入「应用程序」。
2. 打开 QiaOrbit，导入配置并选择节点。
3. 如需使用虚拟网卡，请按 macOS 提示允许网络扩展。

QiaOrbit 是商业软件，配置、代理节点或订阅需自行准备。 [联系技术支持](mailto:support@minovra.app).
