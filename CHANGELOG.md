# Release Notes — v1.14

### Built-in Direct Routing Pseudo-Node

Magic V2Ray can now run **xray-core as a pure router**, when not using any proxy node.

This allows your Android device to act as a **VPN gateway**, routing hotspot traffic through the module's `tun0` interface.

#### Example: Use Your Phone as a VPN Gateway

1. Enable **1.1.1.1** and connect on your Android device.
2. Open the **Magic V2Ray WebUI**, select the **FREEDOM** node, and press **Start Engine**.
3. Enable **Wi-Fi Hotspot** and connect another device to it.

Once started, **xray-core acts as the gateway**, forwarding traffic from connected hotspot devices through `tun0`.

---

[Click here for older release notes](https://github.com/vincentng295/Magic_V2Ray/releases)
