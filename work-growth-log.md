# 工作成长与技术沉淀

统计周期：2025-12-01 至 2026-05-21  
统计口径：扫描 `/Users/b/newgrand` 下 Git 仓库；只统计 `release` / `main` 分支上作者为 `diandian` 的提交；同一仓库同一 commit hash 去重。  
生成时间：2026-05-21

## 索引

- 时间线：[2025-12](work-growth/timeline/2025-12.md)、[2026-01](work-growth/timeline/2026-01.md)、[2026-02](work-growth/timeline/2026-02.md)、[2026-03](work-growth/timeline/2026-03.md)、[2026-04](work-growth/timeline/2026-04.md)、[2026-05](work-growth/timeline/2026-05.md)
- 项目线：[inewgrand-front](work-growth/projects/inewgrand-front.md)、[inewgrand-sys-react](work-growth/projects/inewgrand-sys-react.md)、[inewgrand-weixin](work-growth/projects/inewgrand-weixin.md)、[inewgrand-uia-web](work-growth/projects/inewgrand-uia-web.md)、[sentry-docker](work-growth/projects/sentry-docker.md)、[inewgrand-uia-portaldesign](work-growth/projects/inewgrand-uia-portaldesign.md)、[GlitchTip](work-growth/projects/glitchtip.md)、[mcp-test](work-growth/projects/mcp-test.md)
- 博客草稿：[内网环境自托管 Sentry 落地复盘](work-growth/posts/2026-04-sentry-self-hosted.md)、[产业信息平台支付与订单链路建设复盘](work-growth/posts/2026-03-payment-order-flow.md)、[微信端活动与住宿场景体验优化复盘](work-growth/posts/2026-04-weixin-activity-flow.md)

## 跟踪项目状态

### 活跃项目

| 项目 | 分支 | 本期提交数 | 一句话定位 |
| --- | --- | ---: | --- |
| inewgrand-front | release / origin/release | 274 | 产业信息平台前台，覆盖应用市场、租户、订单、支付、N-Claw、Sentry 接入等用户侧链路。 |
| inewgrand-sys-react | release / origin/release | 246 | 管理后台，覆盖商品、产品、订单、活动、住宿、签到设备、N-Claw 管理等运营链路。 |
| inewgrand-weixin | release / origin/release / origin/main | 202 | 微信端活动、报名、住宿、支付、扫码签到和 Sentry 监控建设。 |
| inewgrand-uia-web | origin/release / origin/main | 27 | 云服务平台应用配置、订购跳转、产品类型和门户集成。 |
| sentry-docker | main / origin/main | 21 | 自托管 Sentry 的内网部署、资源调优、ClickHouse 清理和离线能力建设。 |

### 观察项目

| 项目 | 原因 |
| --- | --- |
| inewgrand-uia-portaldesign | 本期有少量 `main` 分支提交，主要是门户设计组件初始化。 |
| GlitchTip | 本期有少量 `main` 分支提交，主要是错误监控替代方案初始化与文档配置。 |
| mcp-test | 本期有初始化提交，暂不展开项目线。 |

### 未纳入正文

| 项目 | 原因 |
| --- | --- |
| hr-react、iNewGrandfront、ng-design-mcp、ng-design、nova | 当前本地未发现 `release` / `main` 分支，按规则不统计。 |
| community、inewgrand、inewgrandaiautofront、lanhu-mcp、mi8-react、ng-nup-portaldesign-web、pm-pcm-react、portal-design-react、psm-react | 存在 `release` / `main` 相关分支，但本周期内未命中 `diandian` 提交。 |

## 当月重点

### 2025-12

前台和后台从基础框架进入核心业务链路建设：前台完成登录注册、租户、应用市场、订单确认、上传凭证、发票等基础能力；后台完成产品、商品、标签、订单、对公支付凭证审核等管理能力；微信端开始接入授权登录。这个阶段的价值是把产业信息平台从页面雏形推进到可围绕商品、租户和订单闭环运行的业务骨架。

### 2026-01

