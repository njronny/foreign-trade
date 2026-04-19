---
name: foreign-trade-content-marketing
description: >
  外贸B2B内容营销全流程系统。从SEO关键词策略、内容日历规划、博客文章批量生成、LinkedIn运营、
  产品描述多语言撰写、客户案例包装到视频脚本生成的完整工作流。支持独立站SEO优化和社交媒体矩阵建设。
  Use when: (1) 用户要做外贸内容营销、SEO优化、博客撰写, (2) 需要生成英文产品描述或技术文章,
  (3) 需要规划LinkedIn/YouTube内容策略, (4) 需要搭建内容发布日历,
  (5) 用户提到"内容营销"、"SEO"、"独立站"、"博客"、"LinkedIn"、"产品描述"、"案例"、"视频脚本"。
  Triggers: "外贸内容营销", "SEO优化", "独立站博客", "LinkedIn运营", "英文内容", "产品描述",
  "客户案例", "视频脚本", "content marketing", "SEO for export", "B2B blog", "product description",
  "foreign trade content", "export marketing content".
---

# 外贸B2B内容营销全流程系统

## 前置信息

需要确认（可从上文或直接询问）：
1. **产品/品类** — 具体做什么
2. **目标市场** — 北美/欧洲/中东等
3. **独立站URL** — 有则分析，无则建议搭建
4. **已有内容** — 目前有哪些营销内容

## 执行流程（按顺序）

### Phase 1: SEO审计 + 关键词策略

**目标**: 建立关键词矩阵，明确内容方向

**步骤**：
1. 使用 `exa.web_search_exa` 搜索行业核心关键词
2. 分析竞品独立站的关键词布局
3. 建立关键词矩阵，按搜索量/难度/意图分类

**关键词分类框架**：
| 类型 | 示例 | 搜索量 | 优化难度 | 内容形式 |
|------|------|--------|---------|---------|
| 核心词 | "CNC machining" | 高 | 高 | 产品页/首页 |
| 长尾词 | "CNC machining aluminum parts tolerances" | 中低 | 低 | 博客文章 |
| 问题词 | "how to choose CNC machining supplier" | 中 | 中 | 指南/FAQ |
| 比较词 | "CNC vs injection molding" | 中 | 中 | 对比文章 |
| 行业+产品 | "hydraulic valve body machining" | 中低 | 低 | 案例文章 |

**参考**: `references/seo-keyword-guide.md`

**产出**: 关键词矩阵文件 → 保存到 `foreign-trade/content-marketing/seo/`

### Phase 2: 内容策略制定

**目标**: 确定内容支柱和发布节奏

**内容支柱模型**（4根支柱）：
1. **产品能力** — 我们能做什么（技术文章、工艺介绍）
2. **行业知识** — 行业洞察（趋势分析、标准解读）
3. **客户成功** — 案例和信任（客户故事、项目回顾）
4. **公司故事** — 品牌人格（工厂展示、团队文化）

**发布节奏建议**：
| 渠道 | 频率 | 内容类型 |
|------|------|---------|
| 博客 | 2-4篇/月 | SEO文章、技术指南 |
| LinkedIn | 3-5帖/周 | 行业洞察、工厂照片、客户反馈 |
| YouTube | 2-4个/月 | 工厂视频、产品演示、技术讲解 |
| 产品页 | 按需 | 产品描述、规格参数 |

**产出**: 内容策略文档 → 保存到 `foreign-trade/content-marketing/strategy/`

### Phase 3: 建立内容日历

**目标**: 30天/90天可执行的内容发布计划

**参考**: `references/content-calendar.md`

**日历结构**：
```
Week 1: 产品能力聚焦
  - 博客: "5-axis CNC Machining: What You Need to Know"
  - LinkedIn: 工厂照片 + 加工过程视频
  - 产品页: 更新3个核心产品描述

Week 2: 行业知识聚焦
  - 博客: "Hydraulic Valve Body Manufacturing: Tolerances & Standards"
  - LinkedIn: 行业标准解读帖子
  - YouTube: 阀体加工过程视频(2分钟)

Week 3: 客户成功聚焦
  - 博客: 客户案例: "How We Helped a US Company Save 30% on CNC Parts"
  - LinkedIn: 客户评价/反馈截图
  - Email: 案例邮件推送给潜在客户

Week 4: 公司故事聚焦
  - 博客: 工厂巡礼 / 质量管控流程
  - LinkedIn: 团队照片 + 质量检测视频
  - YouTube: 工厂全景视频(3-5分钟)
```

**产出**: 内容日历表格 → 同时在飞书多维表格中创建

### Phase 4: 批量生成博客文章

**目标**: 生成SEO优化的英文博客文章

**参考**: `references/blog-templates.md`

