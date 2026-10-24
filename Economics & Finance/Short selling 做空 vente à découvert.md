---
aliases:
  - short selling
  - short
  - vente à découvert
  - position courte
  - shorting
summary: 借入资产卖出、日后买回归还，从价格下跌中获利
tags: [finance, learning]
---
# Definition

**做空**（short selling, *vente à découvert*）是卖出自己并不持有的资产，期望日后以更低价格买回，从价格下跌中获利。由此形成的头寸称为**空头**（short position, *position courte*），是[[Long 做多 position longue|做多]]的对应面：多头从上涨中获利，空头从下跌中获利。

# Mechanism

**借券**（securities lending, *prêt de titres*）。典型流程：

1. 投资者通过券商从出借方（常为养老金、[[Index fund 指数基金 fonds indiciel|指数基金]]等长期持有者）借入股票；
2. 在市场卖出，获得现金 $S_0$；
3. 借券期间支付借券费（borrow fee），并须把期间的[[Dividend 股息 dividende|股息]]等额补偿给出借方（manufactured dividend）；
4. 平仓（covering）：在 $t$ 时以 $S_t$ 买回股票归还。

忽略费用，空头损益为

$$\Pi_{\text{short}} = S_0 - S_t.$$

由于 $S_t \ge 0$ 且无上界，最大收益为 $S_0$（股价归零），**潜在亏损无上限**。这与多头恰好相反：多头最大亏损为 $S_0$，收益无上限。

**保证金**（margin, *dépôt de garantie*）。卖空所得资金不能自由支配，券商还要求额外抵押。设初始保证金比例 $m_0$（如 50%）、维持保证金比例 $m$（如 30%）。卖空 $N$ 股后账户权益为

$$E_t = (1 + m_0) N S_0 - N S_t,$$

当 $E_t / (N S_t) < m$ 时触发**追加保证金**（margin call, *appel de marge*）。解得触发价

$$S_t^* = \frac{(1 + m_0) S_0}{1 + m}.$$

若无法补足，券商会强制平仓，往往发生在价格最不利的时刻。

**轧空**（short squeeze）。当空头仓位占流通股比例很高时，价格上涨迫使空头买回平仓（主动止损或被强平），买盘进一步推高价格，形成正反馈。2021 年 GameStop 是典型例子；2008 年大众汽车曾因此短暂成为全球市值最高的公司。

**监管**。许多市场限制裸卖空（naked short selling，未先借券就卖出），并在危机时临时禁止卖空（如 2008 年和 2020 年法国 AMF 的禁令）。

# Example

以 $S_0 = 100$ 欧元卖空 1 000 股，$m_0 = 50\%$，$m = 30\%$。

- 若股价跌至 80 欧元：收益 $1000 \times (100 - 80) = 20\,000$ 欧元（未计费用）；
- 追加保证金触发价 $S^* = 1.5 \times 100 / 1.3 \approx 115.4$ 欧元；
- 若股价涨至 200 欧元：亏损 $100\,000$ 欧元，即初始保证金 50 000 欧元的两倍。

# Common misconceptions

- "做空就是看跌期权。"买入看跌[[Option 期权 option|期权]]的最大亏损是权利金，做空的亏损无上限。
- "做空只是投机，对市场有害。"做空也用于[[Hedge 对冲 couverture|对冲]]、套利，并通过让负面信息进入价格来改善价格发现（参见[[Efficient market hypothesis 有效市场假说 hypothèse des marchés efficients|有效市场假说]]）。
- "长期做空和长期做多是对称的。"股票长期平均正收益，且空头需支付借券费和股息，长期持有空头成本很高。

# Vocabulaire

| français | 中文 | English |
|---|---|---|
| la vente à découvert (f.) | 做空 | short selling |
| la position courte (f.) | 空头头寸 | short position |
| le prêt de titres (m.) | 借券 | securities lending |
| le dépôt de garantie (m.) | 保证金 | margin |
| l'appel de marge (m.) | 追加保证金 | margin call |
| le rachat (m.) | 平仓买回 | covering |
| le vendeur à découvert (m.) | 卖空者 | short seller |

# Related

- [[Long 做多 position longue|做多]]
- [[Leverage 杠杆|杠杆]]
- [[Option 期权 option|期权]]
- [[Hedge 对冲 couverture|对冲]]
- [[Hedge fund 对冲基金 gestion alternative|对冲基金]]
- [[Speculation 投机|投机]]
- [[Financial risks 金融风险 risques financiers|金融风险]]

# Self-check 自测

> [!question]- 为什么做空的亏损理论上无上限，而做多不是？
> 空头损益 $S_0 - S_t$，$S_t$ 没有上界，所以亏损无界；多头损益 $S_t - S_0$，由于 $S_t \ge 0$，最大亏损为 $S_0$。

> [!question]- 推导卖空追加保证金的触发价 $S^*$。
> 账户资产为卖空所得加初始保证金 $(1+m_0)NS_0$，负债为买回成本 $NS_t$，权益 $E_t = (1+m_0)NS_0 - NS_t$。令 $E_t = m N S_t$，解得 $S^* = (1+m_0)S_0/(1+m)$。

> [!question]- 轧空为什么是一种正反馈？
> 价格上涨使空头亏损扩大、保证金不足，空头被迫买入平仓；这些买单本身推高价格，又迫使更多空头平仓。空头占比越高、借券越难，这种循环越剧烈。
