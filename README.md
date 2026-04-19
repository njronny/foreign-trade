# Foreign Trade AI System 🌍

**AI驱动的外贸B2B全流程系统** — 从市场分析到客户复购的完整闭环。

基于 OpenClaw Agent Skill 框架，5个Skill覆盖外贸全链路，每个Skill可独立使用，组合使用形成完整商业闭环。

## 系统架构

```
┌─────────────────────────────────────────────────────────────┐
│                    外贸AI全流程闭环                           │
│                                                             │
│  Skill 0          Skill 1          Skill 2                  │
│  ┌──────────┐     ┌──────────┐     ┌──────────┐            │
│  │ 市场分析  │────→│ 开发信    │────→│ 内容营销  │            │
│  │          │     │ 客户触达  │     │          │            │
│  └──────────┘     └──────────┘     └──────────┘            │
│       ↓                ↓                ↓                   │
│  市场在哪？         谁是客户？        怎么建立信任？           │
│  竞品是谁？         怎么联系？        怎么被找到？            │
│  我们凭啥赢？       怎么跟进？        怎么展示专业？           │
│                                                             │
│  Skill 3          Skill 4                                  │
│  ┌──────────┐     ┌──────────┐                             │
│  │ 询盘报价  │────→│ 客户跟进  │────┐                        │
│  │          │     │ CRM管理   │     │                        │
│  └──────────┘     └──────────┘     │                        │
│       ↓                ↓           │                        │
│  怎么报价？         怎么不丢客户？    │                        │
│  怎么谈判？         怎么促复购？      │                        │
│  怎么成交？         怎么防流失？      │                        │
│                                    │                        │
│         ┌──────────────────────────┘                        │
│         ↓                                                    │
│    🔄 复购 & 转介绍 & 新需求 → 回到 Skill 1/3               │
└─────────────────────────────────────────────────────────────┘
```

## 5个Skill详解

### Skill 0: 市场分析&竞品分析 `foreign-trade-market-analysis`

> **搞清战场，再打仗**

| Phase | 内容 | 产出 |
|-------|------|------|
| 1 | 市场规模&趋势 | TAM/SAM/SOM分析报告 |
| 2 | 目标行业筛选 | 10个行业100分评分排名 |
| 3 | 竞品地图 | 5-10个竞品档案 |
| 4 | 价格带分析 | 全球价格体系+定价空间 |
| 5 | 差异化定位 | USP + Elevator Pitch |
| 6 | 渠道分析 | 8个渠道评估+预算分配 |
| 7 | SWOT+行动计划 | 交叉策略+90天行动方案 |

**参考文件**: 市场规模方法、行业评分模型、竞品分析模板、价格带数据、定位画布、渠道策略、SWOT框架

---

### Skill 1: 开发信&客户触达 `foreign-trade-outreach`

> **主动出击，找到对的人**

| Phase | 内容 | 产出 |
|-------|------|------|
| 1 | 目标客户搜索 | 6大渠道搜索方法 |
| 2 | 买家画像匹配 | 4种买家类型分析 |
| 3 | 关键人定位 | 决策者LinkedIn搜索 |
| 4 | 个性化开发信 | 定制英文邮件 |
| 5 | 跟进序列设计 | 5封14天跟进链 |
| 6 | A/B测试方案 | 标题+正文对照实验 |
| 7 | CRM导入 | 飞书多维表格客户管理 |

**已有数据**:
- 12封定制开发信（6家液压+6家阀门公司）
- 9位关键决策人（含LinkedIn）
- 飞书CRM表格（14条客户记录）

**参考文件**: 开发信模板、跟进序列、买家画像、A/B测试、客户调研模板

---

### Skill 2: 内容营销 `foreign-trade-content-marketing`

> **让客户主动找到你**

| Phase | 内容 | 产出 |
|-------|------|------|
| 1 | SEO关键词矩阵 | 30+关键词优先级排序 |
| 2 | 内容策略制定 | 博客+LinkedIn+视频组合 |
| 3 | 内容日历规划 | 30天/90天发布计划 |
| 4 | 博客文章写作 | SEO优化的英文长文 |
| 5 | LinkedIn内容 | 每周5帖内容包 |
| 6 | 产品描述 | 多语言产品页 |
| 7 | 视频脚本 | YouTube/短视频脚本 |

**已有数据**:
- 3篇SEO博客（公差指南/成本指南/选供应商清单）
- LinkedIn一周内容包（5帖）
- 工厂巡礼视频脚本
- 2个产品描述页（液压阀体+铝合金零件）
- 飞书内容管理表格（10条内容）

**参考文件**: SEO指南、内容日历模板、LinkedIn策略、博客模板、产品描述模板、案例模板、视频脚本指南

---

### Skill 3: 询盘处理&报价 `foreign-trade-inquiry`

> **专业报价，快速成交**

| Phase | 内容 | 产出 |
|-------|------|------|
| 1 | 询盘解析 | A/B/C分级+信息提取 |
| 2 | 技术评估 | 图纸审查+DFM建议 |
| 3 | 成本核算 | 分项成本计算+阶梯报价 |
| 4 | 报价单生成 | 专业英文报价单 |
| 5 | 谈判话术 | 6个场景应对方案 |
| 6 | 样品管理 | SOP流程+转化技巧 |

**已有数据**:
- RED-WHITE VALVE完整报价演示（6个Phase全走通）
- 试单50pcs $89/pc → 月产500pcs $62/pc

