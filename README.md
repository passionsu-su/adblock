# adblock

去广告规则订阅合集，按客户端分类。所有链接都指向各作者的成品订阅地址，随上游自动更新，本仓库不做二次加工。
##一键复制 https://hark.site/s/5660ee14-e0ae-4592-a366-ee03e763ebfb?hark_region=us
## 📦 订阅文件

| 客户端 | 文件 | 用法 |
|:---|:---|:---|
| AdGuard / AdGuard Home | [adguard/filters.txt](adguard/filters.txt) | 逐条添加为 DNS 黑名单 |
| Clash Meta / mihomo / Stash | [clash/adblock.yaml](clash/adblock.yaml) | 合并 `rule-providers` 与 `rules` 段（Stash 请用 yaml / text 源，不用 .mrs） |
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
| Surge / QX / Loon / Stash | 规则集：blackmatrix7 或 217heidai 对应格式；App 开屏广告：墨鱼（QX）、可莉（Loon）、app2smile（Surge / Stash） |

## ⚠️ 注意

1. 同类大列表别全开：HaGeZi Pro / Ultimate、OISD Big / Small 各选一个；Clash 里 Sukka 基础与 extra 同开很吃内存。
2. `.mrs` 是二进制格式，只有 mihomo 支持。
3. anti-ad.net 有 Cloudflare 验证，拉不到时用文件里给的 GitHub 源。
4. 大陆拉 raw.githubusercontent.com 慢，可换成 `https://cdn.jsdelivr.net/gh/<用户>/<仓库>@<分支>/<路径>`；jsDelivr 单文件上限 20 MB。
5. 「重写 / 模块 / 插件」类需要开启 MitM 并信任证书才生效，规则集类不需要。

## 📚 规则集来源

按 Star 降序（排序以 2026-10-22 为准，徽章实时显示）。✅ 表示作者提供该客户端可用的格式。

