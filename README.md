# adblock

## 自制规则

每天北京时间 3:00 抓 217heidai 的成品，去掉那 5 个源和 PRO mini

- MosDNS 自定义版：`https://raw.githubusercontent.com/passionsu-su/adblock/main/adblockmosdns-custom.txt`

## 去广告规则合集
上游地址
adguard规则来源
https://raw.githubusercontent.com/217heidai/adblockfilters/main/rules/adblockdns.txt
https://anti-ad.net/adguard.txt
https://raw.githubusercontent.com/neodevpro/neodevhost/master/adblocker
https://raw.githubusercontent.com/badmojr/1Hosts/master/Lite/adblock.txt
https://hblock.molinero.dev/hosts_adblock.txt
https://github.com/badmojr/1Hosts/releases/download/latest/1hosts-Xtra_adblock.txt
https://raw.githubusercontent.com/8680/GOODBYEADS/master/data/rules/adblock.txt
https://raw.githubusercontent.com/VeleSila/yhosts/master/hosts.txt
https://cdn.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adblock/ultimate.txt
https://cdn.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adblock/pro.txt
https://big.oisd.nl
https://small.oisd.nl
https://raw.githubusercontent.com/Cats-Team/AdRules/main/adblock_plus.txt

clash去广告规则
  anti-ads:
    type: http
    behavior: domain
    url: https://anti-ad.net/clash.yaml
    path: ./ruleset/anti-ads.yaml
    interval: 86400

  privacy:
    type: http
    behavior: domain
    url: https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Clash/Privacy/Privacy.yaml
    path: ./ruleset/privacy.yaml
    interval: 86400

  app-ads:
    type: http
    behavior: classical
    url: https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Clash/Advertising/Advertising.yaml
    path: ./ruleset/app-ads.yaml
    interval: 86400

  cn-ads:
    type: http
    behavior: domain
    url: https://raw.githubusercontent.com/217heidai/adblockfilters/main/rules/adblockmihomo.yaml
    path: ./ruleset/cn-ads.yaml
    interval: 86400

  rule-merger:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/xndeye/rule-merger/refs/heads/release/reject.yaml"
    path: ./ruleset/rule-merger.yaml
    interval: 86400

  reject:
    type: http
    behavior: domain
    url: "https://cdn.jsdelivr.net/gh/Loyalsoldier/clash-rules@release/reject.txt"
    path: ./ruleset/reject.yaml
    interval: 86400

  surfboard-ad:
    type: http
    behavior: domain
    format: text
    url: "https://getsurfboard.com/adblock.txt"
    path: ./ruleset/surfboard-ad.txt
    interval: 86400
    
  xkww3n:
    type: http
    behavior: domain
    path: ./ruleset/xkww3n.yaml
    url: https://rules.xkww3n.cyou/yaml/reject.yaml
    interval: 86400

  reject_non_ip_no_drop:
    type: http
    behavior: classical
    format: text
    interval: 43200
    url: https://ruleset.skk.moe/Clash/non_ip/reject-no-drop.txt
    path: ./sukkaw_ruleset/reject_non_ip_no_drop.txt
    
  reject_non_ip_drop:
    type: http
    behavior: classical
    format: text
    interval: 43200
    url: https://ruleset.skk.moe/Clash/non_ip/reject-drop.txt
    path: ./sukkaw_ruleset/reject_non_ip_drop.txt
    
  reject_non_ip:
    type: http
    behavior: classical
    format: text
    interval: 43200
    url: https://ruleset.skk.moe/Clash/non_ip/reject.txt
    path: ./sukkaw_ruleset/reject_non_ip.txt
    
  reject_domainset:
    type: http
    behavior: domain
    format: text
    interval: 43200
    url: https://ruleset.skk.moe/Clash/domainset/reject.txt
    path: ./sukkaw_ruleset/reject_domainset.txt
  # 在 Clash 上，同时启用基础和额外的拦截域名会导致内存占用过高和匹配用时增加等性能问题
  reject_extra_domainset:
    type: http
    behavior: domain
    format: text
    interval: 43200
    url: https://ruleset.skk.moe/Clash/domainset/reject_extra.txt
    path: ./sukkaw_ruleset/reject_domainset_extra.txt
    
  reject_ip:
    type: http
    behavior: classical
    format: text
    interval: 43200
    url: https://ruleset.skk.moe/Clash/ip/reject.txt
    path: ./sukkaw_ruleset/reject_ip.txt

  sogouinput:
    type: http
    behavior: classical
    format: text
    interval: 43200
    url: https://ruleset.skk.moe/Clash/non_ip/sogouinput.txt
    path: ./sukkaw_ruleset/sogouinput.txt

  adguard_block:
    type: http
    behavior: classical
    path: ./ruleset/adguard_block.yaml
    url: https://raw.githubusercontent.com/AyraHikari/openclash_adguard/main/rules/adguard_block.yaml
    interval: 43200
    
  adblock:
    type: http
    behavior: classical
    url: https://raw.githubusercontent.com/REIJI007/AdBlock_Rule_For_Clash/main/adblock_reject.yaml
    path: ./ruleset/adblock_reject.yaml
    interval: 86400
    
