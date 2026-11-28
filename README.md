# <img src="assets/icon.png" height="44" align="middle" alt="">&nbsp; <img src="assets/wordmark.png" height="44" align="middle" alt="QiaOrbit">

**A native macOS client for proxy connections and traffic routing**

Import a profile, route traffic by website or app, and see how each connection was handled.

<a href="https://github.com/ovralab/QiaOrbit/releases/latest"><img src="assets/buttons/download-en.png" width="200" height="36" alt="Download for macOS"></a>&nbsp; <a href="https://minovra.app/products/qiaorbit"><img src="assets/buttons/website-en.png" width="180" height="36" alt="Official website"></a>

macOS 14+ · Apple silicon&nbsp; <sup><a href="https://github.com/ovralab/QiaOrbit/releases/latest"><img src="https://img.shields.io/github/v/release/ovralab/QiaOrbit?label=Current%20version&amp;labelColor=0066FF&amp;color=white&amp;style=flat-square" height="20" align="middle" alt="Current release"></a></sup>&nbsp; · [简体中文](README.zh-CN.md)

<img src="assets/screenshots/dashboard.png" width="820" alt="QiaOrbit dashboard showing connection status, traffic, network diagnostics, and routing rules">

## Core features

| Feature | What you can do |
| --- | --- |
| **Rule-based routing** | Set direct, proxy, or block rules for domains, IP addresses, or apps. |
| **Two connection methods** | Choose System Proxy or the virtual network interface (TUN). |
| **Node testing and switching** | Compare latency and stability, and check whether common AI services are reachable. |
| **Connection history** | See the actual route and matching rule. Search, filter, and export records to CSV. |

## See where each connection went

Search Connection History by app or destination to see whether a connection went direct, used a proxy, or was blocked, and which rule matched.

<img src="assets/screenshots/history-en.png" width="820" alt="QiaOrbit Connection History showing apps, destinations, connection methods, and matched rules">

<details>
<summary>View the traffic rules screen</summary>

<img src="assets/screenshots/rules-zh-CN.png" width="820" alt="QiaOrbit traffic rules screen in Chinese, with direct, proxy, and block options">

</details>

## App specifications

| Item | Details |
| --- | --- |
| Interface | Native macOS interface built with SwiftUI |
| Core | Mihomo (Clash.Meta) |
| Signing and notarization | Developer ID signing and Apple notarization |

## Get started

1. Open the DMG and drag QiaOrbit into Applications.
2. Import a ClashMeta / Mihomo subscription or local configuration, then choose a node. QiaOrbit does not provide nodes or subscriptions.
3. Enable System Proxy or TUN as needed. If you enable TUN, approve the network extension when macOS prompts you.

<details>
<summary>When should I use System Proxy or TUN?</summary>

Use System Proxy for apps that follow macOS proxy settings. Choose TUN to route system traffic after you approve the network extension.

</details>

<details>
<summary>Where are my profiles and connection history stored?</summary>

Profiles, rules, and connection history are stored on your Mac in `~/Library/Application Support/QiaOrbit`.

</details>

[Official website](https://minovra.app/products/qiaorbit) · [Release notes](https://github.com/ovralab/QiaOrbit/releases) · [Rules repository](https://github.com/ovralab/Qiaorbit-rules) · [Support](mailto:support@minovra.app)

<sub>© 2026 Minovra</sub>
