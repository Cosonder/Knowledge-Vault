---
aliases:
  - hedge
  - hedging
  - couverture
---
# Definition
**对冲**（hedge / hedging，法 couverture）是指持有一个与现有风险敞口（exposure）价值变动方向相反的头寸，以抵消或降低价格不利变动带来的损失的风险管理策略。对冲的目的在于**降低不确定性**，而不是获利；代价是同时放弃部分潜在收益，并承担对冲成本。

英语 hedge 原意为"树篱"，引申为"设限、防护"；俗语 hedge one's bets（两边下注）即此义。

# Mechanism
对冲头寸与被对冲资产的价值变化应呈负相关。最小方差对冲比率（minimum variance hedge ratio）为：

$$h^* = \rho \cdot \frac{\sigma_S}{\sigma_F}$$

其中 $\sigma_S$、$\sigma_F$ 分别为现货和期货价格变化的标准差，$\rho$ 为两者相关系数。所需合约数 $N^* = h^* \cdot \dfrac{Q_A}{Q_F}$（$Q_A$ 为被对冲头寸规模，$Q_F$ 为每份合约规模）。

# Instruments
- [[Future 期货 contrat à terme normalisé|期货]]与[[Forward contract 远期合同 contrat à terme|远期]]：锁定未来价格。
  - 多头对冲 / 买入套期保值（long hedge）：未来要买入资产者（如航空公司买原油）。
  - 空头对冲 / 卖出套期保值（short hedge）：未来要卖出资产者（如农民卖小麦）。
- 期权（option）：如买入看跌期权（protective put），在限制下行损失的同时保留上行收益，代价是期权费。
- [[Swap 交换交易 swap|互换]]：对冲利率、汇率和信用风险。
- 自然对冲（natural hedge）：通过经营安排匹配收支币种，如在海外市场本地生产。
- 分散化（diversification）：[[Portfolio 投资组合 portefeuille|投资组合]]中配置低相关资产。

# Example
某出口商 3 个月后将收到 100 万美元，担心美元贬值。现在以 1 USD = 7.20 CNY 卖出 3 个月美元远期。若届时即期汇率跌至 7.00，现货端少收 $100 \times 0.20 = 20$ 万元，远期端盈利 20 万元，两者抵消，锁定收入 720 万元；反之若美元升值，出口商也无法享受升值收益。

# Basis risk
对冲很少完美。现货价格与期货价格之差称为**基差**（basis = spot − futures），基差的不确定变动称为基差风险（basis risk）；用相关但不同的资产对冲（cross hedging）时该风险更大。

# Distinction
- 对冲 vs. [[Speculation 投机 spéculation|投机]]：对冲减少既有风险，投机主动承担风险以博取收益。同一种工具（如期货）可用于两种目的。
- 对冲 vs. [[Hedge fund 对冲基金 gestion alternative|对冲基金]]：对冲基金得名于早期的多空对冲策略，但现代对冲基金泛指采用灵活策略（含[[Leverage 杠杆 effet de levier|杠杆]]、做空）的私募基金，未必以对冲为主。

# Related
- [[Risk management 风险管理 gestion des risques|Risk management 风险管理]]
- [[Financial risks 金融风险 risques financiers|Financial risks]]
- [[Derivative 金融衍生品 produit dérivé|Derivative 金融衍生品]]
- [[Long 做多 position longue|Long 做多]]
