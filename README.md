# clash-rules
自定义 Clash / OpenClash 分流规则库

## 规则集列表 (.list)
- **Direct-Custom.list**: 微信图片域名优先直连、自建服务器及内网直连服务 (199222.xyz 等)
- **Futu.list**: 富途 / Moomoo 交易与行情强制代理 (含相关域名与腾讯云 IP-CIDR)
- **MediaScrape.list**: 基础及特殊影视刮削代理 (TMDB, TVDB, IMDb, DMM, AVBase 等)
- **Community.list**: 常用社区代理 (Hostloc, NodeSeek)
- **WifiCall-UK.list**: 英国三大运营商 WiFi Calling 分流代理 (EE, Vodafone, O2, 3UK)
- **PT-Direct.list**: BT/PT 下载防泄漏全量直连规则 (常用端口、Tracker 关键词、100+ PT 站点后缀、详细 Tracker 域名、CIDR)

## 配置文件
- **openclash_custom_rules.yaml**: 可直接贴入 OpenClash 自定义规则的完整合并规则文件
- **ACL4SSR_Custom_Full_Futu.ini**: 订阅转换使用的 ACL4SSR 扩展规则配置

微信图片修复：`Direct-Custom.list` 内的两条 `wxsnsdy*.wxs.qq.com` 精确域名规则必须排在 ACL4SSR `BanAD` / `BanProgramAD` 之前；本仓库的订阅转换配置已调整顺序。只更新 GitHub 列表、不重新生成并加载 OpenClash 配置，不会改变当前运行规则。路由器上的本地优先规则保留作为即时兜底。