**文章模板类型**：
1. **技术指南型** — "Ultimate Guide to [Topic]"
2. **对比分析型** — "[A] vs [B]: Which is Better for [Application]?"
3. **列表型** — "10 Things to Consider When [Action]"
4. **案例型** — "How We [Achievement] for [Client Type]"
5. **FAQ型** — "[Topic] FAQ: Answers to Common Questions"

**每篇文章包含**：
- SEO标题（含主关键词，≤60字符）
- Meta描述（含关键词，≤160字符）
- H1/H2/H3结构化标题
- 内链建议（链接到产品页/其他博客）
- 外链建议（链接到权威来源）
- CTA（引导询盘/下载/联系）
- 社交媒体摘要（LinkedIn/推特点享文案）

**SEO优化要求**：
- 主关键词密度 1-2%
- 长尾关键词自然分布
- 图片alt标签建议
- 至少800-1500字
- 段落不超过3-4句

**产出**: 批量博客文章 → 保存到 `foreign-trade/content-marketing/blog/`

### Phase 5: LinkedIn内容矩阵

**目标**: 生成一周5天的LinkedIn帖子

**参考**: `references/linkedin-strategy.md`

**帖子类型**：
| 天 | 类型 | 示例 |
|----|------|------|
| 周一 | 行业洞察 | "3 trends in CNC machining for 2026..." |
| 周二 | 工厂/过程 | 加工过程照片+简短技术说明 |
| 周三 | 技术帖 | 公差对比图/材料性能表 |
| 周四 | 客户反馈 | 引用客户评价+项目背景 |
| 周五 | 轻松互动 | "Fact or Fiction: Friday" 行业趣味帖 |

**产出**: LinkedIn内容包 → 保存到 `foreign-trade/content-marketing/linkedin/`

### Phase 6: 产品描述 + 客户案例

**目标**: 高转化产品页 + 信任背书案例

**产品描述模板**（参考 `references/product-description.md`）：
```
## [Product Name] — [Primary Benefit]

### Overview
2-3句话概述产品及核心优势

### Specifications
- Material options
- Tolerance capabilities
- Surface finishes
- Certifications
- MOQ & Lead time

### Applications
行业应用列表（带图标）

### Why Choose Us
3-5个差异化优势

### Request a Quote
CTA按钮/表单链接
```

**客户案例模板**（参考 `references/case-study-template.md`）：
```
## Challenge → Solution → Results
- 客户背景
- 面临的问题
- 我们的解决方案
- 量化成果（成本节省%、交期缩短、良率提升）
- 客户原话
```

**产出**: 产品描述 + 案例文章 → 保存到 `foreign-trade/content-marketing/products/`

### Phase 7: 视频脚本 + 内容管理表格

**目标**: 生成视频脚本 + 建立飞书内容管理表

**参考**: `references/video-script-guide.md`

**视频类型**：
1. **工厂巡礼** (3-5分钟) — 全景展示实力
2. **产品演示** (1-2分钟) — 单品加工全过程
3. **技术讲解** (2-3分钟) — 工艺/材料/公差知识
4. **客户证言** (1-2分钟) — 客户采访片段

**飞书内容管理表格**：
| 字段 | 类型 | 说明 |
|------|------|------|
| 标题 | 文本 | 内容标题 |
| 类型 | 单选 | 博客/LinkedIn/YouTube/产品页/案例 |
| 关键词 | 文本 | SEO关键词 |
| 阶段 | 单选 | 待写/写作中/待审核/待发布/已发布 |
| 计划日期 | 日期 | 计划发布日期 |
| 实际日期 | 日期 | 实际发布日期 |
| 渠道 | 多选 | 网站/LinkedIn/YouTube/Email |
| 漏斗阶段 | 单选 | 认知/兴趣/考虑/决策 |
| 文件链接 | 超链接 | 内容文件位置 |
| 备注 | 文本 | — |

使用 `feishu_bitable_app` 创建表格，将所有已生成的内容导入。

## 关键原则

1. **SEO优先** — 每篇内容都有目标关键词和搜索意图
2. **内容支柱** — 围绕4根支柱（产品/行业/案例/公司）持续产出
3. **本地化** — 不是翻译，是本地化表达
4. **CTA清晰** — 每篇内容都有明确的下一步行动
5. **数据驱动** — 追踪每篇内容的流量/询盘转化
6. **批量生产** — 一次规划一个月的内容，批量生成

## 与开发信Skill联动

内容营销产出可直接用于开发信：
- 博客文章链接 → 作为跟进邮件的附加价值
- 客户案例 → 替代空洞的"我们很厉害"
- YouTube视频 → 嵌入开发信增加信任感
- LinkedIn帖子 → 在开发信前先建立触点
