# 工作成长与技术沉淀

统计周期：2025-12-01 至 2026-06-08
统计口径：扫描 `/Users/b/newgrand` 直接子目录 Git 仓库；只统计 `release` / `main` 分支上作者为 `diandian` 的提交；同一仓库同一 commit hash 去重。
口径补充：`inewgrand-spider` 为用户确认的更名项目与作者归属例外，当前项目所有提交均计入个人产出，包含 `shirley` 作者提交和 `dev/origin/dev` 上的补充事实。
生成时间：2026-06-08

## 索引

- 时间线：[2025-12](work-growth/timeline/2025-12.md)、[2026-01](work-growth/timeline/2026-01.md)、[2026-02](work-growth/timeline/2026-02.md)、[2026-03](work-growth/timeline/2026-03.md)、[2026-04](work-growth/timeline/2026-04.md)、[2026-05](work-growth/timeline/2026-05.md)、[2026-06](work-growth/timeline/2026-06.md)
- 项目线：[inewgrand-front](work-growth/projects/inewgrand-front.md)、[inewgrand-sys-react](work-growth/projects/inewgrand-sys-react.md)、[inewgrand-weixin](work-growth/projects/inewgrand-weixin.md)、[inewgrand-uia-web](work-growth/projects/inewgrand-uia-web.md)、[sentry-docker](work-growth/projects/sentry-docker.md)、[mcp-test](work-growth/projects/mcp-test.md)、[inewgrand-spider](work-growth/projects/inewgrand-spider.md)、[inewgrand-uia-portaldesign](work-growth/projects/inewgrand-uia-portaldesign.md)、[GlitchTip](work-growth/projects/glitchtip.md)
- 博客草稿：[产业信息平台支付与订单链路建设复盘](work-growth/posts/2026-03-payment-order-flow.md)、[内网环境自托管 Sentry 落地复盘](work-growth/posts/2026-04-sentry-self-hosted.md)、[微信端活动与住宿场景体验优化复盘](work-growth/posts/2026-04-weixin-activity-flow.md)、[inewgrand-spider 住建部资质采集后端与验证码自动化复盘](work-growth/posts/2026-06-inewgrand-spider-crawler.md)

## 跟踪项目状态

### 活跃项目

| 项目 | 分支 | 近 30 天个人提交 | 本周新增 | 一句话定位 |
| --- | --- | ---: | ---: | --- |
| inewgrand-spider | main / dev / origin/dev / origin/main | 14 | 14 | 住建部企业资质运维后端，围绕公开平台数据采集、验证码处理、接口解密和后续预警能力搭建基础；用户确认 `shirley` 提交也归属个人产出。 |
| inewgrand-front | release / origin/release | 38 | 0 | 产业信息平台前台，重点承载应用市场、租户、订单、支付、N-Claw 充值、推广页和 Sentry 接入。 |
| inewgrand-sys-react | release / origin/release | 11 | 0 | 管理后台，支撑商品、订单、活动、住宿、签到设备、接口库、N-Claw 管理和支付配置。 |
| inewgrand-weixin | release / origin/release / origin/main | 1 | 0 | 微信端活动、报名、住宿、支付、扫码签到和移动端错误监控。 |
| inewgrand-uia-web | origin/release / origin/main | 2 | 2 | 云服务平台应用配置、订购跳转、产品类型、门户入口和登录页合规信息集成。 |
| sentry-docker | main / origin/main | 3 | 0 | 自托管 Sentry 的内网部署、资源调优、ClickHouse 清理和离线能力建设。 |
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

围绕 N-Claw、支付、首页体验和可观测性做收敛。前台完成 N-Claw 积分充值组件、协议弹窗、支付渠道品牌名、支付宝支付二维码、推广页、首页产品轮播大图和响应式导航优化；后台优化支付二维码、支付宝 PC 端跳转、租户认证逻辑，并补充接口库请求参数拆分与请求体树结构编辑；Sentry 自托管配置补齐内网服务名、外网超时规避和 ClickHouse 日志清理。整体体现了从功能交付到链路稳定、部署适配和体验打磨的收尾能力。

### 2026-06

