# Release Notes — v1.17.2

Add configurable Xray DNS engine options: The Traffic Settings tab now has a "DNS engine options" section for tuning Xray's built-in DNS module. You can disable the DNS cache, serve stale (expired) cache entries with a configurable lifetime, disable fallback queries, disable fallback when a server's domain list already matched, use parallel queries, and append the device hosts file. Parallel query is enabled by default to speed up resolving, and all other options keep Xray's defaults.

# Release Notes — v1.17.1

Add local DoH DNS entries for Vietnam carriers

# Release Notes — v1.17

Xray Module v1.17 introduces flexible control over DNS query strategies by upgrading from the legacy IPv6 preference toggle to a full query strategy configuration. Users can now explicitly choose between UseIP, UseIPv4, UseIPv6, and UseSystem options to fit their specific network environments, while existing configurations smoothly migrate without breaking behavior.

This release improves host management and user experience with a dedicated reload button for custom hosts. The web interface now allows quick reloading of host definitions modified outside the app without losing pending changes. Furthermore, an indicator has been added to provide instant visual feedback during public IP checks.

Routing rules management is now more intuitive with the addition of dedicated reordering controls. Users can adjust the priority of custom routing rules directly in the interface with automatic background persistence to keep configurations synchronized.

Network flexibility has been expanded with a new setting to route LAN and private network traffic through Xray while keeping local loopback traffic isolated. Under the hood, background connectivity tests during interface initialization have been cleaned up for cleaner startup behavior.

---

[Click here for older release notes](https://github.com/vincentng295/Magic_V2Ray/releases?utm_source=gemini)