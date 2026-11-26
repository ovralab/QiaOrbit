# QiaOrbit

**Decide how your Mac’s traffic is routed. See what happens to each connection.**

QiaOrbit brings proxy profiles, traffic rules, and connection diagnostics into one macOS app. Import your own configuration, choose a node, and see which rules matched when you need to troubleshoot a connection.

[Download for Apple Silicon](https://github.com/ovralab/QiaOrbit/releases/latest) · [Product page](https://minovra.app/products/qiaorbit) · [简体中文](README.zh-CN.md)

Requires macOS 14 or later.

## The dashboard

![QiaOrbit dashboard with connection controls, network diagnostics, and subscription usage](assets/screenshots/dashboard.png)

From the dashboard, you can switch nodes, check your outbound IP and traffic rates, and see whether DNS, the selected node, and the proxy service are working.

## From profile to connection

1. **Add a profile.** Open the DMG, drag QiaOrbit into Applications, and import a ClashMeta / Mihomo subscription or a local configuration file.
2. **Choose what to route.** Use System Proxy for apps that follow macOS proxy settings. To route system traffic with the virtual network interface (TUN), enable it and approve the network extension when prompted.
3. **Choose where traffic goes.** Use Smart Routing to apply built-in and custom rules for domains, IP addresses, or apps. Switch to Global Proxy or Direct when you want a single policy.

## When a connection isn’t working

Compare node latency and stability, check the network diagnostics, or open Connection History to see which rule matched. The dashboard also shows traffic rule counts and subscription usage when available.

<a href="assets/screenshots/dashboard-rules.png"><img src="assets/screenshots/dashboard-rules.png" width="620" alt="QiaOrbit dashboard showing traffic rule counts and subscription usage"></a>

QiaOrbit is a commercial app. You supply your own profiles, proxy nodes, or subscriptions.

[Contact Minovra support](mailto:support@minovra.app) for help or feedback. Include your macOS and QiaOrbit versions and a brief description of the issue.