| 项目 | ⭐ Star | 主页 | AdGuard | Clash | Stash | Surge | QX | Loon | 小火箭 |
|:---|:---:|:---|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| Johnshall / Shadowrocket-ADBlock-Rules-Forever | ![](https://img.shields.io/github/stars/Johnshall/Shadowrocket-ADBlock-Rules-Forever?style=flat-square&label=) | [GitHub](https://github.com/Johnshall/Shadowrocket-ADBlock-Rules-Forever) |  |  |  |  |  |  | ✅ |
| StevenBlack / hosts | ![](https://img.shields.io/github/stars/StevenBlack/hosts?style=flat-square&label=) | [GitHub](https://github.com/StevenBlack/hosts) | ✅ |  |  |  |  |  |  |
| Loyalsoldier / clash-rules · surge-rules | ![](https://img.shields.io/github/stars/Loyalsoldier/clash-rules?style=flat-square&label=) | [GitHub](https://github.com/Loyalsoldier/clash-rules) · [surge-rules](https://github.com/Loyalsoldier/surge-rules) |  | ✅ | ✅ | ✅ |  |  | ✅ |
| blackmatrix7 / ios_rule_script | ![](https://img.shields.io/github/stars/blackmatrix7/ios_rule_script?style=flat-square&label=) | [GitHub](https://github.com/blackmatrix7/ios_rule_script) | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| HaGeZi / dns-blocklists | ![](https://img.shields.io/github/stars/hagezi/dns-blocklists?style=flat-square&label=) | [GitHub](https://github.com/hagezi/dns-blocklists) | ✅ |  |  |  |  |  |  |
| anti-AD | ![](https://img.shields.io/github/stars/privacy-protection-tools/anti-AD?style=flat-square&label=) | [GitHub](https://github.com/privacy-protection-tools/anti-AD) · [官网](https://anti-ad.net) | ✅ | ✅ | ✅ | ✅ |  |  | ✅ |
| 217heidai / adblockfilters | ![](https://img.shields.io/github/stars/217heidai/adblockfilters?style=flat-square&label=) | [GitHub](https://github.com/217heidai/adblockfilters) | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| ACL4SSR | ![](https://img.shields.io/github/stars/ACL4SSR/ACL4SSR?style=flat-square&label=) | [GitHub](https://github.com/ACL4SSR/ACL4SSR) |  | ✅ | ✅ | ✅ |  |  | ✅ |
| 秋风广告规则 AWAvenue | ![](https://img.shields.io/github/stars/TG-Twilight/AWAvenue-Ads-Rule?style=flat-square&label=) | [GitHub](https://github.com/TG-Twilight/AWAvenue-Ads-Rule) | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| GMOogway / shadowrocket-rules | ![](https://img.shields.io/github/stars/GMOogway/shadowrocket-rules?style=flat-square&label=) | [GitHub](https://github.com/GMOogway/shadowrocket-rules) |  |  |  |  |  |  | ✅ |
| MetaCubeX / meta-rules-dat | ![](https://img.shields.io/github/stars/MetaCubeX/meta-rules-dat?style=flat-square&label=) | [GitHub](https://github.com/MetaCubeX/meta-rules-dat) |  | ✅ |  |  |  |  |  |
| SukkaW Ruleset | ![](https://img.shields.io/github/stars/SukkaW/Surge?style=flat-square&label=) | [GitHub](https://github.com/SukkaW/Surge) · [官网](https://ruleset.skk.moe) |  | ✅ | ✅ | ✅ |  |  | ✅ |
| AdGuard 过滤器（基础 / 中文） | ![](https://img.shields.io/github/stars/AdguardTeam/AdguardFilters?style=flat-square&label=) | [GitHub](https://github.com/AdguardTeam/AdguardFilters) | ✅ |  |  |  |  |  |  |
| Cats-Team / AdRules | ![](https://img.shields.io/github/stars/Cats-Team/AdRules?style=flat-square&label=) | [GitHub](https://github.com/Cats-Team/AdRules) | ✅ | ✅ | ✅ | ✅ |  | ✅ | ✅ |
| EasyList / EasyList China | ![](https://img.shields.io/github/stars/easylist/easylist?style=flat-square&label=) | [GitHub](https://github.com/easylist/easylist) · [EasyList China](https://github.com/easylist/easylistchina) | ✅ |  |  |  |  |  |  |
| 乘风广告过滤规则 | ![](https://img.shields.io/github/stars/xinggsf/Adblock-Plus-Rule?style=flat-square&label=) | [GitHub](https://github.com/xinggsf/Adblock-Plus-Rule) | ✅ |  |  |  |  |  |  |
| DandelionSprout / adfilt | ![](https://img.shields.io/github/stars/DandelionSprout/adfilt?style=flat-square&label=) | [GitHub](https://github.com/DandelionSprout/adfilt) | ✅ |  |  |  |  |  |  |
| CJX's Annoyance List | ![](https://img.shields.io/github/stars/cjx82630/cjxlist?style=flat-square&label=) | [GitHub](https://github.com/cjx82630/cjxlist) | ✅ |  |  |  |  |  |  |
| badmojr / 1Hosts | ![](https://img.shields.io/github/stars/badmojr/1Hosts?style=flat-square&label=) | [GitHub](https://github.com/badmojr/1Hosts) | ✅ |  |  |  |  |  |  |
| hBlock | ![](https://img.shields.io/github/stars/hectorm/hblock?style=flat-square&label=) | [GitHub](https://github.com/hectorm/hblock) | ✅ |  |  |  |  |  |  |
| 8680 / GOODBYEADS | ![](https://img.shields.io/github/stars/8680/GOODBYEADS?style=flat-square&label=) | [GitHub](https://github.com/8680/GOODBYEADS) | ✅ |  |  |  | ✅ |  |  |
| NoCoin | ![](https://img.shields.io/github/stars/hoshsadiq/adblock-nocoin-list?style=flat-square&label=) | [GitHub](https://github.com/hoshsadiq/adblock-nocoin-list) | ✅ |  |  |  |  |  |  |
| DustinWin / ruleset_geodata | ![](https://img.shields.io/github/stars/DustinWin/ruleset_geodata?style=flat-square&label=) | [GitHub](https://github.com/DustinWin/ruleset_geodata) |  | ✅ |  |  |  |  |  |
| AdGuard DNS filter | ![](https://img.shields.io/github/stars/AdguardTeam/AdGuardSDNSFilter?style=flat-square&label=) | [GitHub](https://github.com/AdguardTeam/AdGuardSDNSFilter) | ✅ |  |  |  |  |  |  |
| neodevpro / neodevhost | ![](https://img.shields.io/github/stars/neodevpro/neodevhost?style=flat-square&label=) | [GitHub](https://github.com/neodevpro/neodevhost) | ✅ | ✅ | ✅ |  |  |  |  |
| VeleSila / yhosts（已归档） | ![](https://img.shields.io/github/stars/VeleSila/yhosts?style=flat-square&label=) | [GitHub](https://github.com/VeleSila/yhosts) | ✅ |  |  |  |  |  |  |
| REIJI007 | ![](https://img.shields.io/github/stars/REIJI007/AdBlock_Rule_For_Clash?style=flat-square&label=) | [GitHub](https://github.com/REIJI007/AdBlock_Rule_For_Clash) · [合集](https://github.com/REIJI007/Adblock-Rule-Collection) | ✅ | ✅ |  |  |  |  |  |
| OISD | ![](https://img.shields.io/github/stars/sjhgvr/oisd?style=flat-square&label=) | [GitHub](https://github.com/sjhgvr/oisd) · [官网](https://oisd.nl) | ✅ |  |  |  |  |  |  |
| xkww3n / Rules | ![](https://img.shields.io/github/stars/xkww3n/Rules?style=flat-square&label=) | [GitHub](https://github.com/xkww3n/Rules) · [官网](https://rules.xkww3n.cyou) |  | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| xndeye / rule-merger | ![](https://img.shields.io/github/stars/xndeye/rule-merger?style=flat-square&label=) | [GitHub](https://github.com/xndeye/rule-merger) |  | ✅ |  |  |  |  |  |
| AyraHikari / openclash_adguard | ![](https://img.shields.io/github/stars/AyraHikari/openclash_adguard?style=flat-square&label=) | [GitHub](https://github.com/AyraHikari/openclash_adguard) |  | ✅ |  |  |  |  |  |

另收录：[Surfboard 去广告规则](https://getsurfboard.com)（Clash domain 格式）。


## 📱 iOS 去广告重写 / 模块 / 插件

去 App 开屏广告、App 内广告需要这一类，配合上面的规则集使用。

| 项目 | ⭐ Star | 主页 | Stash | Surge | QX | Loon | 小火箭 | 内容 |
|:---|:---:|:---|:---:|:---:|:---:|:---:|:---:|:---|
| 墨鱼去广告 ddgksf2013 | ![](https://img.shields.io/github/stars/ddgksf2013/ddgksf2013?style=flat-square&label=) | [GitHub](https://github.com/ddgksf2013/ddgksf2013) · [重写](https://github.com/ddgksf2013/Rewrite) |  |  | ✅ |  |  | 开屏去广告、App 净化 |
| fmz200 / wool_scripts | ![](https://img.shields.io/github/stars/fmz200/wool_scripts?style=flat-square&label=) | [GitHub](https://github.com/fmz200/wool_scripts) | ✅ | ✅ | ✅ | ✅ | ✅ | 去广告规则与重写合集，含 Egern |
| 可莉 luestr / ProxyResource | ![](https://img.shields.io/github/stars/luestr/ProxyResource?style=flat-square&label=) | [GitHub](https://github.com/luestr/ProxyResource) |  |  |  | ✅ |  | Loon 插件库 |
| 毒奶 limbopro / Adblock4limbo | ![](https://img.shields.io/github/stars/limbopro/Adblock4limbo?style=flat-square&label=) | [GitHub](https://github.com/limbopro/Adblock4limbo) |  | ✅ | ✅ | ✅ | ✅ | 网页去广告 |
| app2smile / rules | ![](https://img.shields.io/github/stars/app2smile/rules?style=flat-square&label=) | [GitHub](https://github.com/app2smile/rules) | ✅ | ✅ | ✅ | ✅ |  | B站、贴吧、YouTube 等 App 去广告 |
| 毒奶 limbopro / Profiles4limbo | ![](https://img.shields.io/github/stars/limbopro/Profiles4limbo?style=flat-square&label=) | [GitHub](https://github.com/limbopro/Profiles4limbo) |  |  | ✅ |  |  | QX 懒人配置，含去广告分流 |
| Moli-X / Resources | ![](https://img.shields.io/github/stars/Moli-X/Resources?style=flat-square&label=) | [GitHub](https://github.com/Moli-X/Resources) |  | ✅ | ✅ | ✅ |  | 重写、插件、规则 |
| deezertidal / QuantumultX-Rewrite | ![](https://img.shields.io/github/stars/deezertidal/QuantumultX-Rewrite?style=flat-square&label=) | [GitHub](https://github.com/deezertidal/QuantumultX-Rewrite) |  |  | ✅ |  |  | QX 重写合集 |
| Maasea / sgmodule | ![](https://img.shields.io/github/stars/Maasea/sgmodule?style=flat-square&label=) | [GitHub](https://github.com/Maasea/sgmodule) |  | ✅ |  |  |  | YouTube 去广告等模块 |

感谢以上项目作者的维护，规则版权归原作者所有。
