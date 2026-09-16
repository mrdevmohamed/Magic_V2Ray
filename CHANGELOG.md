# Release Notes — v1.13

**Professional Mode**
Hide the built-in node pickers entirely and write `config.json` by hand for full control over your Xray setup. A new "Load template" button gives you a ready-made skeleton (fwmark 255, tun-in, socks-test-in, etc.) to edit instead of starting from scratch, plus in-app documentation covering the rules your config must follow (fwmark, the mandatory tun inbound, DNS routing order...) so a misconfigured tunnel doesn't silently deadlock.

**VLESS Encryption Support**
Added the outbound-side `encryption` field for VLESS (post-quantum, per XTLS/Xray-core#5067), read from and written to link query params — defaults to "none" as before when not specified.

**FinalMask Support for Nodes**
A network-agnostic masking layer now works uniformly across every protocol — VMess, VLESS, Trojan, Shadowsocks, and Hysteria2. On import/export, FinalMask merges intelligently with any existing obfuscation layer (like Hysteria2's salamander) instead of overwriting it, and a malformed FinalMask never takes the whole node down — it just falls back to running without the extra masking.

**Bug Fixes**
Fixed node confirmation before connecting.

---

[Click here for older release notes](https://github.com/vincentng295/Magic_V2Ray/releases)