围绕订单、开票、付款凭证、商品管理、活动报名、微信端个人资料和活动列表等做密集补齐。后台侧持续修复订单字段、上传回执、标签过滤、产品分类树等问题；前台侧完善应用购买、免费试用、订单入口、验证码和认证逻辑；微信端形成活动报名与用户注册链路。

### 2026-02

工作重心转向应用配置、门户微应用集成和活动/住宿流程补齐。`inewgrand-uia-web` 开始承接门户设计入口和应用配置重构；前台和后台继续完善活动、住宿、页面路由和数据展示，整体从“能跑”向“可配置、可运营”演进。

### 2026-03

微信端进入高强度交付期，重点是住宿预订、微信 JSAPI 支付、订单详情、支付倒计时和支付状态处理；前台侧推进产品页、首页动态数据、SmartImage、CDN/OSS 配置和 API baseURL 适配；后台侧继续完善住宿房型、房损规则、活动订单导出等运营能力。

### 2026-04

技术建设和业务功能并行：一方面推进自托管 Sentry、前后台/微信端 Sentry 接入、隧道、用户信息和构建信息上报；另一方面交付扫码签到、签到设备、住宿订单导出、N-Claw 积分包管理、AI 产品类型、服务管理等功能。这个月可以作为“稳定性建设 + 业务复杂场景落地”的重点材料。

### 2026-05

围绕 N-Claw、支付和可观测性做收敛：前台完成 N-Claw 积分充值组件、支付宝支付二维码与跳转逻辑；后台优化支付二维码、支付宝 PC 端跳转、租户认证相关逻辑；Sentry 自托管配置补齐内网服务名和外网超时规避。整体体现了从功能交付到链路稳定、部署适配和体验打磨的收尾能力。

## 最值得讲的亮点

1. **产业信息平台前后台业务闭环建设**：从 2025-12 开始，持续建设前台应用市场、租户、订单、支付、上传凭证、后台商品/订单/产品/标签管理等能力，形成从用户购买到后台运营审核的主链路。
2. **微信端活动与住宿场景落地**：围绕活动报名、微信授权、住宿预订、订单明细、微信 JSAPI 支付、扫码签到、退款审核意见等场景持续交付，覆盖用户现场使用的关键路径。
3. **支付与订单链路完善**：横跨前台、后台、微信端完成对公支付凭证、微信支付、支付宝扫码/跳转、支付二维码弹窗、订单状态与支付倒计时等能力。
4. **可观测性与内网部署建设**：自托管 Sentry 配置、ClickHouse TTL、内网服务名、消费者资源、前后台/微信端 Sentry 接入和用户信息上报，形成问题定位基础设施。
5. **工程化和可维护性改进**：在多个项目中通过组件抽象、hook 提取、枚举/类型统一、环境变量拆分、构建配置优化和 AGENTS 规则沉淀，降低后续开发和排查成本。

## 提效与影响

- 业务效率：订单、支付、开票、上传凭证、退款审核等功能线上化后，减少人工流转和线下确认环节。具体节省时间需要结合运营处理量补充数据。
- 排查效率：Sentry 接入和自托管部署使错误可按环境、用户、版本和堆栈追踪，故障定位从“用户反馈 + 人工复现”转向“事件化排查”。实际 MTTR 改善幅度待验证。
- 开发效率：通用上传、树形组件、金额格式化、请求配置、产品类型枚举等抽象减少重复实现，后续相似需求可复用。建议补充复用次数或后续需求交付周期变化。
- 体验收益：微信端住宿/支付/扫码签到、前台 N-Claw 充值和后台支付二维码优化降低关键路径阻塞。具体转化率或失败率变化需要业务埋点或客服反馈支撑。

## 建议补充数据

- 订单、支付、开票、上传凭证功能上线后的使用量、失败率和人工处理量变化。
- Sentry 接入前后的线上问题定位时长、错误发现数量、重复问题处理次数。
- N-Claw 充值链路上线后的访问量、支付成功率和用户反馈。
- 微信端活动/住宿/签到场景的实际使用峰值、扫码签到成功率和现场问题数量。
