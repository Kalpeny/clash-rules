# clash-rules
自定义 Clash / OpenClash 分流规则库

## 规则集列表 (.list)
- **Direct-Custom.list**: 自建服务器及内网直连服务 (199222.xyz 等)
- **Futu.list**: 富途 / Moomoo 交易与行情强制代理 (含相关域名与腾讯云 IP-CIDR)
- **MediaScrape.list**: 基础及特殊影视刮削代理 (TMDB, TVDB, IMDb, DMM, AVBase 等)
- **Community.list**: 常用社区代理 (Hostloc, NodeSeek)
- **WifiCall-UK.list**: 英国三大运营商 WiFi Calling 分流代理 (EE, Vodafone, O2, 3UK)
- **PT-Direct.list**: BT/PT 下载防泄漏全量直连规则 (常用端口、Tracker 关键词、100+ PT 站点后缀、详细 Tracker 域名、CIDR)

## 配置文件
- **openclash_custom_rules.yaml**: 可直接贴入 OpenClash 自定义规则的完整合并规则文件
- **ACL4SSR_Custom_Full_Futu.ini**: 订阅转换使用的 ACL4SSR 扩展规则配置
