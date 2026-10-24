---
aliases:
  - future
  - futures
  - contrat à terme normalisé
---
# Definition
**期货**（futures contract，常简称 future / futures；法 contrat à terme normalisé，亦称 contrat future）是在期货交易所集中交易的标准化合约，约定买卖双方在未来某一特定日期，按事先确定的价格交割一定数量和质量的标的资产（underlying asset）。期货是最基本的[[Derivative 金融衍生品 produit dérivé|金融衍生品]]之一。

# Futures vs. forwards
期货与[[Forward contract 远期合同 contrat à terme|远期合约]]本质相同，区别在于交易方式：

| | 期货 future | 远期 forward |
|---|---|---|
| 交易场所 | 交易所（exchange-traded） | 场外（OTC） |
| 合约条款 | 标准化（数量、质量、交割月） | 双方协商定制 |
| 信用风险 | 由清算所（clearing house）作为中央对手方承担，几乎无对手风险 | 存在交易对手风险 |
| 结算 | 每日盯市（mark-to-market） | 一般到期结算 |
| 平仓 | 可随时对冲平仓，多数不进行实物交割 | 通常持有至到期 |

# Mechanism
- **保证金制度**（margin，法 dépôt de garantie）：交易者只需缴纳合约价值一定比例（通常 5%–15%）的初始保证金（initial margin），因此期货具有内在的[[Leverage 杠杆 effet de levier|杠杆]]。
- **每日结算 / 盯市**：每个交易日结束按结算价计算盈亏并调整保证金账户；余额低于维持保证金（maintenance margin）时，须追加保证金（margin call），否则会被强行平仓。
- **交割**：实物交割（physical delivery）或现金交割（cash settlement，如股指期货）。
- **持有成本模型**（cost of carry）：理论期货价格
  $$F_0 = S_0 \, e^{(r + u - y)T}$$
  其中 $S_0$ 为现货价格，$r$ 为无风险利率，$u$ 为仓储成本，$y$ 为便利收益或股息收益率，$T$ 为期限。

# Classification
- **商品期货**：农产品、金属、能源（见 [[Commodity 商品 matière première|Commodity 商品]]）。
- **金融期货**：股指期货（如沪深 300、S&P 500 期货）、国债期货、利率期货、外汇期货。

# Uses
- [[Hedge 对冲 couverture|套期保值]]（hedging）：生产商、消费者锁定价格。
- [[Speculation 投机 spéculation]]：利用杠杆博取价格变动收益，[[Long 做多 position longue|做多]]或做空均可。
- 套利（arbitrage）：利用期现价差或跨期价差。
- 价格发现：期货价格反映市场对未来现货价格的预期。

# Example
某投资者以 4000 点买入 1 手沪深 300 股指期货（合约乘数 300 元/点），合约价值 120 万元，保证金比例 12%，需保证金 14.4 万元。若指数上涨 2% 至 4080 点，盈利 $80 \times 300 = 2.4$ 万元，相对保证金收益率约 16.7%；下跌 2% 则亏损同等金额。

# Related
- [[Derivative 金融衍生品 produit dérivé|Derivative 金融衍生品]]
- [[Forward contract 远期合同 contrat à terme|Forward contract 远期合同]]
- [[Swap 交换交易 swap|Swap 交换交易]]
- [[Leverage 杠杆 effet de levier]]
- [[Trading day 交易日 jour de bourse]]
