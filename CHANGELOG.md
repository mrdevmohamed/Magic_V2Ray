# Release Notes — v1.20

Magic V2Ray v1.20 brings significant feature additions, system-level enhancements, and UI improvements focused on application control, network compatibility, and log handling.

The release introduces the Exclude Apps feature, allowing specific applications to bypass the proxy entirely and connect directly at the OS level. The system handles list management through the WebUI, dynamically updates IPTables rules, and uses inotify to automatically process app installs or uninstalls in real time.

IPv6 routing capabilities are expanded with support for IPv6 ULA Decoy. When active, a local-only Unique Local Address is advertised on the active interface so applications recognize IPv6 connectivity even on IPv4-only physical networks, keeping IPv6 socket support intact while funneling traffic safely through Xray.

Log handling receives a dedicated daemon service, moving away from simple tail operations to provide smooth, real-time log streaming and memory-safe buffer management. The log view in the WebUI is upgraded with adjustable font sizing, word-wrap toggles, and improved styling.

Additionally, outbound TLS configurations now support peer certificate verification by name (`verifyPeerCertByName`), and ECH configuration parameters have been extended to Hysteria2 links. The network latency monitor has also been updated to operate directly with the lifecycle of its WebUI tab, automatically running when opened and stopping upon leaving.

---

[Click here for older release notes](https://github.com/vincentng295/Magic_V2Ray/releases)