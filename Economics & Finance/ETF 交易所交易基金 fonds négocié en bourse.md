---
aliases:
  - etf
  - exchange-traded fund
  - fonds négocié en bourse
  - tracker
  - fonds indiciel coté
summary: 在交易所像股票一样买卖的基金，多为指数基金
tags: [finance, learning]
---
# Definition

**ETF**（exchange-traded fund, *fonds négocié en bourse*；法语日常称 ***tracker*** 或 *fonds indiciel coté*）是在[[Stock exchange 证券交易所 bourse|证券交易所]]上市、可在交易时段内像[[Stock 股票 action|股票]]一样连续买卖的基金。绝大多数 ETF 是[[Index fund 指数基金 fonds indiciel|指数基金]]，复制某一指数的表现。

ETF 有两个价格：**市价**（市场成交价）和**净值**（NAV, *valeur liquidative*），即每份额对应的资产价值：

$$\mathrm{NAV} = \frac{\text{资产市值} - \text{负债}}{\text{份额数}}.$$

# Mechanism

**申购与赎回（creation / redemption）**。ETF 在[[Primary market 一级市场 marché primaire|一级市场]]只与少数**授权参与者**（authorised participants, AP，通常是大型券商）交易，且以"一篮子股票 ↔ 大额 ETF 份额"实物交换为主；普通投资者在[[Secondary market 二级市场 marché secondaire|二级市场]]相互买卖份额。

这一机制形成套利，使市价贴近 NAV：

- 若市价 $>$ NAV（溢价）：AP 买入一篮子成分股，向基金申购新份额，在市场卖出，赚取差价，份额供给增加压低市价；
- 若市价 $<$ NAV（折价）：AP 在市场买入份额，向基金赎回换得股票并卖出，份额减少推高市价。

**实物复制与合成复制**。
- **实物复制**（physical replication, *réplication physique*）：基金真实持有成分股，可全量复制或抽样复制。
- **合成复制**（synthetic replication, *réplication synthétique*）：基金持有另一篮子资产，并与银行签订总收益[[Swap 交换交易 swap|互换]]，由对手方支付指数收益。优点是跟踪误差小、可复制难以直接持有的市场；缺点是引入对手方风险（欧盟 UCITS 规则将其敞口限制在净值的 10%）。在法国，合成 ETF 使 PEA 账户也能投资全球指数。

**累积型与分配型**。
- **累积型**（accumulating, *capitalisant*，代码常带 Acc / C）：[[Dividend 股息 dividende|股息]]自动再投资，体现在 NAV 中；
- **分配型**（distributing, *distribuant*，Dist / D）：定期向持有人派息。

两者税前总收益相同，差别在于现金流形式和税务处理。

# ETF vs mutual fund

| | ETF | 传统[[Mutual fund 共同基金 fonds commun de placement\|共同基金]] |
|---|---|---|
| 交易 | 盘中连续，按市价 | 每日一次，按收盘 NAV |
| 管理方式 | 多为被动 | 多为主动 |
| 费用 | 通常低（0.05%–0.5%） | 通常高，可能含申购费 |
| 成本 | 有买卖价差、佣金 | 无价差 |
| 透明度 | 通常每日公布持仓 | 定期公布 |

# Example

某 MSCI World ETF 的 NAV 为 100.00 欧元，市场报价 100.30 欧元（溢价 0.3%）。AP 以 100.00 欧元/份的成本买入一篮子股票，申购 50 000 份，在市场以 100.30 卖出，毛利约 $50000 \times 0.30 = 15\,000$ 欧元（扣除交易成本前）。持续的卖出压力把市价推回接近 100.00。

# Common misconceptions

- "ETF 都是低风险的。"ETF 只是包装形式；杠杆 ETF、反向 ETF、单一行业 ETF 风险可以很高。
- "ETF 交易量小就不能买。"流动性最终取决于成分股的流动性，AP 可随时创造份额；但小 ETF 的买卖价差可能较大。
- "合成 ETF 不持有任何资产。"它持有抵押资产篮子，只是收益来源于互换。

# Vocabulaire

| français | 中文 | English |
|---|---|---|
| le tracker (m.) | ETF（口语） | tracker, ETF |
| la valeur liquidative (f.) | 基金净值 | net asset value |
| la réplication physique (f.) | 实物复制 | physical replication |
| la réplication synthétique (f.) | 合成复制 | synthetic replication |
| capitalisant / distribuant (adj.) | 累积型 / 分配型 | accumulating / distributing |
| le teneur de marché (m.) | 做市商 | market maker |
| l'écart acheteur-vendeur (m.) | 买卖价差 | bid–ask spread |

# Related

- [[Index fund 指数基金 fonds indiciel|指数基金]]
- [[Mutual fund 共同基金 fonds commun de placement|共同基金]]
- [[Investment fund 证券投资基金 fonds d'investissement|证券投资基金]]
- [[Swap 交换交易 swap|互换]]
- [[Dividend 股息 dividende|股息]]
- [[Investment fees 投资费用 frais|投资费用]]
- [[Diversification 分散投资 diversification|分散投资]]

# Self-check 自测

> [!question]- ETF 折价时，套利机制如何把价格推回 NAV？
> AP 在二级市场以低于 NAV 的价格买入 ETF 份额，向基金赎回换得等值的一篮子股票，再卖出股票获利。市场上份额被买走、总份额减少，买入压力推高市价，直到折价小于交易成本。

> [!question]- 合成复制 ETF 的主要额外风险是什么？
> 对手方风险：若互换对手方违约，基金拿不到指数收益，只剩抵押资产篮子的价值。UCITS 规定对单一对手方的敞口不超过净值的 10%，且通常每日重置。

> [!question]- 累积型和分配型 ETF 的税前总收益是否相同？
> 相同（忽略再投资的时点和成本）。累积型把股息留在基金内部再投资，NAV 更高；分配型发放现金，NAV 相应较低。区别在于税务（如股息是否当年计税）与现金流需求。
