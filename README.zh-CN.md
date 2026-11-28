# <img src="assets/icon.png" height="44" align="middle" alt="">&nbsp; <img src="assets/wordmark.png" height="44" align="middle" alt="QiaOrbit">

**原生 macOS 代理与分流客户端**

导入配置，按网站或应用设置分流，并查看每条连接的实际走向。

<a href="https://github.com/ovralab/QiaOrbit/releases/latest/download/QiaOrbit-1.0.1.dmg"><img src="assets/buttons/download-zh.png" width="182" height="36" alt="下载 macOS 版"></a>&nbsp; <a href="https://minovra.app/zh-CN/products/qiaorbit"><img src="assets/buttons/website-zh.png" width="146" height="36" alt="官方网站"></a>

macOS 14+ · Apple 芯片&nbsp; <sup><a href="https://github.com/ovralab/QiaOrbit/releases/latest"><img src="https://img.shields.io/github/v/release/ovralab/QiaOrbit?label=%E5%BD%93%E5%89%8D%E7%89%88%E6%9C%AC&amp;labelColor=0066FF&amp;color=FFFFFF&amp;style=flat" height="20" align="middle" alt="当前正式版本"></a></sup>&nbsp; · [English](README.md)

<img src="assets/screenshots/dashboard.png" width="820" alt="QiaOrbit 控制台，显示连接状态、实时速率、网络诊断与分流策略">

## 核心功能

| 功能 | 可以做什么 |
| --- | --- |
| **按规则分流** | 按域名、IP 或应用设置直连、代理或拦截。 |
| **两种接管方式** | 根据需要选择系统代理或虚拟网卡（TUN）。 |
| **节点检测与切换** | 比较节点延迟和稳定性，也可检测常用 AI 服务的可用性。 |
| **连接记录** | 查看实际出站方式和命中的规则，支持搜索、筛选和导出 CSV。 |

## 看清每条连接走了哪里

在「连接记录」中按应用或目标搜索，查看访问是直连、走代理还是被拦截，以及命中的规则。

<img src="assets/screenshots/history-zh-CN.png" width="820" alt="QiaOrbit 连接记录，逐条显示应用、目标、连接方式与命中依据">

<details>
<summary>查看流量规则界面</summary>

<img src="assets/screenshots/rules-zh-CN.png" width="820" alt="QiaOrbit 流量规则界面，展示直连、代理和拦截设置">

</details>

## 应用规格

| 项目 | 说明 |
| --- | --- |
| 界面 | 原生 macOS 界面，使用 SwiftUI 构建 |
| 内核 | Mihomo（Clash.Meta） |
| 签名与公证 | Developer ID 签名，Apple 公证 |

## 开始使用

1. 打开 DMG，将 QiaOrbit 拖入「应用程序」。
2. 导入 ClashMeta / Mihomo 订阅或本地配置，然后选择节点。QiaOrbit 不提供节点或订阅。
3. 按需启用系统代理或虚拟网卡。首次启用虚拟网卡时，请按 macOS 提示允许网络扩展。

<details>
<summary>系统代理和虚拟网卡怎么选？</summary>

系统代理适合遵循 macOS 代理设置的应用。虚拟网卡适合需要接管系统流量的场景，须先完成网络扩展授权。

</details>

<details>
<summary>我的配置和连接记录存在哪里？</summary>

配置、规则和连接记录保存在本机的 `~/Library/Application Support/QiaOrbit`。

</details>

[官方网站](https://minovra.app/zh-CN/products/qiaorbit) · [发行说明](https://github.com/ovralab/QiaOrbit/releases) · [规则仓库](https://github.com/ovralab/Qiaorbit-rules) · [技术支持](https://minovra.app/zh-CN/support/new)

<sub>© 2026 Minovra</sub>
