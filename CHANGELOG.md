# Release Notes — v1.15

We are excited to announce the release of **Magic V2Ray v1.15**! This update introduces a dedicated Custom Hosts management tab, full support for custom blocklists such as AdGuard and AdBlock, file path storage at `/data/adb/magic_v2ray/hosts`, and live outbound IP checking directly from the status badge.

## What's New

### Dedicated Custom Hosts Tab

The Web UI now features a dedicated Custom Hosts tab, allowing you to easily view, search, add, edit, and delete domain-to-IP mappings. Custom rules are saved and loaded directly from `/data/adb/magic_v2ray/hosts` using the standard `/etc/hosts` format (`IP hostname`), making them human-readable and easy to manage manually or via external scripts. The interface includes an in-memory search bar and lazy-loaded rendering to maintain smooth performance even when handling large AdGuard or AdBlock lists. All entries are seamlessly merged into Xray's `dns.hosts` configuration on top of default resolutions, with support for removing built-in defaults using the `!` prefix.

### Live IP Check & Active Node Badge

The header status badge now displays the label of your active proxy node, built-in direct routing, or custom configuration mode. By simply tapping the status badge, the app queries `icanhazip.com` via Xray's SOCKS5 test inbound to immediately verify your active public IP address.

---

[Click here for older release notes](https://github.com/vincentng295/Magic_V2Ray/releases?utm_source=gemini)