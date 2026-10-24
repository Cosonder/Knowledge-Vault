---
aliases:
  - dividend
  - dividende
  - dividend yield
  - rendement du dividende
summary: 公司将利润以现金或股票形式分配给股东
tags: [finance, learning]
---
# Definition

**股息**（dividend, *dividende*）是公司把部分利润分配给股东的款项，通常以现金支付，也可以是股票股息（stock dividend）。是否派息、派多少由董事会提议、股东大会批准。美国公司多按季度派息，法国公司多为每年一次。

# Formula

**股息率**（dividend yield, *rendement du dividende*）：设每股年度股息 $D$，股价 $P$，

$$\text{dividend yield} = \frac{D}{P}.$$

**派息率**（payout ratio, *taux de distribution*）：设每股收益（EPS）为 $E$，

$$\text{payout ratio} = \frac{D}{E}, \qquad \text{留存率 } b = 1 - \frac{D}{E}.$$

派息率超过 100% 意味着公司在用储备或借债派息，通常不可持续。

**除息价格下跌**。股息有一个**除息日**（ex-dividend date, *date de détachement*）：此日及之后买入的股票不再享有本期股息。忽略税收与市场波动，无套利要求

$$P_{\text{ex}} \approx P_{\text{cum}} - D,$$

因为公司资产减少了 $D$。所以派息本身不创造价值：股东从"持有 $P_{\text{cum}}$ 的股票"变为"持有 $P_{\text{cum}} - D$ 的股票 + $D$ 的现金"。这是 Modigliani–Miller 股息无关论（1961）的核心：在无税、无交易成本的完美市场中，股息政策不影响公司价值。

**总收益**（total return, *rendement total*）。持有期 $[0,1]$ 的总收益为

$$R = \frac{P_1 - P_0 + D}{P_0} = \underbrace{\frac{P_1 - P_0}{P_0}}_{\text{资本利得}} + \underbrace{\frac{D}{P_0}}_{\text{股息率}}.$$

比较投资业绩应使用总收益指数（如 CAC 40 GR 而非 CAC 40 价格指数），否则会低估股息贡献，见 [[Return 收益率 rendement|收益率]]。

# Dividends vs buybacks

**股票回购**（share buyback, *rachat d'actions*）是返还现金的另一方式：公司用现金在市场买回并注销股份。在完美市场中，派息 $D$ 与等额回购对股东价值等价：回购后股数减少，每股价格不下跌，留下的股东持股比例上升。现实差别主要在于：

- 税收：许多国家股息当年计税，回购只在卖出时实现资本利得；
- 灵活性：削减股息常被市场视为坏信号，回购则可随时调整；
- 信号作用与管理层激励（如以 EPS 为考核目标）。

# Example

某股票除息前收盘价 50 欧元，每股派息 2 欧元。

- 股息率 $= 2/50 = 4\%$；若 EPS 为 5 欧元，派息率 $= 2/5 = 40\%$；
- 除息日开盘理论价 $\approx 48$ 欧元；
- 若一年后股价为 52 欧元（已除息），总收益 $= (52 - 50 + 2)/50 = 8\%$，其中资本利得 4%、股息 4%。

# Common misconceptions

- "高股息股票是免费的收入。"股息来自股价的等额下降，不是额外收益；股息率高还可能因为股价暴跌（dividend trap）。
- "只花股息不动本金就安全。"从总收益角度，花掉股息与卖出等值股票在经济上相近，见 [[Safe withdrawal rate 安全提取率 taux de retrait|安全提取率]]。
- "不派息的公司对股东没有价值。"留存利润可再投资或用于回购，价值体现在股价上。

# Vocabulaire

| français | 中文 | English |
|---|---|---|
| le dividende (m.) | 股息 | dividend |
| le rendement du dividende (m.) | 股息率 | dividend yield |
| le taux de distribution (m.) | 派息率 | payout ratio |
| la date de détachement (f.) | 除息日 | ex-dividend date |
| le rachat d'actions (m.) | 股票回购 | share buyback |
| le bénéfice par action (m.) | 每股收益 | earnings per share |
| l'actionnaire (m./f.) | 股东 | shareholder |

# Related

- [[Stock 股票 action|股票]]
- [[Return 收益率 rendement|收益率]]
- [[Passive income 被动收入 revenu passif|被动收入]]
- [[ETF 交易所交易基金 fonds négocié en bourse|ETF]]（累积型与分配型）
- [[Safe withdrawal rate 安全提取率 taux de retrait|安全提取率]]

# Self-check 自测

> [!question]- 为什么除息日股价会下跌约等于股息？
> 派息后公司现金减少 $D$，每股对应的资产价值减少 $D$。若价格不下跌，投资者可在除息前买入、领息、除息后以原价卖出，获得无风险利润，这与无套利矛盾。实际跌幅受税收和当天其他信息影响。

> [!question]- 股息率 6% 的股票是否意味着年收益至少 6%？
> 不是。总收益 $= $ 资本利得 $+$ 股息率，资本利得可以为负。股息率高也可能是股价下跌或市场预期股息即将削减的结果。

> [!question]- 完美市场中，100 万欧元现金股息与 100 万欧元回购对一位不参与回购的股东有何差别？
> 没有价值差别。派息时他得到现金、股价下跌；回购时他不得到现金，但股数减少使每股价值不变、持股比例上升。他若需要现金，可卖出相应股份自制股息（homemade dividend）。
