# DNS Block Lists

Simple DNS blocklists for blocking ads, tracking, and unwanted domains.

## Available Lists

**[tiktok.txt](tiktok.txt)** - TikTok/ByteDance blocking (6,600+ domains)
- All TikTok and ByteDance domains
- Analytics and tracking endpoints
- CDN networks and mirrors

**[meta.txt](meta.txt)** - Facebook/Meta blocking (45 domains)
- Facebook, Instagram, WhatsApp
- Meta AI and tracking pixels
- Social media analytics

**[google.txt](google.txt)** - Google tracking blocking (28 domains)
- Google Analytics and Ads
- DoubleClick advertising
- AdMob and tracking (keeps core Google services)

**[microsoft.txt](microsoft.txt)** - Microsoft telemetry blocking (24 domains)
- Windows telemetry and diagnostics
- Office usage analytics
- Unnecessary data collection (keeps Windows Updates)

**[chinese-shops.txt](chinese-shops.txt)** - Chinese marketplace blocking (42 domains)
- Temu, AliExpress, Wish tracking
- Shein and other platforms
- Aggressive data collection networks

**[scam.txt](scam.txt)** - Scam and fraud sites (14 domains)
- Fake webshops and dropshipping scams
- Known fraud domains
- Phishing websites

**[tracking.txt](tracking.txt)** - General tracking blocking (12 domains)
- Third-party analytics
- Social media widgets
- Samsung and Yahoo tracking

**[datto-kaseya.txt](datto-kaseya.txt)** - Datto RMM / Kaseya blocking (18 IPs, 5 domains)
- Enterprise remote monitoring software
- Network tracking and device discovery
- Referenced: 2021 Kaseya ransomware attack

## How to use

**NextDNS**
1. Go to [nextdns.io](https://nextdns.io) and create account
2. Settings > Security > Blocklists > Add custom domains
3. Copy domains from the .txt files (remove the `0.0.0.0` part)

**Pi-hole**
1. Admin panel > Group Management > Adlists
2. Add the raw GitHub URLs:
   ```
   https://raw.githubusercontent.com/Stensel8/DNS-Block/main/tiktok.txt
   https://raw.githubusercontent.com/Stensel8/DNS-Block/main/meta.txt
   https://raw.githubusercontent.com/Stensel8/DNS-Block/main/google.txt
   ```
3. Update gravity

**AdGuard Home**
1. Filters > DNS blocklists
2. Add the raw GitHub URLs from above

## My Setup

This is how I personally handle these blocks:

- **IP blocks** Add these to your router or firewall to block traffic at the network level
- **DNS blocks**: Add these to your DNS service (I use [NextDNS](https://nextdns.io)) to prevent domain resolution

## Recommended public lists

Use these well-maintained lists alongside the ones here:

- **NextDNS Ads & Trackers Blocklist**: A beginner-friendly blocklist to block ads and trackers globally.

- **HaGeZi - Multi PRO++**: Aggressive list that blocks ads, trackers, phishing, malware, scams, and more.

- **AdGuard DNS Filter**: Combines several AdGuard filters, optimized for DNS-level ad blocking.

- **OISD Blocklist**: All-in-one blocklist for ads, tracking, malware, phishing, scams, and more.

- **AdGuard Tracking Protection Filter**: Focuses on blocking online tracking, analytics, and counters.

- **AdGuard Mobile Ads Filter**: Blocks known mobile ad networks.

- **AdGuard Base Filter**: Blocks ads on general English-language websites.

- **AdGuard Russian Filter**: Removes ads from Russian-language websites.

- **EasyList**: The most popular general-purpose ad-blocking list.

- **EasyList Dutch**: Targets ads on Dutch-language websites.

- **EasyPrivacy**: Focuses specifically on blocking all forms of online tracking.

- **Steven Black Hosts**: Merges several host files for ads, tracking, and malware protection.

- **Goodbye Ads**: Designed for mobile ad blocking, including aggressive mobile ad networks.

- **notracking**: Blocks ads, trackers, and general online garbage.

- **Lightswitch05 - Ads & Tracking**: A highly expanded list focused on ads and tracking domains.

- **1Hosts (Pro)**: Balanced blocklist against ads, tracking, and malware.

These blocklists are updated in real-time and cover ads, telemetry, scam sites, fake shops, spyware, crypto miners, analytics, and more.

## Results

DNS blocking typically stops 20-35% of network requests, preventing thousands of tracking attempts daily.
## Allowed Domains (Exclusions)

See [`allowlist.txt`](allowlist.txt) for the full list of domains that are excluded from blocking and will remain accessible. This allowlist is maintained to ensure important services and apps continue to work.