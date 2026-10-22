# adblock

## 自制规则

每天北京时间 3:00 抓 217heidai 的成品，去掉那 5 个源和 PRO mini

- MosDNS 自定义版：`https://raw.githubusercontent.com/passionsu-su/adblock/main/adblockmosdns-custom.txt`

## 去广告规则合集

按客户端分好类，链接都是各作者的成品订阅地址，自动随上游更新。每个文件顶部是推荐组合，其余按需打开。

| 客户端 | 文件 | 用法 |
|---|---|---|
| AdGuard / AdGuard Home | [adguard/filters.txt](adguard/filters.txt) | 逐条添加为 DNS 黑名单 |
| Clash Meta / mihomo | [clash/adblock.yaml](clash/adblock.yaml) | 合并 rule-providers 与 rules 段 |
| Shadowrocket | [shadowrocket/adblock.conf](shadowrocket/adblock.conf) | 复制到配置的 [Rule] 段最前 |

Raw 地址：

- `https://raw.githubusercontent.com/passionsu-su/adblock/main/adguard/filters.txt`
- `https://raw.githubusercontent.com/passionsu-su/adblock/main/clash/adblock.yaml`
- `https://raw.githubusercontent.com/passionsu-su/adblock/main/shadowrocket/adblock.conf`

### 推荐组合

- **AdGuard Home**：217heidai adblockdns + anti-AD + AdGuard DNS filter + HaGeZi Pro
- **Clash**：217heidai mihomo.mrs + Sukka reject（non_ip / domainset / ip）+ blackmatrix7 Advertising
- **Shadowrocket**：Sukka reject（non_ip / domainset / ip）+ 217heidai surge 域名集 + blackmatrix7 Advertising

### 注意

- 同类大列表别全开：HaGeZi Pro/Ultimate、OISD Big/Small 各选一；Clash 里 Sukka 基础与 extra 同开很吃内存。
- `.mrs` 只有 mihomo 支持。
- anti-ad.net 有 Cloudflare 验证，部分环境拉不到时用文件里给的 GitHub 源。
- 大陆网络拉 raw.githubusercontent.com 慢，可换成 `https://cdn.jsdelivr.net/gh/<用户>/<仓库>@<分支>/<路径>`；jsDelivr 单文件上限 20 MB（Cats-Team adblock_plus、REIJI007 yaml 超限）。
- 已核实过的失效地址不收录：REIJI007 的 Shadowrocket/AdGuard 仓库、xkww3n 的 Surge 格式、8680 的 clash 格式。

### 来源

217heidai/adblockfilters · anti-AD · HaGeZi · OISD · Cats-Team/AdRules · 8680/GOODBYEADS · neodevpro/neodevhost · badmojr/1Hosts · hBlock · VeleSila/yhosts · AWAvenue-Ads-Rule · AdGuard DNS filter · blackmatrix7/ios_rule_script · SukkaW (skk.moe) · Loyalsoldier · xndeye/rule-merger · xkww3n · Surfboard · AyraHikari/openclash_adguard · REIJI007 · ACL4SSR · Johnshall
