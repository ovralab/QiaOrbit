# <img src="assets/icon.png" height="44" align="middle" alt="">&nbsp; <img src="assets/wordmark.png" height="44" align="middle" alt="QiaOrbit">

**Native macOS proxy and routing client**

Import a configuration, route by website or app, and see where each connection actually went.

<a href="https://github.com/ovralab/QiaOrbit/releases/latest/download/QiaOrbit.dmg"><img src="assets/buttons/download-en.png" width="200" height="36" alt="Download for macOS"></a>&nbsp; <a href="https://minovra.app/products/qiaorbit"><img src="assets/buttons/website-en.png" width="180" height="36" alt="Official website"></a>

macOS 14+ · Apple silicon&nbsp; <sup><a href="https://github.com/ovralab/QiaOrbit/releases/latest"><img src="https://img.shields.io/github/v/release/ovralab/QiaOrbit?label=Version&amp;labelColor=0066FF&amp;color=white&amp;style=plastic" height="20" align="middle" alt="Current release"></a></sup>&nbsp; · <a href="README.zh-CN.md"><  align="middle" alt="简体中文"></a>

<img src="assets/screenshots/dashboard-en.png" width="820" alt="QiaOrbit dashboard showing connection state, live throughput, network diagnostics and routing policy">

## Core features

| Feature | What it does |
| --- | --- |
| **Rule-based routing** | Set direct, proxy, or block per domain, IP address, or app. |
| **Two ways to take over traffic** | Use System Proxy or the virtual network interface (TUN), depending on your needs. |
| **Node testing and switching** | Compare latency and stability, and check availability of common AI services. |
| **Connection history** | See the actual egress path and the rule that matched; search, filter, and export to CSV. |

## See where every connection went

In **History**, search by app or destination to see whether traffic went direct, through the proxy, or was blocked — and which rule matched.

<img src="assets/screenshots/history-en.png" width="820" alt="QiaOrbit connection history listing app, destination, method and matched rule">

<details>
<summary>View the traffic rules screen</summary>

<img src="assets/screenshots/rules-en.png" width="820" alt="QiaOrbit traffic rules screen showing direct, proxy and block rules">

</details>

## App specifications

| Item | Details |
| --- | --- |
| Interface | Native macOS interface built with SwiftUI |
| Core | Mihomo (Clash.Meta) |
| Signing | Developer ID signing and Apple notarization |

## Get started

1. Open the DMG and drag QiaOrbit into Applications.
2. Import a ClashMeta / Mihomo subscription or local configuration, then select a node. QiaOrbit does not provide nodes or subscriptions.
3. Enable System Proxy or TUN as needed. The first time you enable TUN, approve the network extension when macOS asks.

<details>
<summary>System Proxy or TUN — which one?</summary>

System Proxy covers apps that follow macOS proxy settings. TUN is for cases where system-wide traffic must be captured, and requires approving the network extension first.

</details>

<details>
<summary>Where are my configuration and connection history stored?</summary>

Configuration, rules, and connection history are stored locally in `~/Library/Application Support/QiaOrbit`.

</details>

[Official website](https://minovra.app/products/qiaorbit) · [Release notes](https://github.com/ovralab/QiaOrbit/releases) · [Rules repository](https://github.com/ovralab/Qiaorbit-rules) · [Support](https://minovra.app/support/new)

<sub>© 2026 Minovra</sub>
