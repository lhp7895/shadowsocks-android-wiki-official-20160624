Q1: What's the recommended QR code scanner? 

A1: https://play.google.com/store/apps/details?id=tw.com.quickmark

***

Q2: Why is NAT mode deprecated?

A2: 1) Requiring ROOT permission. 2) No IPv6 support. 3) No UDP relay support.

***

Q3: Why are MIUI, EMUI and other AOSPs in China not officially supported?

A3: 1) Broken VPNService implementation, especially for IPv6. 2) Aggressive (or called broken) background service killing policy.

***

Q4: Why does Shadowsocks consume so much battery?

A4: As Shadowsocks takes over the whole device network, any battery used by other apps' network activities are also calculated as Shadowsocks'. So, the battery usage of shadowsocks equals the sum of all the network activities of your device. Shadowsocks itself is a totally I/O bound application on modern Android devices, which is expected not to consume any notable battery.