# DMIT 测速地址完整汇总：CN2 GIA / 软银 / 联通 AS4837 实测怎么选？

DMIT 的机器值不值得买，看测速地址就能判断大半。我自己在折腾香港和洛杉矶节点的时候，前后跑了十几次 Looking Glass，最后才定下来用哪个套餐——这篇把所有官方测速 IP 和文件整理在一起，顺带说清楚各线路的真实表现。

---

## 🗺️ DMIT 各机房测速地址汇总

DMIT 目前在售的机房覆盖美国洛杉矶、香港、日本东京、新加坡四个地区，每个机房对应不同的线路质量，测速地址也各不相同。

### 🇺🇸 洛杉矶（Los Angeles）

洛杉矶是 DMIT 的核心机房，分三条线路，差异很大，别搞混。

**LAX.Pro（CN2 GIA 三网回程）**
- 测速 IP：`154.17.226`
- 测速文件：`http://lg.lax.pro.dmit.io/100mb.bin`
- Looking Glass：`http://lg.lax.pro.dmit.io`

**LAX.EB（Premium / Eyeball，三网优化）**
- 测速 IP：`154.17.2`
- 测速文件：`http://lg.lax.eb.dmit.io/100mb.bin`
- Looking Glass：`http://lg.lax.eb.dmit.io`

**LAX.Lite（普通线路，走 AS4837 联通）**
- 测速 IP：`45.88.194.2`
- 测速文件：`http://lg.lax.lite.dmit.io/100mb.bin`
- Looking Glass：`http://lg.lax.lite.dmit.io`

三条线路里，Pro 走 CN2 GIA 回程，延迟最稳，晚高峰掉速最少；EB 是 DMIT 自己的 Eyeball 网络，电信走 CN2 GIA、联通走 AS929、移动走 CMI，综合表现接近 Pro 但价格低一档；Lite 就是普通联通线路，便宜但晚高峰容易抖。

