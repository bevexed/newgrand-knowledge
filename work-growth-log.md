# 工作成长与技术沉淀

统计周期：2025-12-01 至 2026-05-25
统计口径：扫描 `/Users/b/newgrand` 直接子目录 Git 仓库；只统计 `release` / `main` 分支上作者为 `diandian` 的提交；同一仓库同一 commit hash 去重。
生成时间：2026-05-25

## 索引

- 时间线：[2025-12](work-growth/timeline/2025-12.md)、[2026-01](work-growth/timeline/2026-01.md)、[2026-02](work-growth/timeline/2026-02.md)、[2026-03](work-growth/timeline/2026-03.md)、[2026-04](work-growth/timeline/2026-04.md)、[2026-05](work-growth/timeline/2026-05.md)
- 项目线：[inewgrand-front](work-growth/projects/inewgrand-front.md)、[inewgrand-sys-react](work-growth/projects/inewgrand-sys-react.md)、[inewgrand-weixin](work-growth/projects/inewgrand-weixin.md)、[inewgrand-uia-web](work-growth/projects/inewgrand-uia-web.md)、[sentry-docker](work-growth/projects/sentry-docker.md)、[mcp-test](work-growth/projects/mcp-test.md)、[inewgrand-uia-portaldesign](work-growth/projects/inewgrand-uia-portaldesign.md)、[GlitchTip](work-growth/projects/glitchtip.md)
- 博客草稿：[产业信息平台支付与订单链路建设复盘](work-growth/posts/2026-03-payment-order-flow.md)、[内网环境自托管 Sentry 落地复盘](work-growth/posts/2026-04-sentry-self-hosted.md)、[微信端活动与住宿场景体验优化复盘](work-growth/posts/2026-04-weixin-activity-flow.md)

## 跟踪项目状态

### 活跃项目

| 项目 | 分支 | 近 30 天个人提交 | 本周新增 | 一句话定位 |
| --- | --- | ---: | ---: | --- |
| inewgrand-front | release / origin/release | 25 | 6 | 产业信息平台前台，重点承载应用市场、租户、订单、支付、N-Claw 充值和 Sentry 接入。 |
| inewgrand-sys-react | release / origin/release | 12 | 0 | 管理后台，支撑商品、订单、活动、住宿、签到设备、N-Claw 管理和支付配置。 |
| inewgrand-weixin | release / origin/release / origin/main | 1 | 0 | 微信端活动、报名、住宿、支付、扫码签到和移动端错误监控。 |
| inewgrand-uia-web | origin/release / origin/main | 0 | 0 | 云服务平台应用配置、订购跳转、产品类型和门户入口集成；近 30 天分支仍有变化，保留跟踪。 |
| sentry-docker | main / origin/main | 2 | 0 | 自托管 Sentry 的内网部署、资源调优、ClickHouse 清理和离线能力建设。 |
| mcp-test | main | 1 | 0 | MCP 测试项目，当前仅有初始化提交，后续视真实工具化沉淀扩展。 |

### 观察项目

| 项目 | 分支 | 原因 |
| --- | --- | --- |
| inewgrand | origin/release / origin/main | 近 30 天 release/main 有文件变化，但未命中 `diandian` 提交；仅总入口观察。 |
| lanhu-mcp | main / origin/main | 近 30 天 main 有文件变化，但未命中 `diandian` 提交；仅总入口观察。 |

### 历史项目

| 项目 | 分支 | 原因 |
| --- | --- | --- |
| GlitchTip | main | 已有项目线，但近 90 天 release/main 未命中 `diandian` 产出，保留故事线，不写入周报正文。 |
| inewgrand-uia-portaldesign | main / origin/main | 已有项目线，近 30 天无 release/main 变化，本期只保留索引。 |

### 未纳入

| 项目 | 原因 |
| --- | --- |
| hr-react、iNewGrandfront、ng-design、ng-design-mcp、nova | 未纳入：缺少 `release` / `main` 分支。 |
| community、inewgrandaiautofront、mi8-react、ng-nup-portaldesign-web、pm-pcm-react、portal-design-react、psm-react | 存在 `release` / `main` 相关分支，但本周期未命中 `diandian` 提交，也未进入知识库项目线。 |

## 当月重点

### 2025-12