**参考文件**: 询盘解析指南、技术评估清单、成本核算方法、报价单模板、谈判话术库、样品管理流程

---

### Skill 4: 客户跟进&CRM `foreign-trade-crm`

> **不丢客户，持续复购**

| Phase | 内容 | 产出 |
|-------|------|------|
| 1 | 客户分级体系 | A/B/C/D/E五级+100分模型 |
| 2 | 跟进节奏管理 | 全生命周期时间线 |
| 3 | 沟通记录模板 | 标准化记录格式 |
| 4 | 复购预测 | 消耗周期+行为信号+季节性 |
| 5 | 流失预警&挽回 | 5种挽回策略+话术 |
| 6 | 飞书CRM搭建 | 客户总表+沟通记录+订单跟踪 |

**参考文件**: 客户分级体系、跟进节奏、沟通记录模板、复购预测模型、流失预警策略

---

## Skill间数据流

```
Skill 0 (市场分析)
  ├→ 行业优先级 → Skill 1 (选择目标行业)
  ├→ USP/定位   → Skill 1 (开发信卖点)
  ├→ 关键词     → Skill 2 (SEO内容规划)
  ├→ 渠道策略   → Skill 2 (内容分发渠道)
  ├→ 价格带     → Skill 3 (定价策略)
  └→ 竞品分析   → Skill 4 (客户分级权重)

Skill 1 (开发信)
  └→ 客户线索 → Skill 4 (CRM导入)

Skill 2 (内容营销)
  └→ 内容互动 → Skill 4 (沟通记录)

Skill 3 (询盘报价)
  ├→ 报价记录 → Skill 4 (订单跟踪)
  └→ 谈判进展 → Skill 4 (状态更新)

Skill 4 (CRM)
  └→ 复购提醒 → Skill 3 (新一轮报价)
  └→ 客户需求 → Skill 2 (内容选题)
```

## 快速开始

### 1. 安装Skill

将 `.skill` 文件解压到 OpenClaw workspace 的 `skills/` 目录：

```bash
# 安装全部5个Skill
unzip foreign-trade-market-analysis.skill -d ~/.openclaw/workspace/skills/
unzip foreign-trade-outreach.skill -d ~/.openclaw/workspace/skills/
unzip foreign-trade-content-marketing.skill -d ~/.openclaw/workspace/skills/
unzip foreign-trade-inquiry.skill -d ~/.openclaw/workspace/skills/
unzip foreign-trade-crm.skill -d ~/.openclaw/workspace/skills/
```

### 2. 执行顺序

```
推荐顺序: 0 → 1 → 2 → 3 → 4

1. 先做市场分析（Skill 0）— 搞清楚方向
2. 开始发开发信（Skill 1）— 获取第一批线索
3. 同步做内容营销（Skill 2）— 长期流量
4. 收到询盘就报价（Skill 3）— 成交转化
5. 全程维护CRM（Skill 4）— 持续经营
```

### 3. 使用方式

在 OpenClaw 中直接对话：

```
你: "帮我分析CNC加工北美市场"
→ 自动使用 Skill 0

你: "帮我找液压行业的北美客户"
→ 自动使用 Skill 1

你: "帮我写一篇CNC公差指南的博客"
→ 自动使用 Skill 2

你: "收到一个询盘，客户要报阀体价"
→ 自动使用 Skill 3

你: "帮我给客户分级，看看该跟进谁"
→ 自动使用 Skill 4
```

## 目录结构

```
foreign-trade/
├── README.md                              # 本文件
│
├── skills/                                # Skill源文件
│   ├── foreign-trade-market-analysis/     # Skill 0: 市场分析
│   ├── foreign-trade-outreach/            # Skill 1: 开发信
│   ├── foreign-trade-content-marketing/   # Skill 2: 内容营销
│   ├── foreign-trade-inquiry/             # Skill 3: 询盘报价
│   └── foreign-trade-crm/                 # Skill 4: 客户CRM
│
├── cold-email-system/                     # 开发信系统数据
│   ├── templates/                         # 模板库
│   └── prospects/                         # 客户数据
│
├── content-marketing/                     # 内容营销产出
│   ├── seo/                               # SEO关键词矩阵
│   ├── blog/                              # 博客文章
│   ├── linkedin/                          # LinkedIn内容
│   ├── products/                          # 产品描述
│   └── video/                             # 视频脚本
│
├── inquiry-demo/                          # 询盘报价演示
│   └── RWV-valve-285-*                    # RED-WHITE VALVE完整案例
│
├── foreign-trade-market-analysis.skill    # 打包Skill文件
├── foreign-trade-outreach.skill           # 打包Skill文件
├── foreign-trade-content-marketing.skill  # 打包Skill文件
├── foreign-trade-inquiry.skill            # 打包Skill文件
└── foreign-trade-crm.skill                # 打包Skill文件
```

## 适用场景

- 🏭 **CNC机械加工** 外贸出口
- 🔧 **液压设备/阀门** 精密零件
- 🌎 **北美市场** 为主要目标
- 📧 **B2B冷启动** 从0到第一个订单
- 🤖 **AI辅助** 减少重复劳动，提高效率

## 技术栈

- **框架**: OpenClaw Agent Skill
- **CRM**: 飞书多维表格（Bitable）
- **语言**: 英文内容 + 中文操作指引
- **搜索**: web_fetch 在线搜索
- **协作**: GitHub版本管理

## License

MIT