本周新增重点从业务前台收尾转向工程化采集服务探索：`inewgrand-spider` 完成住建部企业资质运维后端骨架、验证码统一调度、Playwright 会话自动化、接口 token 刷新、AES-CBC 解密结果落盘、Qwen VLM 接入验证和端到端 smoke 脚本；`inewgrand-uia-web` 补齐登录页版权、备案号和产品名称展示。整体目标是为后续资质采集、规则比对和预警能力打底，同时把登录页合规展示信息补齐。

## 目标导向亮点

1. **为资质运维业务建立可扩展采集底座**：`inewgrand-spider` 初始化 NestJS + Fastify + TypeScript 后端，拆出 crawler、qualification、personnel、compliance、warning、notification 等模块边界，目标是支撑后续企业资质、注册人员、规则比对和预警能力。证据：`ebbb04a`、README、`AGENTS.md`。
2. **降低住建部详情接口采集的人工介入成本**：`inewgrand-spider` 用 Playwright 维护浏览器会话，遇到 408 token 失效后触发验证码桥接、刷新 accessToken、重试接口并保存解密结果，目标是把“人工打开页面验证再复制 token”的流程沉淀为可执行后端能力。证据：`562d714`、`700998a`、`docs/mohurd-crawl-flow.md`。
3. **提升复杂验证码处理的可演进性**：`inewgrand-spider` 建立验证码统一调度架构，覆盖滑块、旋转、单点、顺序点选、文字点选等类型，并把识别、求解和执行动作拆层，目标是让验证码能力可插拔、可测试、可替换。证据：`50af75f`、`7bc72c0`、`dd877a5`、`84277a2`、`docs/captcha-architecture.md`、`docs/mohurd-geetest-vlm.md`。
4. **补齐登录页合规与品牌信息展示**：`inewgrand-uia-web` 在登录页添加版权信息和备案号，并修正版权产品名称为“新云汇”，目标是减少登录入口缺少主体信息或品牌不一致的问题。证据：`5192cfe`、`6775313`。
5. **沉淀 AI Agent 协作规则**：`inewgrand-spider` 和 `inewgrand-front` 均有项目级 `AGENTS.md` 约束上下文阅读、最小改动、pnpm 使用、测试和变更摘要，目标是减少 AI 辅助开发时的上下文偏差和无关改动。证据：`inewgrand-spider` 的 `ebbb04a`、`inewgrand-front` 的 `ec2624a`。

## AI 提效观察

- 可验证证据：项目级 `AGENTS.md` 已进入 `inewgrand-spider` 的 main 分支和 `inewgrand-front` 的 release 分支，用于约束 AI Agent 阅读上下文、最小改动、pnpm 使用、测试要求、变更摘要和推送边界。后续可观察它是否减少返工或无关文件改动。
- `inewgrand-spider` 的 `docs/captcha-architecture.md`、`docs/mohurd-crawl-flow.md`、`docs/mohurd-geetest-vlm.md` 体现了“边实现边沉淀架构、流程和排障经验”的做法；AI 在文档整理、方案拆分、测试清单和复盘表达上的提效有直接材料可追踪，但具体节省时长仍需人工补充。
- 本知识库维护过程本身可由 AI Agent 按固定口径扫描 release/main、去重 commit hash、提炼目标导向总结，能降低周/月复盘整理成本。证据是本仓库的时间线、项目线和博客草稿持续更新。
- 对验证码求解、Playwright 会话刷新和接口解密等代码实现阶段的 AI 提效，目前只能从 `AGENTS.md`、文档和提交结构间接证明 AI 参与了规范沉淀与复盘整理；不能直接证明具体代码由 AI 生成，仍标记为“待补充证据”。

## 建议补充数据

- N-Claw 充值访问量、订单创建量、支付成功率、协议弹窗确认率。
- N-Claw 推广页访问量、下载按钮点击率、不同视口下的访问设备分布。
- 首页产品轮播点击率、移动端导航使用情况、接口库请求体编辑使用次数。
- 住建部采集成功率、验证码一次通过率、平均重试次数、接口 408 触发频率、单次采集耗时、解密结果准确率。
- 支付二维码加载失败率、支付宝跳转失败率、生产资源路径问题数量。
- Sentry 接入前后的错误发现数量、线上问题定位时长、重复问题处理次数、ClickHouse 数据增长和清理效果。
- AGENTS 规则落地后 AI 协作返工次数、无关改动次数、测试补充率和复盘整理耗时变化。