https://raw.githubusercontent.com/neodevpro/neodevhost/master/clash
https://raw.githubusercontent.com/Cats-Team/AdRules/main/adrules-mihomo.mrs


  ACL4SSR-BanAD:
    type: http
    behavior: classical
    format: yaml
    url: "https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Providers/BanAD.yaml"
    path: ./rules/ACL4SSR-BanAD.yaml
    interval: 86400

  ACL4SSR-BanProgramAD:
    type: http
    behavior: classical
    format: yaml
    url: "https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Providers/BanProgramAD.yaml"
    path: ./rules/ACL4SSR-BanProgramAD.yaml
    interval: 86400

  ACL4SSR-BanEasyListChina:
    type: http
    behavior: classical
    format: yaml
    url: "https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Providers/BanEasyListChina.yaml"
    path: ./rules/ACL4SSR-BanEasyListChina.yaml
    interval: 86400adguard规则来源
https://raw.githubusercontent.com/217heidai/adblockfilters/main/rules/adblockdns.txt
https://anti-ad.net/adguard.txt
https://raw.githubusercontent.com/neodevpro/neodevhost/master/adblocker
https://raw.githubusercontent.com/badmojr/1Hosts/master/Lite/adblock.txt
https://hblock.molinero.dev/hosts_adblock.txt
https://github.com/badmojr/1Hosts/releases/download/latest/1hosts-Xtra_adblock.txt
https://raw.githubusercontent.com/8680/GOODBYEADS/master/data/rules/adblock.txt
https://raw.githubusercontent.com/VeleSila/yhosts/master/hosts.txt
https://cdn.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adblock/ultimate.txt
https://cdn.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adblock/pro.txt
https://big.oisd.nl
https://small.oisd.nl
https://raw.githubusercontent.com/Cats-Team/AdRules/main/adblock_plus.txt