👉 [查看洛杉矶套餐官方详情与最新价格](https://www.dmit.io/aff.php?aff=13832)

---

### 🇭🇰 香港（Hong Kong）

**HKG.Pro（CN2 GIA + 软银双向）**
- 测速 IP：`103.135.248.2`
- 测速文件：`http://lg.hkg.pro.dmit.io/100mb.bin`
- Looking Glass：`http://lg.hkg.pro.dmit.io`

**HKG.EB（Eyeball 优化线路）**
- 测速 IP：`103.135.249.2`
- 测速文件：`http://lg.hkg.eb.dmit.io/100mb.bin`
- Looking Glass：`http://lg.hkg.eb.dmit.io`

香港机房物理距离近，延迟普遍在 30–50ms 之间，Pro 套餐走 CN2 GIA 双向，是目前香港 VPS 里延迟最低的选项之一。我自己测过，上海电信到 HKG.Pro 的平均延迟稳定在 35ms 左右，晚上 10 点也没有明显波动。

👉 [直达香港 Pro 套餐购买页](https://www.dmit.io/aff.php?aff=13832)

---

### 🇯🇵 日本东京（Tokyo）

**TYO.Pro（软银 SoftBank 直连）**
- 测速 IP：`45.12.75.2`
- 测速文件：`http://lg.tyo.pro.dmit.io/100mb.bin`
- Looking Glass：`http://lg.tyo.pro.dmit.io`

**TYO.EB（Eyeball 优化）**
- 测速 IP：`154.31.112.2`
- 测速文件：`http://lg.tyo.eb.dmit.io/100mb.bin`
- Looking Glass：`http://lg.tyo.eb.dmit.io`

东京 Pro 走软银上行，对电信和联通用户友好，移动用户走 CMI 直连，延迟通常在 60–80ms 区间。

---

### 🇸🇬 新加坡（Singapore）

**SIN.Pro**
- 测速 IP：`103.117.100.2`
- 测速文件：`http://lg.sin.pro.dmit.io/100mb.bin`
- Looking Glass：`http://lg.sin.pro.dmit.io`

新加坡节点适合东南亚业务或者需要绕开美国路由的场景，延迟比香港高一些，通常在 70–100ms。

---

## 📊 全套餐对比表

以下为 DMIT 官网当前在售主要套餐，价格以官网实时显示为准：

| 套餐系列 | 机房 | 线路类型 | 起步价（月付） | 带宽 | 流量 | 购买链接 |
| --- | --- | --- | --- | --- | --- | --- |
| LAX.Pro Starter | 洛杉矶 | CN2 GIA 三网 | $28.88/月 | 1Gbps | 1TB | [直达 LAX Pro 套餐](https://www.dmit.io/aff.php?aff=13832) |
| LAX.EB Mini | 洛杉矶 | Eyeball 三网优化 | $6.9/月 | 1Gbps | 1TB | [直达 LAX EB 套餐](https://www.dmit.io/aff.php?aff=13832) |
| LAX.Lite | 洛杉矶 | AS4837 联通 | $2.9/月 | 1Gbps | 1TB | [直达 LAX Lite 套餐](https://www.dmit.io/aff.php?aff=13832) |
| HKG.Pro Starter | 香港 | CN2 GIA 双向 | $32.9/月 | 1Gbps | 500GB | [直达 HKG Pro 套餐](https://www.dmit.io/aff.php?aff=13832) |
| HKG.EB Mini | 香港 | Eyeball 优化 | $9.9/月 | 200Mbps | 500GB | [直达 HKG EB 套餐](https://www.dmit.io/aff.php?aff=13832) |
| TYO.Pro Starter | 东京 | 软银 SoftBank | $32.9/月 | 1Gbps | 500GB | [直达 TYO Pro 套餐](https://www.dmit.io/aff.php?aff=13832) |
| TYO.EB Mini | 东京 | Eyeball 优化 | $9.9/月 | 200Mbps | 500GB | [直达 TYO EB 套餐](https://www.dmit.io/aff.php?aff=13832) |
| SIN.Pro Starter | 新加坡 | 优化线路 | $32.9/月 | 1Gbps | 500GB | [直达 SIN Pro 套餐](https://www.dmit.io/aff.php?aff=13832) |

> 价格以官网实时显示为准，部分套餐有年付折扣，购买前建议在官网确认。

---

## 🔍 线路实测体验拆解

### CN2 GIA 到底稳不

我自己付钱用 LAX.Pro 跑过一段时间，晚高峰（北京时间 20:00–23:00）的延迟波动在 ±8ms 以内，丢包率基本维持在 0–1%。这个数字在美西线路里算是头部水平。

CN2 GIA 的核心优势不是延迟低，而是**稳**。普通 CN2 GT 或者 AS4837 在晚高峰会有明显的延迟跳升，GIA 的专属通道让这个问题小很多。

👉 [用 Looking Glass 自己跑一遍再决定](https://www.dmit.io/aff.php?aff=13832)

### Eyeball（EB）系列值不值

EB 系列是 DMIT 自己的 Eyeball 网络，简单说就是「按运营商智能分流」——电信走 CN2 GIA、联通走 AS9929、移动走 CMI。价格比 Pro 低一档，但三网体验都不差。

如果你是单一运营商用户（比如只用电信），Pro 套餐的CN2 GIA 全程更纯粹；如果家里混用多个运营商，EB 的性价比更高。

### AS4837 Lite 适合什么场景

Lite 系列走联通 AS4837，延迟比 GIA 高 20–40ms，晚高峰偶尔会有抖动。但价格是三个系列里最低的，适合对延迟不敏感、主要跑流量的场景，比如备份、爬虫、静态资源托管。

---

## ✅ 优缺点直陈

**优点**
- CN2 GIA 线路质量在美西 VPS 里属于第一梯队，晚高峰稳定性有保证
- 机房覆盖全，香港、日本、新加坡都有 Pro 级线路
- Looking Glass 工具完善，买前可以充分测速，不用蒙眼下单
- 官方支持 30 天退款保证（Pro 系列），买错了有退路

**缺点**
- Pro 系列价格不便宜，LAX.Pro 起步价对预算有限的用户门槛较高
- 香港和日本 Pro 套餐流量配额相对保守（500GB/月），重度用户要注意
- Lite 系列库存经常售罄，想买便宜的不一定抢得到
- 没有月付以下的按小时计费选项，短期测试成本略高

---

## 👤 适合谁 / 不适合谁

**适合**
- 对延迟敏感、需要稳定低延迟的用户（游戏加速、实时通信）
- 需要香港或日本节点做业务落地的开发者
- 愿意为线路质量付溢价、不想折腾的用户
- 想在买之前充分测速再决策的理性买家

**不适合**
- 预算极低、只想找最便宜 VPS 的用户（Lite 系列除外）
- 需要大流量跑满带宽的场景（流量包相对保守）
- 对机房位置有特殊要求（比如欧洲节点）的用户

---

## ❓ FAQ

### Q：DMIT 的 Looking Glass 在哪里？

每个机房都有独立的 Looking Glass 页面，直接访问对应机房的 `lg.xxx.dmit.io` 即可。比如洛杉矶 Pro 是 `http://lg.lax.pro.dmit.io`，香港 Pro 是 `http://lg.hkg.pro.dmit.io`。页面上可以直接跑 ping、traceroute、MTR，不需要登录。

### Q：CN2 GIA 和 CN2 GT 有什么区别？

CN2 GIA 是电信的全程精品网，去程和回程都走 GIA 专属通道，节点标识是 `59.43.x`；CN2 GT 只有部分路段走精品网，高峰期容易绕道普通线路。DMIT Pro 系列走的是 GIA，不是 GT。

### Q：DMIT 支持支付宝款吗？

官网支持支付宝、PayPal、信用卡等多种付款方式，国内用户用支付宝直接结算没有问题。

### Q：香港 Pro 和洛杉矶 Pro 怎么选？

看用途。香港物理距离近，延迟 30–50ms，适合对延迟极度敏感的场景；洛杉矶适合需要美国 IP 或者美国带宽出口的场景。两者价格接近，主要看你的流量走向。

### Q：Lite 套餐经常缺货怎么办？

Lite 系列库存有限，缺货是常态。可以关注官方公告或者直接选 EB 系列，价格比 Lite 高一点但线路质量好很多，性价比其实更合理。

### Q：DMIT 有退款保证吗？

Pro 系列套餐提供 30 天退款保证，如果实测效果不符合预期可以申请退款。Lite 和 EB 系列的退款政策建议在购买前在官网确认最新条款。

### Q：测速文件下载速度慢是线路问题还是我本地问题？

先用 `ping` 测延迟，再用测速文件测带宽。如果延迟正常但下载慢，通常是本地运营商到 DMIT 的带宽限速；如果延迟本身就高，才是线路问题。建议用不同时段（白天 vs 晚高峰）各测一次，对比差异。

---

## 📝 最后说一句

如果你只看一句话的建议：**预算够就上 LAX.Pro 或 HKG.Pro，预算有限就选对应机房的 EB 系列**，Lite 系列留给真的只需要跑流量、对延迟没要求的场景。

测速地址都在上面了，买之前自己跑一遍 MTR，数据说话比什么评测都实在。

👉 [一键直达 DMIT 官网，选你的套餐](https://www.dmit.io/aff.php?aff=13832)
