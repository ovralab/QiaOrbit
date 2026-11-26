<p align="center"><img src="assets/icon.png" width="88" alt="QiaOrbit icon"></p>

<h1 align="center">QiaOrbit</h1>
<p align="center">A macOS proxy client for managing profiles, routing traffic, and diagnosing connections.</p>
<p align="center"><strong>English</strong> · <a href="README.zh-CN.md">简体中文</a></p>
<p align="center"><a href="https://minovra.app/products/qiaorbit">Official website</a> · <a href="https://github.com/ovralab/QiaOrbit/releases/latest">Download</a> · <a href="mailto:support@minovra.app">Support</a></p>

![QiaOrbit dashboard showing connection status, outbound modes, network diagnostics, and subscription usage](assets/screenshots/dashboard.png)

## Features

- **Connection modes.** Use System Proxy for apps that respect system proxy settings, or enable the virtual network interface (TUN) to route system traffic.
- **Traffic rules.** Choose Smart Routing, Global Proxy, or Direct mode. Use built-in rules or define rules for domains, IP addresses, and apps.
- **Profiles and nodes.** Import a ClashMeta / Mihomo subscription or a local configuration file. Switch nodes and compare their latency and stability.
- **Connection diagnostics.** Check DNS resolution, node reachability, proxy service status, and routing. Review recent connections to see which rules matched.

<details>
<summary>View another dashboard screenshot</summary>

![QiaOrbit dashboard showing traffic rule counts and subscription usage](assets/screenshots/dashboard-rules.png)

</details>

## Download and installation

The macOS build requires **macOS 14 or later** and an **Apple Silicon Mac**. Get the DMG from [GitHub Releases](https://github.com/ovralab/QiaOrbit/releases/latest) or visit the [official product page](https://minovra.app/products/qiaorbit).

1. Open the DMG and drag QiaOrbit into Applications.
2. Open QiaOrbit, import a profile or subscription, and choose a node.
3. If you enable the virtual network interface, approve the QiaOrbit network extension when macOS prompts you.

QiaOrbit is a commercial client. Bring your own profiles, proxy nodes, or subscriptions.

For help or feedback, [contact Minovra support](mailto:support@minovra.app). Include your macOS and QiaOrbit versions and a brief description of the issue.
