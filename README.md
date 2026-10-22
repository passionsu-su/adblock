# adblock

去广告规则订阅合集，按客户端分类。所有链接都指向各作者的成品订阅地址，随上游自动更新，本仓库不做二次加工。

## 📦 订阅文件

| 客户端 | 文件 | 用法 |
|:---|:---|:---|
| AdGuard / AdGuard Home | [adguard/filters.txt](adguard/filters.txt) | 逐条添加为 DNS 黑名单 |
| Clash Meta / mihomo | [clash/adblock.yaml](clash/adblock.yaml) | 合并 `rule-providers` 与 `rules` 段 |
| Shadowrocket | [shadowrocket/adblock.conf](shadowrocket/adblock.conf) | 复制到配置 `[Rule]` 段最前 |

<details>
<summary>Raw 地址</summary>

```
https://raw.githubusercontent.com/passionsu-su/adblock/main/adguard/filters.txt
https://raw.githubusercontent.com/passionsu-su/adblock/main/clash/adblock.yaml
https://raw.githubusercontent.com/passionsu-su/adblock/main/shadowrocket/adblock.conf
```

</details>

每个文件顶部是默认开启的推荐组合，其余源已注释，按需打开。

## ⭐ 推荐组合

| 客户端 | 组合 |
|:---|:---|
| AdGuard Home | 217heidai adblockdns + anti-AD + AdGuard DNS filter + HaGeZi Pro |
| Clash | 217heidai mihomo.mrs + Sukka reject（non_ip / domainset / ip）+ blackmatrix7 Advertising |
| Shadowrocket | Sukka reject（non_ip / domainset / ip）+ 217heidai surge 域名集 + blackmatrix7 Advertising |

## ⚠️ 注意

1. 同类大列表别全开：HaGeZi Pro / Ultimate、OISD Big / Small 各选一个；Clash 里 Sukka 基础与 extra 同开很吃内存。
2. `.mrs` 是二进制格式，只有 mihomo 支持。
3. anti-ad.net 有 Cloudflare 验证，拉不到时用文件里给的 GitHub 源。
4. 大陆拉 raw.githubusercontent.com 慢，可换成 `https://cdn.jsdelivr.net/gh/<用户>/<仓库>@<分支>/<路径>`；jsDelivr 单文件上限 20 MB。

## 📚 引用来源

| 项目 | 主页 | AdGuard | Clash | Shadowrocket |
|:---|:---|:---:|:---:|:---:|
| 217heidai / adblockfilters | [GitHub](https://github.com/217heidai/adblockfilters) | ✅ | ✅ | ✅ |
| anti-AD | [GitHub](https://github.com/privacy-protection-tools/anti-AD) · [官网](https://anti-ad.net) | ✅ | ✅ | ✅ |
| HaGeZi DNS Blocklists | [GitHub](https://github.com/hagezi/dns-blocklists) | ✅ | | |
| OISD | [官网](https://oisd.nl) | ✅ | | |
| AdGuard DNS filter | [GitHub](https://github.com/AdguardTeam/AdGuardSDNSFilter) | ✅ | | |
| Cats-Team / AdRules | [GitHub](https://github.com/Cats-Team/AdRules) | ✅ | ✅ | ✅ |
| 8680 / GOODBYEADS | [GitHub](https://github.com/8680/GOODBYEADS) | ✅ | | |
| neodevpro / neodevhost | [GitHub](https://github.com/neodevpro/neodevhost) | ✅ | ✅ | |
| badmojr / 1Hosts | [GitHub](https://github.com/badmojr/1Hosts) | ✅ | | |
| hBlock | [GitHub](https://github.com/hectorm/hblock) | ✅ | | |
| VeleSila / yhosts | [GitHub](https://github.com/VeleSila/yhosts) | ✅ | | |
| 秋风广告规则 AWAvenue | [GitHub](https://github.com/TG-Twilight/AWAvenue-Ads-Rule) | ✅ | ✅ | ✅ |
| REIJI007 | [Clash](https://github.com/REIJI007/AdBlock_Rule_For_Clash) · [合集](https://github.com/REIJI007/Adblock-Rule-Collection) | ✅ | ✅ | |
| blackmatrix7 / ios_rule_script | [GitHub](https://github.com/blackmatrix7/ios_rule_script) | | ✅ | ✅ |
| SukkaW Ruleset | [GitHub](https://github.com/SukkaW/Surge) · [官网](https://ruleset.skk.moe) | | ✅ | ✅ |
| Loyalsoldier | [clash-rules](https://github.com/Loyalsoldier/clash-rules) · [surge-rules](https://github.com/Loyalsoldier/surge-rules) | | ✅ | ✅ |
| xndeye / rule-merger | [GitHub](https://github.com/xndeye/rule-merger) | | ✅ | |
| xkww3n / rules | [GitHub](https://github.com/xkww3n/rules) · [官网](https://rules.xkww3n.cyou) | | ✅ | |
| Surfboard | [官网](https://getsurfboard.com) | | ✅ | |
| AyraHikari / openclash_adguard | [GitHub](https://github.com/AyraHikari/openclash_adguard) | | ✅ | |
| ACL4SSR | [GitHub](https://github.com/ACL4SSR/ACL4SSR) | | ✅ | ✅ |
| Johnshall / Shadowrocket-ADBlock-Rules-Forever | [GitHub](https://github.com/Johnshall/Shadowrocket-ADBlock-Rules-Forever) | | | ✅ |

感谢以上项目作者的维护。规则版权归原作者所有。
