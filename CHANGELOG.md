# Release Notes — v1.18

Release v1.18 introduces flexible DNS controls, enhanced multi-server configurations, and improved settings management for a smoother proxy and routing experience.

A major feature in this release is configurable DNS Hijacking. Users can now choose whether port 53 DNS traffic from local inbounds is handed over directly to Xray's internal DNS module or forwarded outward. Along with this change, DNS port 53 traffic is no longer unconditionally dropped over IPv6 firewall rules, preventing unnecessary packet loss and keeping IPv6 resolution smooth.

The Foreign DNS module has been upgraded to support multiple fallback servers simultaneously. Users can now input a comma-separated list of resolvers, allowing Xray to distribute and failover foreign domain queries across several DNS endpoints. Additionally, local DoH DNS entries for major Vietnamese ISPs (Viettel, Mobifone, and VNPT) have been included in the default fallback list.

To improve usability in the Web UI, advanced Xray DNS engine parameters can now be configured directly, such as caching controls, stale query behavior, and system hosts integration. A new "Reset to defaults" button has also been added to the Traffic Settings tab, allowing users to restore default traffic parameters easily without affecting custom network interfaces, routing rules, or hosts overrides.

---

[Click here for older release notes](https://github.com/vincentng295/Magic_V2Ray/releases)