clash去广告规则
  anti-ads:
    type: http
    behavior: domain
    url: https://anti-ad.net/clash.yaml
    path: ./ruleset/anti-ads.yaml
    interval: 86400

  privacy:
    type: http
    behavior: domain
    url: https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Clash/Privacy/Privacy.yaml
    path: ./ruleset/privacy.yaml
    interval: 86400

  app-ads:
    type: http
    behavior: classical
    url: https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Clash/Advertising/Advertising.yaml
    path: ./ruleset/app-ads.yaml
    interval: 86400

  cn-ads:
    type: http
    behavior: domain
    url: https://raw.githubusercontent.com/217heidai/adblockfilters/main/rules/adblockmihomo.yaml
    path: ./ruleset/cn-ads.yaml
    interval: 86400

  rule-merger:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/xndeye/rule-merger/refs/heads/release/reject.yaml"
    path: ./ruleset/rule-merger.yaml
    interval: 86400

  reject:
    type: http
    behavior: domain
    url: "https://cdn.jsdelivr.net/gh/Loyalsoldier/clash-rules@release/reject.txt"
    path: ./ruleset/reject.yaml
    interval: 86400

  surfboard-ad:
    type: http
    behavior: domain
    format: text
    url: "https://getsurfboard.com/adblock.txt"
    path: ./ruleset/surfboard-ad.txt
    interval: 86400
    
  xkww3n:
    type: http
    behavior: domain
    path: ./ruleset/xkww3n.yaml
    url: https://rules.xkww3n.cyou/yaml/reject.yaml
    interval: 86400

  reject_non_ip_no_drop:
    type: http
    behavior: classical
    format: text
    interval: 43200
    url: https://ruleset.skk.moe/Clash/non_ip/reject-no-drop.txt
    path: ./sukkaw_ruleset/reject_non_ip_no_drop.txt
    
  reject_non_ip_drop:
    type: http
    behavior: classical
    format: text
    interval: 43200
    url: https://ruleset.skk.moe/Clash/non_ip/reject-drop.txt
    path: ./sukkaw_ruleset/reject_non_ip_drop.txt
    
  reject_non_ip:
    type: http
    behavior: classical
    format: text
    interval: 43200
    url: https://ruleset.skk.moe/Clash/non_ip/reject.txt
    path: ./sukkaw_ruleset/reject_non_ip.txt
    
  reject_domainset:
    type: http
    behavior: domain
    format: text
    interval: 43200
    url: https://ruleset.skk.moe/Clash/domainset/reject.txt
    path: ./sukkaw_ruleset/reject_domainset.txt
  # 在 Clash 上，同时启用基础和额外的拦截域名会导致内存占用过高和匹配用时增加等性能问题
  reject_extra_domainset:
    type: http
    behavior: domain
    format: text
    interval: 43200
    url: https://ruleset.skk.moe/Clash/domainset/reject_extra.txt
    path: ./sukkaw_ruleset/reject_domainset_extra.txt
    
  reject_ip:
    type: http
    behavior: classical
    format: text
    interval: 43200
    url: https://ruleset.skk.moe/Clash/ip/reject.txt
    path: ./sukkaw_ruleset/reject_ip.txt

  sogouinput:
    type: http
    behavior: classical
    format: text
    interval: 43200
    url: https://ruleset.skk.moe/Clash/non_ip/sogouinput.txt
    path: ./sukkaw_ruleset/sogouinput.txt

  adguard_block:
    type: http
    behavior: classical
    path: ./ruleset/adguard_block.yaml
    url: https://raw.githubusercontent.com/AyraHikari/openclash_adguard/main/rules/adguard_block.yaml
    interval: 43200
    
  adblock:
    type: http
    behavior: classical
    url: https://raw.githubusercontent.com/REIJI007/AdBlock_Rule_For_Clash/main/adblock_reject.yaml
    path: ./ruleset/adblock_reject.yaml
    interval: 86400
    
https://raw.githubusercontent.com/neodevpro/neodevhost/master/clash
https://raw.githubusercontent.com/Cats-Team/AdRules/main/adrules-mihomo.mrs


  ACL4SSR-BanAD:
    type: http
    behavior: classical
    format: yaml
    url: "https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Providers/BanAD.yaml"
    path: ./rules/ACL4SSR-BanAD.yaml
    interval: 86400

  ACL4SSR-BanProgramAD:
    type: http
    behavior: classical
    format: yaml
    url: "https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Providers/BanProgramAD.yaml"
    path: ./rules/ACL4SSR-BanProgramAD.yaml
    interval: 86400

  ACL4SSR-BanEasyListChina:
    type: http
    behavior: classical
    format: yaml
    url: "https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Providers/BanEasyListChina.yaml"
    path: ./rules/ACL4SSR-BanEasyListChina.yaml
    interval: 86400

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
