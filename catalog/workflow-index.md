# 工作流索引（140）

| 工作流 | slug | 归属 | 触发 | 调用技能 |
|---|---|---|---|---|
| `选题挖掘` | `wf-indie-coldstart-topic-mining` | `de-indie-coldstart-growth-officer` | 定时（每日 8:00） | `community-hotpost-digest`、`painpoint-sellingpoint-match` |
| `开发日志转营销内容` | `wf-indie-coldstart-log-to-content` | `de-indie-coldstart-growth-officer` | 人工（提交 commit 摘要/日志） | `painpoint-sellingpoint-match`、`narrative-rewrite` |
| `多平台改写适配` | `wf-indie-coldstart-multichannel` | `de-indie-coldstart-growth-officer` | 事件（主稿确认后） | `platform-format-adapter`、`title-generator` |
| `发布排期` | `wf-indie-coldstart-scheduling` | `de-indie-coldstart-growth-officer` | 定时 | `platform-format-adapter`、`scheduled-dispatch` |
| `数据反馈与选题迭代` | `wf-indie-coldstart-review` | `de-indie-coldstart-growth-officer` | 定时（每周） | `brief-generator` |
| `发布素材包生成` | `wf-indie-launch-material-pack` | `de-indie-launch-day-commander` | 人工（T-7 天启动） | `producthunt-copy-writer`、`hero-image-sellingpoint`、`faq-pregenerate` |
| `多平台文案适配` | `wf-indie-launch-copy-adapt` | `de-indie-launch-day-commander` | 事件（素材确认后） | `platform-format-adapter`、`multilingual-writing` |
| `发布日历排期` | `wf-indie-launch-calendar` | `de-indie-launch-day-commander` | 人工（T-3 天） | `scheduled-dispatch` |
| `当日评论监控与回复建议` | `wf-indie-launch-comment-monitor` | `de-indie-launch-day-commander` | 定时（发布日每 15 分钟） | `review-sentiment-tag`、`reply-copy-generator` |
| `战报复盘` | `wf-indie-launch-battle-report` | `de-indie-launch-day-commander` | 事件（T+1） | `review-sentiment-tag`、`brief-generator` |
| `关键词调研` | `wf-indie-seo-keyword-research` | `de-indie-seo-content-assistant` | 人工（每月） | `keyword-clustering` |
| `竞品内容差距分析` | `wf-indie-seo-serp-analysis` | `de-indie-seo-content-assistant` | 事件（调研后） | `serp-analysis` |
| `文章大纲生成` | `wf-indie-seo-outline` | `de-indie-seo-content-assistant` | 人工 | `outline-generator` |
| `多语言文章产出` | `wf-indie-seo-multilingual` | `de-indie-seo-content-assistant` | 事件（大纲确认后） | `programmatic-seo-page-generator`、`multilingual-writing` |
| `内链建议` | `wf-indie-seo-draft-internal-link` | `de-indie-seo-content-assistant` | 定时（每周） | `internal-link-matcher` |
| `收录与排名监控` | `wf-indie-seo-effect-review` | `de-indie-seo-content-assistant` | 定时（每周） | `rank-volatility-alert` |
| `多渠道反馈采集` | `wf-indie-feedback-aggregate` | `de-indie-feedback-analyst` | 定时（每日） | `data-ingest-adapter` |
| `去重聚类` | `wf-indie-feedback-dedup` | `de-indie-feedback-analyst` | 事件（采集后） | `feedback-clustering` |
| `情绪与优先级打标` | `wf-indie-feedback-tagging` | `de-indie-feedback-analyst` | 事件（聚类后） | `review-sentiment-tag`、`demand-intensity-score` |
| `周报生成` | `wf-indie-feedback-weekly` | `de-indie-feedback-analyst` | 定时（每周一） | `brief-generator` |
| `路线图建议` | `wf-indie-feedback-roadmap` | `de-indie-feedback-analyst` | 定时（每月） | `demand-intensity-score`、`roadmap-recommendation` |
| `内容一次录入` | `wf-indie-publisher-intake` | `de-indie-multichannel-publisher` | 人工 | `platform-format-adapter` |
| `平台规则适配` | `wf-indie-publisher-dispatch` | `de-indie-multichannel-publisher` | 事件（录入后） | `platform-format-adapter`、`rule-validation` |
| `定时发布` | `wf-indie-publisher-schedule` | `de-indie-multichannel-publisher` | 定时 | `scheduled-dispatch` |
| `数据回捞` | `wf-indie-publisher-retrieve` | `de-indie-multichannel-publisher` | 定时（T+1/T+7） | `data-ingest-adapter` |
| `跨平台对比报表` | `wf-indie-publisher-report` | `de-indie-multichannel-publisher` | 定时（每周） | `attribution-analysis` |
| `知识库构建` | `wf-indie-cs-kb-build` | `de-indie-light-cs-faq` | 人工（初次 + 月更） | `doc-qa-rag` |
| `自动应答` | `wf-indie-cs-presale-qa` | `de-indie-light-cs-faq` | 事件（用户消息） | `doc-qa-rag`、`multilingual-writing` |
| `人工接管分流` | `wf-indie-cs-human-fallback` | `de-indie-light-cs-faq` | 事件（低置信/敏感词） | `ticket-summary` |
| `高频问题反哺 FAQ` | `wf-indie-cs-faq-gen` | `de-indie-light-cs-faq` | 定时（每周） | `faq-feedback-loop` |
| `收入流水整理` | `wf-indie-finance-monthly-ledger` | `de-indie-finance-tax-assistant` | 定时（每月） | `invoice-classify`、`statement-organize` |
| `报税节点提醒` | `wf-indie-finance-compliance-remind` | `de-indie-finance-tax-assistant` | 定时 | `scheduled-dispatch` |
| `合规文档生成` | `wf-indie-finance-doc-gen` | `de-indie-finance-tax-assistant` | 人工 | `privacy-policy-generator` |
| `政策变动解读` | `wf-indie-finance-policy-digest` | `de-indie-finance-tax-assistant` | 事件（政策发布） | `promo-policy-matcher`、`crossborder-tax-faq` |
| `热点聚合扫描` | `wf-creator-topic-hot-aggregate` | `de-creator-topic-planner` | 定时（每日 07:30） | `trendboard-fetcher`、`competitor-content-monitor` |
| `选题库去重匹配` | `wf-creator-topic-dedup` | `de-creator-topic-planner` | 事件（WF1 完成后自动） | `topic-duplicate-check`、`topic-kb-manage` |
| `选题包生成` | `wf-creator-topic-pack` | `de-creator-topic-planner` | 事件（WF2 后自动，每日 08:00 前交付） | `title-generator`、`viral-structure-analysis` |
| `每周选题复盘` | `wf-creator-topic-weekly-review` | `de-creator-topic-planner` | 定时（每周一 09:00） | `viral-structure-analysis`、`topic-kb-manage` |
| `选题转脚本` | `wf-creator-script-topic-to-script` | `de-creator-script-writer` | 人工（选题确认后） | `script-structure`、`hook-copy` |
| `口播稿口语化改写` | `wf-creator-script-colloquial` | `de-creator-script-writer` | 事件（WF1 后自动） | `colloquial-rewrite`、`persona-tone-lib` |
| `分镜与拍摄清单` | `wf-creator-script-storyboard` | `de-creator-script-writer` | 人工（按需） | `script-structure` |
| `AI 痕迹检测与降 AI 味` | `wf-creator-script-ai-gate` | `de-creator-script-writer` | 事件（交付前强制闸门） | `compliance-word-scan`、`colloquial-rewrite` |
| `每日评论聚合分类` | `wf-creator-comment-aggregate` | `de-creator-comment-operator` | 定时（每日 21:00） | `review-sentiment-tag` |
| `高频问题提取→转选题` | `wf-creator-comment-qa-to-topic` | `de-creator-comment-operator` | 事件（WF1 后自动） | `faq-clustering`、`topic-kb-manage`、`topic-duplicate-check` |
| `回复话术建议` | `wf-creator-comment-copy` | `de-creator-comment-operator` | 人工/事件 | `reply-copy-generator`、`persona-tone-lib` |
| `铁粉识别与互动名单` | `wf-creator-comment-fan-tag` | `de-creator-comment-operator` | 定时（每周） | `fan-segment-tag` |
| `引流钩子内容生成` | `wf-creator-private-hook-design` | `de-creator-private-traffic-converter` | 人工（按活动） | `hook-product-design`、`hook-copy`、`compliance-word-scan` |
| `欢迎语与 7 天培育 SOP` | `wf-creator-private-nurture` | `de-creator-private-traffic-converter` | 事件（新粉加入） | `sop-generator`、`fan-segment-tag`、`reply-copy-generator` |
| `私域内容日历` | `wf-creator-private-copy` | `de-creator-private-traffic-converter` | 定时（每周） | `moments-copy-writer`、`community-group-copy`、`persona-tone-lib` |
| `成交话术与复购提醒` | `wf-creator-private-conversion-track` | `de-creator-private-traffic-converter` | 事件（转化节点/沉睡唤醒） | `community-group-copy`、`attribution-analysis` |
| `一稿多投改写` | `wf-creator-rewrite-style` | `de-creator-multichannel-rewriter` | 人工（成稿后） | `platform-format-adapter`、`xhs-note-layout`、`colloquial-rewrite` |
| `平台合规适配` | `wf-creator-rewrite-compliance` | `de-creator-multichannel-rewriter` | 事件（WF1 后自动） | `compliance-word-scan`、`title-generator` |
| `定时发布排期表` | `wf-creator-rewrite-schedule` | `de-creator-multichannel-rewriter` | 定时（每周） | `scheduled-dispatch` |
| `发布状态核对清单` | `wf-creator-rewrite-publish-check` | `de-creator-multichannel-rewriter` | 定时（每日收尾） | `scheduled-dispatch` |
| `周度数据汇总` | `wf-creator-review-data-merge` | `de-creator-data-reviewer` | 定时（每周日） | `dashboard-interpretation` |
| `爆款/扑街归因` | `wf-creator-review-attribution` | `de-creator-data-reviewer` | 事件（WF1 后自动） | `attribution-analysis`、`viral-structure-analysis` |
| `下周内容策略建议` | `wf-creator-review-strategy` | `de-creator-data-reviewer` | 事件（WF2 后自动） | `strategy-recommendation`、`topic-kb-manage` |
| `月度成长报告` | `wf-creator-review-monthly-report` | `de-creator-data-reviewer` | 定时（每月 1 日） | `copy-layout` |
| `brief 解读与需求清单` | `wf-creator-brand-registry` | `de-creator-brand-deal-manager` | 事件（收到 brief） | `brief-parser` |
| `报价单生成` | `wf-creator-brand-quote` | `de-creator-brand-deal-manager` | 人工 | `quote-calculator` |
| `商单内容合规审查` | `wf-creator-brand-compliance` | `de-creator-brand-deal-manager` | 事件（交稿前） | `ad-compliance-review`、`compliance-word-scan` |
| `结案数据报告` | `wf-creator-brand-closeout-report` | `de-creator-brand-deal-manager` | 事件（结案） | `brief-generator`、`copy-layout` |
| `商品图批量生成与质检` | `wf-ecom-visual-batch-gen-qc` | `de-ecommerce-visual-designer` | 人工 | `white-bg-image` |
| `主图 A/B 版本生成` | `wf-ecom-visual-main-ab` | `de-ecommerce-visual-designer` | 人工 | `white-bg-image`、`copy-layout` |
| `平台合规预审` | `wf-ecom-visual-compliance-precheck` | `de-ecommerce-visual-designer` | 事件（出图完成） | `compliance-word-scan` |
| `多平台规格一键适配` | `wf-ecom-visual-spec-adapt` | `de-ecommerce-visual-designer` | 事件（新品上架） | `platform-spec-adapter` |
| `详情页排版生成` | `wf-ecom-visual-detail-page` | `de-ecommerce-visual-designer` | 人工 | `copy-layout`、`conversion-structure-template` |
| `售前智能导购` | `wf-ecom-cs-presale-guide` | `de-ecommerce-customer-service-assistant` | 事件（买家消息） | `doc-qa-rag`、`negotiation-copy` |
| `订单/物流自动查询` | `wf-ecom-cs-logistics` | `de-ecommerce-customer-service-assistant` | 事件 | `logistics-tracking-reader` |
| `售后工单分流与安抚` | `wf-ecom-cs-after-sale-triage` | `de-ecommerce-customer-service-assistant` | 事件 | `review-sentiment-tag`、`handoff-to-human` |
| `夜间值守+次日汇总` | `wf-ecom-cs-night-watch` | `de-ecommerce-customer-service-assistant` | 定时（22:00-8:00 + 8:30 晨报） | `doc-qa-rag`、`brief-generator` |
| `差评预警联动` | `wf-ecom-cs-review-linkage` | `de-ecommerce-customer-service-assistant` | 事件（新评价） | `review-sentiment-tag` |
| `评价流实时监控与分级` | `wf-ecom-review-monitor` | `de-ecommerce-review-guardian` | 定时（每 30 分钟） | `review-sentiment-tag` |
| `差评根因归因` | `wf-ecom-review-root-cause` | `de-ecommerce-review-guardian` | 事件（新差评） | `negative-review-rootcause` |
| `安抚回复与补偿方案生成` | `wf-ecom-review-soothe` | `de-ecommerce-review-guardian` | 人工确认 | `complaint-soothe` |
| `纠纷证据包整理` | `wf-ecom-review-evidence` | `de-ecommerce-review-guardian` | 人工 | `dispute-evidence-pack` |
| `周报复盘` | `wf-ecom-review-weekly` | `de-ecommerce-review-guardian` | 定时（周一） | `brief-generator` |
| `一份资料多平台 Listing 生成` | `wf-ecom-ops-listing-gen` | `de-ecommerce-multichannel-operator` | 人工 | `category-attr-map`、`title-generator` |
| `规格/类目映射维护` | `wf-ecom-ops-spec-map` | `de-ecommerce-multichannel-operator` | 人工（每月） | `category-attr-map` |
| `库存同步与超卖预警` | `wf-ecom-ops-inventory-sync` | `de-ecommerce-multichannel-operator` | 定时（每 15 分钟） | `inventory-waterline-calc`、`oversell-alert` |
| `竞品价格巡检` | `wf-ecom-ops-price-patrol` | `de-ecommerce-multichannel-operator` | 定时（每日） | `price-monitor` |
| `铺货日报` | `wf-ecom-ops-daily-report` | `de-ecommerce-multichannel-operator` | 定时（每日 21:00） | `brief-generator` |
| `商品卖点提取` | `wf-ecom-video-sellingpoint` | `de-ecommerce-shortvideo-producer` | 人工 | `sellingpoint-extract` |
| `短视频脚本生成` | `wf-ecom-video-script` | `de-ecommerce-shortvideo-producer` | 人工 | `script-structure`、`hook-copy` |
| `口播文案+字幕` | `wf-ecom-video-voiceover-subtitle` | `de-ecommerce-shortvideo-producer` | 人工 | `voiceover-script`、`subtitle-copy` |
| `素材混剪指令包` | `wf-ecom-video-slice` | `de-ecommerce-shortvideo-producer` | 人工 | `mixcut-instruction-generator` |
| `发布排期+数据复盘` | `wf-ecom-video-live-script` | `de-ecommerce-shortvideo-producer` | 定时（每日/每周） | `attribution-analysis`、`brief-generator` |
| `类目热词与趋势采集` | `wf-ecom-scout-category-trend` | `de-ecommerce-product-scout` | 定时（每日） | `data-ingest-adapter` |
| `竞品上架/价格/销量监控` | `wf-ecom-scout-price-monitor` | `de-ecommerce-product-scout` | 定时（每 2 小时） | `competitor-digest`、`price-monitor` |
| `蓝海关键词挖掘` | `wf-ecom-scout-blueocean-keyword` | `de-ecommerce-product-scout` | 定时（每周） | `keyword-opportunity-score` |
| `选品打分卡` | `wf-ecom-scout-selection-scorecard` | `de-ecommerce-product-scout` | 人工 | `profit-calculator`、`product-selection-scorecard` |
| `周度机会简报` | `wf-ecom-scout-intel-brief` | `de-ecommerce-product-scout` | 定时（周一） | `brief-generator` |
| `关键词挖掘与标题组合` | `wf-ecom-listing-title` | `de-ecommerce-listing-copywriter` | 人工 | `keyword-combiner` |
| `五点卖点生成` | `wf-ecom-listing-sellingpoint` | `de-ecommerce-listing-copywriter` | 人工 | `sellingpoint-copy` |
| `极限词/广告法合规扫描` | `wf-ecom-listing-compliance` | `de-ecommerce-listing-copywriter` | 事件（文案定稿） | `compliance-word-scan` |
| `详情页转化文案` | `wf-ecom-listing-detail-copy` | `de-ecommerce-listing-copywriter` | 人工 | `conversion-structure-template` |
| `上架后 CTR 追踪建议` | `wf-ecom-listing-ctr-tracking` | `de-ecommerce-listing-copywriter` | 定时（每周） | `ab-copy-variants` |
| `包裹卡/售后卡文案` | `wf-ecom-repurchase-package-card` | `de-ecommerce-repurchase-operator` | 人工 | `marketing-copy`、`compliance-word-scan` |
| `订单老客分层（RFM）` | `wf-ecom-repurchase-segment` | `de-ecommerce-repurchase-operator` | 定时（每周） | `rfm-segmentation` |
| `复购周期预测与触达文案` | `wf-ecom-repurchase-remind` | `de-ecommerce-repurchase-operator` | 定时（每周） | `repurchase-cycle-calc`、`marketing-copy` |
| `会员日活动方案` | `wf-ecom-repurchase-member-day` | `de-ecommerce-repurchase-operator` | 人工（每月） | `campaign-plan-generator` |
| `复购率月报` | `wf-ecom-repurchase-monthly-report` | `de-ecommerce-repurchase-operator` | 定时（每月） | `repurchase-report` |
| `热点选题抓取` | `wf-local-video-hot-topic` | `de-local-store-video-director` | 定时（每日 7:00） | `local-trend-monitor` |
| `探店脚本生成` | `wf-local-video-script` | `de-local-store-video-director` | 人工（老板投喂素材照片/语音描述） | `script-structure` |
| `口播文案+分镜` | `wf-local-video-oral-storyboard` | `de-local-store-video-director` | 人工（随 W2 联动） | `script-structure` |
| `封面标题生成` | `wf-local-video-cover-title` | `de-local-store-video-director` | 人工 | `platform-format-adapter` |
| `发布日历与复盘` | `wf-local-video-review` | `de-local-store-video-director` | 定时（每周一） | `local-trend-monitor`、`platform-format-adapter` |
| `评价采集与情感分级` | `wf-local-review-collect` | `de-local-review-firefighter` | 定时（每 2 小时巡检） | `platform-review-read` |
| `好评感谢回复生成` | `wf-local-review-positive-reply` | `de-local-review-firefighter` | 事件（新好评） | `reply-copy-generator` |
| `差评灭火回复生成` | `wf-local-review-firefight` | `de-local-review-firefighter` | 事件（新差评）→ **即时推送预警** | `reply-copy-generator`、`complaint-soothe` |
| `差评根因归类` | `wf-local-review-root-cause` | `de-local-review-firefighter` | 定时（每周） | `complaint-soothe` |
| `月度口碑报告` | `wf-local-review-monthly` | `de-local-review-firefighter` | 定时（每月 1 日） | `platform-review-read`、`reply-copy-generator` |
| `入群欢迎与打标` | `wf-local-private-join-tag` | `de-local-private-repeat-buyer-manager` | 事件（客户扫码入群） | `wecom-connect` |
| `每日朋友圈文案` | `wf-local-private-moments` | `de-local-private-repeat-buyer-manager` | 定时（每日 7:30 推送 3 条候选） | `moments-copy-writer` |
| `社群话题/活动 SOP` | `wf-local-private-sop` | `de-local-private-repeat-buyer-manager` | 定时（每周一推送本周 SOP） | `community-sop-library` |
| `沉睡客户唤醒` | `wf-local-private-wakeup` | `de-local-private-repeat-buyer-manager` | 定时（每周扫描） | `coupon-strategy` |
| `到店核销引导` | `wf-local-private-verify` | `de-local-private-repeat-buyer-manager` | 事件（领券后 48h 未到店） | `coupon-strategy`、`wecom-connect` |
| `竞品团购监控` | `wf-local-groupbuy-competitor-monitor` | `de-local-groupbuy-designer` | 定时（每周） | `data-ingest-adapter` |
| `套餐结构设计` | `wf-local-groupbuy-structure` | `de-local-groupbuy-designer` | 人工（发起策划） | `pricing-calculator` |
| `扣点毛利测算` | `wf-local-groupbuy-cost` | `de-local-groupbuy-designer` | 随 W2 联动 | `pricing-calculator`、`platform-rules-kb` |
| `团购标题与图片文案` | `wf-local-groupbuy-listing` | `de-local-groupbuy-designer` | 随 W2 联动 | `groupbuy-copy-writer` |
| `核销数据复盘调价` | `wf-local-groupbuy-redemption-review` | `de-local-groupbuy-designer` | 定时（每月） | `data-ingest-adapter`、`pricing-calculator` |
| `在线预约受理` | `wf-local-booking-collect` | `de-local-booking-scheduler` | 事件（客户微信/小程序发起） | `shift-calendar-engine` |
| `技师/场地智能排班` | `wf-local-booking-schedule` | `de-local-booking-scheduler` | 定时（每日 6:30） | `shift-calendar-engine` |
| `冲突与超售检测` | `wf-local-booking-conflict-check` | `de-local-booking-scheduler` | 事件（新预约写入） | `shift-calendar-engine` |
| `爽约预测+候补补位` | `wf-local-booking-noshow-remind` | `de-local-booking-scheduler` | 定时（每日两次扫描） | `demand-forecast`、`notification-dispatcher` |
| `排班效率周报` | `wf-local-booking-efficiency-weekly` | `de-local-booking-scheduler` | 定时（每周一） | `demand-forecast`、`notification-dispatcher` |
| `会员分层（RFM）` | `wf-local-member-segment` | `de-local-member-awakener` | 定时（每周） | `member-data-sync`、`rfm-segmentation` |
| `召回话术与券包生成` | `wf-local-member-wakeup-copy` | `de-local-member-awakener` | 随 W1 联动 | `winback-copy-generator`、`coupon-strategy` |
| `触达时机推荐` | `wf-local-member-touch-timing` | `de-local-member-awakener` | 定时（每日） | `scheduled-dispatch` |
| `复购效果归因` | `wf-local-member-repurchase-attribution` | `de-local-member-awakener` | 定时（每月） | `member-data-sync`、`rfm-segmentation` |
| `储值流失预警` | `wf-local-member-storedvalue-churn` | `de-local-member-awakener` | 定时（每周） | `rfm-segmentation` |
| `内容一稿多投适配` | `wf-local-hub-content-adapt` | `de-local-multichannel-ops-hub` | 人工（投喂单稿） | `platform-format-adapter` |
| `团购信息多平台同步` | `wf-local-hub-groupbuy-sync` | `de-local-multichannel-ops-hub` | 人工触发+定时校验 | `multichannel-connector` |
| `评价/数据跨平台汇总` | `wf-local-hub-data-merge` | `de-local-multichannel-ops-hub` | 定时（每日） | `multichannel-connector`、`data-dashboard-builder` |
| `周度运营看板` | `wf-local-hub-unified-view` | `de-local-multichannel-ops-hub` | 定时（每周一） | `data-dashboard-builder` |
| `数据采集` | `wf-local-daily-collect` | `de-local-store-daily-report-analyst` | 定时（每日 21:30） | `data-ingest-adapter` |
| `日报生成` | `wf-local-daily-report` | `de-local-store-daily-report-analyst` | 定时（每日 22:00） | `brief-generator` |
| `异常预警` | `wf-local-daily-anomaly` | `de-local-store-daily-report-analyst` | 事件（指标越界） | `anomaly-detect` |
| `周建议` | `wf-local-daily-weekly-advice` | `de-local-store-daily-report-analyst` | 定时（每周一） | `brief-generator`、`anomaly-detect` |
