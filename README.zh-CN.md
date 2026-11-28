# <img src="assets/icon.png" width="44" height="44" alt=""> QiaOrbit

### 连接更简单，流量有去向。

为 macOS 打造的原生代理客户端，把配置、分流和诊断放进同一个窗口。

<a href="https://github.com/ovralab/QiaOrbit/releases/latest"><img src="assets/buttons/download-zh.png" width="178" height="36" alt="下载 macOS 版"></a>&nbsp; <a href="https://minovra.app/products/qiaorbit"><img src="assets/buttons/website-zh.png" width="130" height="36" alt="官方网站"></a>

<p>
  <img src="https://img.shields.io/badge/macOS-14%2B-0066FF" alt="macOS 14+">
  <img src="https://img.shields.io/badge/Apple%20silicon-arm64-0066FF" alt="Apple silicon">
  <img src="https://img.shields.io/badge/SwiftUI-原生界面-0066FF" alt="SwiftUI">
  <img src="https://img.shields.io/badge/Developer%20ID-签名-2EA44F" alt="Developer ID">
  <img src="https://img.shields.io/badge/Apple-公证-2EA44F" alt="Notarized">
</p>

<img src="https://img.shields.io/github/v/release/ovralab/QiaOrbit?label=%E6%9C%80%E6%96%B0%E7%89%88&color=0066FF" alt="最新版"> · [English](README.md)

<img src="assets/screenshots/dashboard.png" width="820" alt="控制台：连接状态、实时速率、网络诊断与分流策略">

---

## 为什么选择 QiaOrbit

- **规则看得懂。** 网站、IP、应用三类规则，直连、代理、拦截三种动作；每条连接命中了哪条规则，都能在记录里逐条查到，不用凭感觉判断。
- **两种接管方式。** 「系统代理」适合遵循 macOS 代理设置的应用；「虚拟网卡」通过已签名的系统扩展接管全部流量，包括不认系统代理的应用。
- **先诊断，再判断。** 切节点前先看延迟与稳定性；出问题时还有 DNS、节点、代理、分流四项检查，把「连上了但打不开」拆开定位。

---

## 功能一览

| 模块 | 说明 |
|---|---|
| **分流** | 我的规则、应用规则、AI 服务、常用服务、其他流量五层。改规则热生效，不用断开连接。 |
| **配置** | 支持 ClashMeta / Mihomo 订阅与本地 YAML、链接导入、二维码导入、按配置自动更新、用量与到期提醒。 |
| **节点** | 按地区分组，延迟分三档着色，稳定性多次采样，另有 AI 可达性一列。 |
| **记录** | 每次连接都记录应用、目标、命中规则与连接方式；支持导出 CSV 与保留天数设置。 |
| **隐私** | 无需注册账号；配置与记录只保存在本机；诊断不会上传你的配置。 |

---

## 规则到底生效了没有

左：规则编辑，直连 / 代理 / 拦截。右：连接记录，逐条显示命中的规则。

<p>
  <img src="assets/screenshots/rules-zh-CN.png" width="47%" alt="流量规则：直连 / 代理 / 拦截">
  &nbsp;
  <img src="assets/screenshots/history-zh-CN.png" width="47%" alt="连接记录：逐条显示命中的规则">
</p>

---

## 技术实现

| 层 | 实现 |
|---|---|
| **界面** | SwiftUI，macOS 14+，浅色设计系统，尺寸与颜色统一走 token |
| **内核** | mihomo（Clash Meta）：虚拟网卡模式下进程内嵌；系统代理模式下作为受管子进程运行 |
| **隧道** | `NEPacketTunnelProvider` 系统扩展，数据包通过 C ABI 交给内核 |
| **签名** | Developer ID + Hardened Runtime + 安全时间戳，Apple 公证，Sparkle EdDSA 更新校验 |

---

## 开始使用

1. 打开 DMG，把 **QiaOrbit** 拖到「应用程序」。
2. 导入 ClashMeta / Mihomo 订阅或本地配置，选一个节点。
3. 按需打开「系统代理」或「虚拟网卡」。首次开虚拟网卡时，在系统弹窗里允许网络扩展。
4. 到「流量规则」里调整分流，改完立即生效，不需要重连。

> **环境要求**：macOS 14.0 或更高 · Apple 芯片 · 虚拟网卡需在「系统设置 → 通用 → 登录项与扩展 → 网络扩展」中允许 QiaOrbit。

---

## 常见问题

<details>
<summary>QiaOrbit 提供节点或订阅吗？</summary>

不提供。它是客户端，需要你自己准备 ClashMeta / Mihomo 配置、订阅或节点链接。
</details>

<details>
<summary>系统代理和虚拟网卡怎么选？</summary>

系统代理只覆盖遵循 macOS 代理设置的应用；虚拟网卡接管全部流量，包括不认系统代理的应用，但需要在系统设置里允许网络扩展。
</details>

<details>
<summary>我的数据存在哪里？</summary>

配置、规则和连接记录都在 `~/Library/Application Support/QiaOrbit`。没有账号体系，也不会上传云端。
</details>


---

## 相关链接

- 官方网站 · <https://minovra.app/products/qiaorbit>
- 更新日志 · [Releases](https://github.com/ovralab/QiaOrbit/releases)
- 规则仓库 · [ovralab/Qiaorbit-rules](https://github.com/ovralab/Qiaorbit-rules)
- 支持邮箱 · <support@minovra.app>

---

<sub>© 2026 Minovra · 隐私政策 · 服务条款 · 第三方声明</sub>
