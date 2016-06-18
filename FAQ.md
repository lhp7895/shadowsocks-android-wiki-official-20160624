### Troubleshooting

Cannot connect to server:

1. Stop battery saver if it's active;
2. If an upgrade breaks anything, do a manual reset first by pressing Reset at the end of the list;
3. Check your config;
4. Wipe app data.

Crash: [Submit an issue](https://github.com/shadowsocks/shadowsocks-android/issues/new) with logcat attached, or submit a crash report to Google Play. Then, try wiping app data.

### UI tips

* Remove the default profile to remove ads;
* Tap the number to enter the port you wish to use; (if the keyboard doesn't pop up automatically for some reason)
* You can swipe to remove profiles and long press to reorder them;
* Use Tasker integration to create a desktop widget.

### What's the recommended QR code scanner? 

https://play.google.com/store/apps/details?id=tw.com.quickmark

### Why is NAT mode deprecated?

1. Requiring ROOT permission;
2. No IPv6 support;
3. No UDP relay support.

### Why are MIUI, EMUI and other AOSPs in China not officially supported?

1. Broken VPNService implementation, especially for IPv6;
2. Aggressive (or called broken) background service killing policy.

### How to pause Shadowsocks service?

* For Android N+: Use quick switch tile in Quick Settings;
* Use Tasker integration;
* For Android 6.0-: Add a profile with per-app proxy enabled for Shadowsocks only, bypass mode off.

### Why does Shadowsocks consume so much battery on Android 5.0+?

As Shadowsocks takes over the whole device network, any battery used by network activities from other apps are also counted as those from Shadowsocks. So, the battery usage of Shadowsocks equals to the sum of all the network activities of your device. Shadowsocks itself is a totally I/O bound application on modern Android devices, which is expected not to consume any notable battery.

So if you notice a significant increase in battery usage after you use Shadowsocks, it's most likely caused by other apps. For example, Google Play services can consume more battery after being able to connecting to Google, etc.

### It works fine under Wi-Fi/3G/4G but stops working in another?

That's a bug of your ROM. Report it to the ROM developer. You can also try doing a manual reset and hope for the best.