前台和后台从基础框架进入核心业务链路建设：前台完成登录注册、租户、应用市场、订单确认、上传凭证、发票等基础能力；后台完成产品、商品、标签、订单、对公支付凭证审核等管理能力；微信端开始接入授权登录。这个阶段的目标是把产业信息平台从页面雏形推进到可围绕商品、租户和订单闭环运行的业务骨架。

### 2026-01

围绕订单、开票、付款凭证、商品管理、活动报名、微信端个人资料和活动列表做密集补齐。后台侧持续修复订单字段、上传回执、标签过滤、产品分类树等问题；前台侧完善应用购买、免费试用、订单入口、验证码和认证逻辑；微信端形成活动报名与用户注册链路。

### 2026-02

工作重心转向应用配置、门户微应用集成和活动/住宿流程补齐。`inewgrand-uia-web` 承接门户设计入口和应用配置重构；前台和后台继续完善活动、住宿、页面路由和数据展示，整体从“能跑”向“可配置、可运营”演进。

### 2026-03

微信端进入高强度交付期，重点是住宿预订、微信 JSAPI 支付、订单详情、支付倒计时和支付状态处理；前台侧推进产品页、首页动态数据、SmartImage、CDN/OSS 配置和 API baseURL 适配；后台侧继续完善住宿房型、房损规则、活动订单导出等运营能力。

### 2026-04

技术建设和业务功能并行：一方面推进自托管 Sentry、前后台/微信端 Sentry 接入、隧道、用户信息和构建信息上报；另一方面交付扫码签到、签到设备、住宿订单导出、N-Claw 积分包管理、AI 产品类型、服务管理等功能。这个月可以作为“稳定性建设 + 业务复杂场景落地”的重点材料。

### 2026-05

围绕 N-Claw、支付和可观测性做收敛。前台完成 N-Claw 积分充值组件、协议弹窗、支付渠道品牌名、支付宝支付二维码与跳转逻辑；后台优化支付二维码、支付宝 PC 端跳转、租户认证相关逻辑；Sentry 自托管配置补齐内网服务名和外网超时规避。整体体现了从功能交付到链路稳定、部署适配和体验打磨的收尾能力。

## 目标导向亮点

1. **提升 N-Claw 积分充值链路完整性**：`inewgrand-front` 本周围绕 iframe 充值入口补充服务协议弹窗、支付渠道标签、品牌名展示和卡片布局，目标是让用户在内嵌充值场景中能清楚理解协议、选择支付并完成二维码支付。证据：`19c3f65`、`ce43f43`、`48eb4c2`、`589b3f9`。
2. **降低支付链路配置和展示风险**：前后台在 5 月持续处理支付宝二维码、微信标识、二维码容错、生产资源路径和 PC 端跳转模式，目标是减少支付入口展示错误和环境差异导致的支付阻塞。证据：`bd1043d`、`f600a1e`、`b9f9c57`、`e2ac235`、`01dc80a`。
3. **降低线上问题定位成本**：`sentry-docker` 和多端 Sentry 接入继续围绕内网服务名、隧道地址、错误处理、日志格式做修正，目标是让错误能按环境、用户、版本和堆栈追踪。证据：`1f2a064`、`3472437`、`94469b7`、`7f8b871`。
4. **沉淀 AI Agent 协作规则**：`inewgrand-front` 添加项目级 `AGENTS.md`，目标是减少 AI 辅助开发时的上下文偏差和无关改动。证据：`ec2624a`。

## AI 提效观察

- 可验证证据：项目级 `AGENTS.md` 已进入 `inewgrand-front` 的 release 分支，用于约束 AI Agent 阅读上下文、最小改动、变更摘要和测试建议。后续可观察它是否减少返工或无关文件改动。
- 本知识库维护过程本身可由 AI Agent 按固定口径扫描 release/main、去重 commit hash、提炼目标导向总结，能降低周/月复盘整理成本。证据是本仓库的时间线、项目线和博客草稿持续更新。
- 对代码实现阶段的 AI 提效，例如需求拆解、组件草稿、Hook 抽象或排障辅助，目前只能从规则文档和提交主题间接推断，仍标记为“待补充证据”，不夸大为确定收益。

## 建议补充数据

- N-Claw 充值访问量、订单创建量、支付成功率、协议弹窗确认率。
- 支付二维码加载失败率、支付宝跳转失败率、生产资源路径问题数量。
- Sentry 接入前后的错误发现数量、线上问题定位时长、重复问题处理次数。
- AGENTS 规则落地后 AI 协作返工次数、无关改动次数和复盘整理耗时变化。
