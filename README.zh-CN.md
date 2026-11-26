# QiaOrbit

**决定 Mac 上的流量走哪条线路，也能查到每条连接命中了什么规则。**

QiaOrbit 是一款 macOS 代理客户端，把代理配置、流量规则和连接诊断放在同一个应用里。导入配置、选好节点后即可连接。遇到问题时，可以从控制台和连接记录入手排查。

[下载 Apple 芯片版](https://github.com/ovralab/QiaOrbit/releases/latest) · [官网产品页](https://minovra.app/zh-CN/products/qiaorbit) · [English](README.md)

需要 macOS 14 或更高版本。

## 控制台

![QiaOrbit 控制台展示连接开关、网络诊断和订阅用量](assets/screenshots/dashboard.png)

你可以在控制台切换节点，查看出站 IP 和实时速率，并检查 DNS、节点连通性和代理服务状态。

## 从导入配置到开始连接

1. **导入配置。** 打开 DMG，将 QiaOrbit 拖入「应用程序」，再导入 ClashMeta / Mihomo 订阅或本地配置文件。
2. **选择接管范围。** 系统代理适用于遵循 macOS 代理设置的应用。如果要接管系统流量，请启用虚拟网卡（TUN），并按系统提示允许网络扩展。
3. **决定流量去向。** 智能分流会按内置规则和自定义规则处理流量。规则可按域名、IP 或应用设置，也可以直接切换为全局代理或全局直连。

## 连接不顺时怎么查

先比较节点的延迟和稳定性，或查看网络诊断。如果只有某个网站或应用受影响，可以打开「连接记录」，看看相关连接命中了哪条规则。控制台也能查看规则统计和订阅用量。

<a href="assets/screenshots/history-zh-CN.png"><img src="assets/screenshots/history-zh-CN.png" width="620" alt="QiaOrbit 连接记录展示连接方式和命中依据"></a>

QiaOrbit 是商业软件，配置、代理节点或订阅需自行准备。

如需帮助或反馈问题，请[联系 Minovra 支持](mailto:support@minovra.app)，并附上 macOS 版本、QiaOrbit 版本和问题描述。
