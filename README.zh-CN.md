<p align="center"><img src="assets/icon.png" width="88" alt="QiaOrbit 图标"></p>

<h1 align="center">QiaOrbit</h1>
<p align="center">面向 macOS 的代理客户端，用于管理配置、按规则分流和排查连接问题。</p>
<p align="center"><a href="README.md">English</a> · <strong>简体中文</strong></p>
<p align="center"><a href="https://minovra.app/zh-CN/products/qiaorbit">官网</a> · <a href="https://github.com/ovralab/QiaOrbit/releases/latest">下载</a> · <a href="mailto:support@minovra.app">技术支持</a></p>

![QiaOrbit 控制台展示连接状态、出站模式、网络诊断和订阅用量](assets/screenshots/dashboard.png)

## 主要功能

- **连接方式。** 使用系统代理接管遵循系统代理设置的应用，或开启虚拟网卡（TUN）接管系统流量。
- **流量规则。** 支持智能分流、全局代理和全局直连。可使用内置规则，也可按域名、IP 或应用自定义规则。
- **配置和节点。** 支持导入 ClashMeta / Mihomo 订阅和本地配置文件，可切换节点并比较延迟与稳定性。
- **连接诊断。** 检查 DNS 解析、节点连通性、代理服务与分流状态，并在连接记录中查看命中的规则。

<details>
<summary>查看另一张控制台截图</summary>

![QiaOrbit 控制台展示流量规则统计和订阅用量](assets/screenshots/dashboard-rules.png)

</details>

## 下载与安装

需要 **macOS 14 或更高版本**及搭载 **Apple 芯片**的 Mac。可从 [GitHub Releases](https://github.com/ovralab/QiaOrbit/releases/latest) 获取 DMG，或访问 [官网产品页](https://minovra.app/zh-CN/products/qiaorbit)。

1. 打开 DMG，将 QiaOrbit 拖入「应用程序」。
2. 打开 QiaOrbit，导入配置或订阅，然后选择节点。
3. 如需使用虚拟网卡，请在 macOS 提示时允许 QiaOrbit 网络扩展。

QiaOrbit 是商业客户端，配置、代理节点或订阅需自行准备。

如需帮助或反馈问题，请[联系 Minovra 支持](mailto:support@minovra.app)，并附上 macOS 版本、QiaOrbit 版本和问题描述。
