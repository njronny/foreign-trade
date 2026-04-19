---
name: foreign-trade-outreach
description: >
  外贸B2B开发信全流程系统。从目标客户搜索、关键人定位、定制开发信生成、跟进序列设计到CRM表格管理的完整工作流。
  Use when: (1) 用户要做外贸、找海外客户、发开发信/cold email, (2) 需要搜索北美/欧洲买家公司,
  (3) 需要生成个性化B2B开发信, (4) 需要搭建客户跟进管理系统,
  (5) 用户提到"外贸开发信"、"cold email"、"找客户"、"目标客户"、"B2B获客"、"海外营销"、"客户触达"。
  Triggers: "外贸开发信", "cold email", "找海外客户", "B2B获客", "开发信模板", "客户触达", "外贸营销",
  "outreach", "prospecting", "lead generation", "foreign trade email", "export marketing".
---

# 外贸B2B开发信全流程系统

## 收集信息

向用户确认以下4项（可一次问完）：

1. **品类/产品** — 具体做什么（如CNC加工、电子元器件、纺织品）
2. **目标市场** — 北美、欧洲、中东、东南亚等
3. **独立站** — 有无官网，有则记录URL
4. **邮箱系统** — 企业邮箱域名

## 执行流程（按顺序）

### Phase 1: 系统搭建

创建文件体系到工作区：
```
foreign-trade/cold-email-system/
├── templates/
│   ├── buyer-personas.md           # 买家画像
│   ├── email-templates-en.md       # 通用邮件模板
│   ├── follow-up-sequence.md       # 跟进序列
│   ├── ab-test-subject-lines.md    # A/B测试方案
│   └── prospect-research-template.md  # 客户调研模板
└── prospect-finding-guide.md       # 找客户渠道指南
```

内容模板从 references/ 目录读取：
- `references/buyer-personas.md` → 买家画像参考
- `references/email-templates.md` → 邮件模板参考
- `references/follow-up-sequence.md` → 跟进序列参考
- `references/subject-line-tests.md` → A/B测试参考
- `references/prospect-research.md` → 客户调研模板
- `references/finding-channels.md` → 找客户渠道指南

根据用户品类和目标市场定制内容后写入文件。

### Phase 2: 选择细分行业

根据品类推荐3-5个细分目标行业，按以下维度评估：

| 维度 | 说明 |
|------|------|
| 进入门槛 | 认证要求、技术难度 |
| 市场规模 | 需求量和频次 |
| 利润空间 | 单价和毛利率 |
| 竞争程度 | 同行数量和价格战 |

让用户选择一个细分行业切入。

### Phase 3: 搜索目标客户

使用 `mcporter call 'exa.web_search_exa'` 搜索目标客户公司。

**搜索公式**：
```
"[产品关键词]" "[行业]" "manufacturer" OR "company" "USA" OR "United States"
"[产品关键词]" "purchasing" OR "sourcing" "USA"
"[产品关键词]" "[行业]" "buyer" OR "OEM" OR "distributor"
```

**筛选标准**：
- 优先找中型公司（11-200人），太小的预算有限，太大的流程复杂
- 找有明确产品需求的OEM/制造商，不是纯贸易商
- 每次搜索目标：找到10-20家候选公司

整理为结构化列表，包含：公司名、所在地、产品、规模、官网、推荐度。

### Phase 4: 查找关键决策人

对每家目标公司，搜索关键联系人。

**搜索策略**：
```
"[公司名]" "purchasing manager" OR "sourcing manager" OR "procurement" site:linkedin.com
"[公司名]" "engineering manager" OR "operations" site:linkedin.com
```

**优先找的职位**（按顺序）：
1. Purchasing / Sourcing / Procurement Manager
2. VP Supply Chain / Director of Operations
3. Engineering Manager
4. Owner / CEO（小公司）

**邮箱猜测**：用 Hunter.io 确认企业邮箱格式，常见格式：
- `firstname@company.com`
- `firstinitial.lastname@company.com`
- `firstname.lastname@company.com`

### Phase 5: 生成定制开发信

对每个目标公司生成个性化开发信，遵循以下结构：

```
Subject Line → 3秒决定开不开（含公司名或具体钩子）
开头钩子 → 提到对方公司的具体产品/成就（证明做了功课）
价值主张 → 我们能提供什么，与对方需求匹配
社会证明 → 认证、客户案例、数据
CTA → 明确的下一步行动（免费样品/DFM分析/报价）
```

**个性化要点**：
- 必须提到对方公司的一个具体细节（产品、成就、新闻）
- 必须提到联系人的具体背景（职位、在位时间）
- 避免泛泛而谈，每个词都要有针对性

### Phase 6: 创建飞书CRM表格

使用 `feishu_bitable_app` 创建多维表格，字段如下：

| 字段 | 类型 | 选项 |
|------|------|------|
| 公司名 | 文本 | — |
| 联系人 | 文本 | — |
| 职位 | 文本 | — |
| 邮箱 | 文本 | — |
| 电话 | 文本 | — |
| 行业 | 单选 | 根据实际情况 |
| 国家 | 单选 | USA/Canada/UK/Germany/其他 |
| 状态 | 单选 | 待发送/已发送/已回复/跟进中/已报价/样品阶段/成交/失败 |
| 发送日期 | 日期 | — |
| 跟进次数 | 数字 | — |
| 下次跟进 | 日期 | — |
| 优先级 | 单选 | ⭐~⭐⭐⭐⭐⭐ |
| 官网 | 超链接 | — |
| 备注 | 文本 | — |

将搜索到的所有客户数据批量导入表格。

### Phase 7: 交付总结

向用户展示：
1. 完整交付物清单
2. 飞书表格链接
3. 邮件文件位置
4. 后续使用指引（发信时间、邮箱预热、跟进节奏）

## 关键原则

1. **每封邮件都要个性化** — 绝不群发通用模板
2. **展示你做了功课** — 提到对方具体产品和成就
3. **降低门槛** — 免费样品/DFM分析是最有效的CTA
4. **持续跟进** — 5封序列，14天周期，每次提供新价值
5. **数据驱动** — 用A/B测试优化Subject Line和邮件内容

## 邮件发送建议

- **发送时间**：目标市场上午9-11点（北美=北京时间21:00-23:00）
- **发送频率**：新邮箱每天8-10封，逐步增加
- **跟进节奏**：Day 1 → Day 3 → Day 7 → Day 11 → Day 14
- **A/B测试**：每次只测一个变量，每组至少50封

## 扩展：新增目标行业

当用户需要拓展到新行业时：
1. 只需从 Phase 2 开始重新执行
2. 文件追加到 `foreign-trade/cold-email-system/prospects/` 目录
3. 新客户数据追加到同一飞书表格
