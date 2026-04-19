# 复购预测模型

## 预测方法

### 方法1: 消耗周期推算
```
上次订单量 ÷ 客户月消耗量 = 预计消耗完毕时间
提前20-30天提醒 = 复购提醒时间
```

**行业消耗率参考**：
| 行业 | 典型消耗率 | 备注 |
|------|-----------|------|
| 液压设备 | 稳定月消耗 | 按设备维护周期 |
| 阀门制造 | 按生产计划 | 需了解客户生产节奏 |
| 航空航天 | 项目制 | 跟踪项目进度 |
| 医疗设备 | 季度备货 | FDA合规备库 |
| 汽车零部件 | JIT模式 | 频繁小批量 |

### 方法2: 行为信号识别

**强信号（1-2周内可能下单）**：
- 客户问"最快交期能做到多少天？"
- 客户要"最新的报价单"
- 客户问"MOQ能不能降低/提高"
- 客户要求"修改之前报价的数量"

**中信号（1个月内可能下单）**：
- 客户在LinkedIn互动增加
- 客户打开了我们多封邮件
- 客户访问了我们网站多次
- 客户询问新产品/新能力

**弱信号（2-3个月内）**：
- 行业展会前3个月
- 客户公司发布新产品
- 客户公司融资/扩张

### 方法3: 季节性预测

| 行业 | 旺季 | 备货时间 | 提醒时间 |
|------|------|---------|---------|
| 农业机械 | Q1-Q2 | 提前2月 | 11月 |
| 建筑设备 | Q2-Q3 | 提前2月 | 1月 |
| 圣诞消费电子 | Q4 | 提前3月 | 6-7月 |
| 船舶 | Q2-Q3 | 提前3月 | 12月 |
| 通用工业 | Q1/Q3 | 提前1月 | 常态化 |

## 复购提醒话术

### 轻度提醒
```
Hi [Name],

Hope everything is going well! Just wanted to check in — 
it's been about [X] months since your last order of [产品].

Are you still running the same production schedule? 
Happy to prepare a fresh quote if you're planning your 
next batch.

Best,
[Name]
```

### 中度提醒（基于消耗推算）
```
Hi [Name],

Based on your typical order pattern, you might be running 
low on [产品] around now.

Quick update:
- Current pricing: [价格] (unchanged)
- Lead time: [X] days
- Material: in stock for immediate start

Want me to pencil in a production slot?

Best,
[Name]
```

### 强度提醒（有行为信号）
```
Hi [Name],

I noticed you've been checking out our [产品页面/案例]. 
Are you planning a new project?

We've recently upgraded our [能力], which means:
- [改进1]
- [改进2]

Happy to provide a quote or DFM review for your new design.

Best,
[Name]
```
