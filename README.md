# DNS-Block
 My own repository, containing blocked DNS domains.

# 🎯 DNS Blocklists for Privacy, Anti-AI, and Anti-Tracking

This is my personal DNS blocklist, used in combination with **NextDNS** to protect myself and my family against unwanted tracking, unnecessary AI background activity, advertisements, scam websites, and telemetry. It’s tailored to block what *I* consider shady, sketchy, or just plain invasive.

> **If I want to use AI services, I'm doing that whenever I want. Not when they want. I want to use AI on my own and not in the background, tracking me and collecting my data.**

---

## 📦 Blocklist Contents

### Meta (Facebook, Instagram, WhatsApp)

```txt
facebook.com
connect.facebook.net
fbcdn.net
fbcdn.com
fbsbx.com
instagram.com
cdninstagram.com
instagram.net
atdmt.com
atlassolutions.com
whatsapp.com
wa.me
dit.whatsapp.net
meta.ai
wit.ai
graph.facebook.com
```

> Blocks Meta's trackers, AI assistant communication, ad networks, and telemetry across Facebook, Instagram, and WhatsApp.

---

### Google (Ads & Analytics)

```txt
doubleclick.net
ad.doubleclick.net
googleads.g.doubleclick.net
googlesyndication.com
pagead2.googlesyndication.com
googleadservices.com
www.googleadservices.com
google-analytics.com
analytics.google.com
s.youtube.com
ads.google.com
adservice.google.com
```

> Blocks Google Ads, AdSense, DoubleClick, Analytics, and tracking via YouTube. Core functionality of Google apps remains intact.

---

### Amazon (Ads & Telemetry)

```txt
amazon-adsystem.com
aax.amazon-adsystem.com
fls-na.amazon.com
device-metrics-us.amazon.com
affiliationjs.s3.amazonaws.com
advice-ads.s3.amazonaws.com
analyticsengine.s3.amazonaws.com
adtago.s3.amazonaws.com
```

> Blocks Amazon ads and tracking/telemetry scripts, including third-party trackers hosted on S3 buckets.

---

### TikTok

```txt
analytics.tiktok.com
ads.tiktok.com
mon.tiktokv.com
api.tiktokv.com
```

> Blocks TikTok telemetry, tracking and ad delivery. Prevents external surveillance without fully breaking TikTok.

---

### Snapchat

```txt
adsapi.snapchat.com
app-analytics.snapchat.com
snapads.com
euw.adserver.snapads.com
usc.adserver.snapads.com
ads-interfaces.sc-cdn.net
```

> Removes ads, telemetry and AI-related features in Snapchat while keeping core chat/Snap functionality intact.

---

### Scam, Fraud & Shady Domains

```txt
*.proyalz.com
*.proyalz.nl
expertoutlets.nl
vinomz.com
itstylish.co
fishproduct.nl
toofacedshop.nl
dealbeauty.nl
fbwinkel.nl
acadapterwinkel.nl
dutch-lands.com
dutchsport.net
dylawear.com
eco-motoroutlet.com
temu.com
aliexpress.com
```

> These domains are known or strongly suspected scam/fraud sites, often involved in phishing, dropshipping scams, or data collection schemes.

---

### Miscellaneous Trackers, Telemetry & Widgets

```txt
*.widgets.pinterest.com
*.browser.sentry-cdn.com
*.smetrics.samsung.com
```

> Blocks Pinterest's embedded social trackers, Samsung telemetry on mobile/TV, and error tracking via Sentry.

---

### Windows Telemetry (Non-critical)

```txt
vortex.data.microsoft.com
settings-win.data.microsoft.com
watson.telemetry.microsoft.com
telecommand.telemetry.microsoft.com
oca.telemetry.microsoft.com
sqm.telemetry.microsoft.com
```

> These are common Microsoft telemetry endpoints. Blocking them reduces background data collection while maintaining system stability and updates.

---

## ✅ Safe Zones (DO NOT Block – Required for Android & Samsung functions)

```txt
connectivitycheck.android.com
time.android.com
android.clients.google.com
play.googleapis.com
fcm.googleapis.com
push.samsungosp.com
samsungcloud.com
galaxystore.samsung.com
```

> Required for OS updates, network checks, Play Store, Samsung sync, and push notifications.

---

## Setup Info

This list is used on **NextDNS** as part of a private configuration. It complements the following well-known and heavily maintained blocklists which I also use and recommend:

- **HaGeZi - Multi ULTIMATE**
- **Ultimate Sweeper**
- **NextDNS Ads & Trackers Blocklist**
- **AdGuard DNS Filter**
- **OISD Full**
- **AdGuard Mobile Ads Filter**
- **EasyList / EasyPrivacy**
- **AdGuard Tracking Protection Filter**
- **Steven Black's Unified Hosts**
- **Goodbye Ads (Mobile Focused)**
- **notracking**
- **Lightswitch05 - Ads & Tracking**
- **1Hosts (Pro)**

---

## 📊 Results

By using these methods (including DNS blocking, DoH/DoT, and firewall rules), my network blocks between **26–39%** of all traffic on average. That’s thousands of tracking/telemetry requests stopped before they even leave the device.

---

## License & Notes

Feel free to use, fork, and share this blocklist. This is a personal effort to take back control over my devices and stop being profiled for profit. Privacy is a right, not a paid upgrade.

> Protect your privacy, protect your family. 💪
