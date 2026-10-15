# 🚀 Sing-box 毕业级配置（Android / 通用）

> 一份经过长期验证、路由顺序精准、国内直连/国外代理/广告拦截/端口防火墙齐全的 Sing-box 配置。

---

## ✨ 配置亮点

- **路由顺序教科书级**：国内域名 → 私有IP → FakeIP → 代理规则集 → 国内IP → 端口拒绝，层层递进，永不误杀。
- **DNS 双重保险**：国内走 local-dns，国外走 fakeip，广告/HttpDNS 直接拒之门外。
- **端口拒绝黑名单**：拦截 BT 下载、木马后门、VPN 探测等垃圾流量，节省代理节点流量。
- **17 个规则集全覆盖**：Google、FCM、Android、proxy、gfw、ai、games、ads 等，开箱即用。
- **广告拦截**：DustinWin + AdGuardSDNSFilter 双重拦截，网页清爽无广告。

---

## 📦 使用方法

1. 下载 [Sing-box Android](https://github.com/SagerNet/sing-box/releases) 最新版。
2. 将本仓库中的 `config.json` 替换到 Sing-box 配置目录。
3. 在 `outbounds` 中添加你的节点配置（VLESS / VMess / Trojan / Shadowsocks 等等均可）。
4. 启动服务，畅享网络。

---

## ⚠️ 注意事项

- 所有规则集均从 `cdn.jsdelivr.net` 加载，如遇下载失败，可将 URL 中的 `cdn.jsdelivr.net` 替换为 `ghproxy.net`。
- 节点配置请自行替换，本配置不包含任何节点信息。
- 本配置适用于 Android，其他平台（Windows/macOS/Linux）需微调 `inbounds` 部分。

---

## 📄 规则集来源

| 规则集 | 来源 |
|--------|------|
| cn / cnip / proxy / ads / ai / games / microsoft-cn / apple-cn / games-cn / networktest / private | [DustinWin/ruleset_geodata](https://github.com/DustinWin/ruleset_geodata) |
| gfw | [MetaCubeX/meta-rules-dat](https://github.com/MetaCubeX/meta-rules-dat) |
| Google / fcm / Android / httpDNS / DNSreject | [SagerNet](https://github.com/SagerNet/SagerNet) |
