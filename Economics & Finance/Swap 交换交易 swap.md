---
aliases:
  - swap
---
# Definition
**互换 / 交换交易**（swap，法 swap / contrat d'échange）是交易双方约定在未来一段时间内，按预先确定的规则定期交换一系列现金流的[[Derivative 金融衍生品 produit dérivé|金融衍生品]]合约。互换可视为一系列[[Forward contract 远期合同 contrat à terme|远期合约]]的组合，绝大多数在场外市场（OTC，over-the-counter）交易，按 ISDA 主协议签订。

# Types
- **利率互换**（interest rate swap, IRS）：最常见。一方支付固定利率，另一方支付浮动利率（如 SOFR、€STR、SHIBOR、LPR），仅交换利息差额，名义本金（notional principal）不交换。
- **货币互换**（currency swap）：交换不同[[Currency 通货 monnaie|货币]]的本金和利息，期初和期末交换本金。央行间的货币互换协议（如中国人民银行与他国央行）用于提供流动性。
- **信用违约互换**（credit default swap, CDS）：买方定期支付保费，若参考实体发生信用事件（违约），卖方赔偿损失，实质是信用保险；在 2008 年金融危机中扮演重要角色。
- **商品互换**（commodity swap）：以固定价格交换[[Commodity 商品 matière première|商品]]的浮动市场价格。
- **股权互换 / 总收益互换**（equity swap / total return swap, TRS）：一方支付股票或指数总收益，另一方支付利率。

# Mechanism
以利率互换为例：A 公司有浮动利率贷款，担心利率上升；B 公司有固定利率负债，希望转为浮动。双方签订互换：

- A 向 B 支付固定利率 3%
- B 向 A 支付浮动利率 SOFR

A 的净融资成本 = 贷款浮动利率 − 收到的 SOFR + 支付的 3%，从而将浮动利率负债转换为约 3% 的固定利率负债。理论基础之一是比较优势（comparative advantage）：双方在不同市场的融资成本优势不同，互换可降低总融资成本。

# Example
名义本金 1 亿元，A 付固定 3%、收浮动，按年结算。若某年浮动利率为 3.5%，则 B 应付 A 净额 $(3.5\% - 3\%) \times 1 \text{亿} = 50$ 万元；若浮动利率为 2.5%，则 A 付 B 50 万元。

# Uses
- [[Hedge 对冲 couverture|对冲]]利率风险、汇率风险、信用风险
- 改变资产负债的现金流结构（资产负债管理 ALM）
- [[Speculation 投机]]：表达对利率走势的观点
- 风险：交易对手风险（counterparty risk），危机后多数标准化互换须通过中央对手方（CCP）集中清算。

# Related
- [[Derivative 金融衍生品 produit dérivé|Derivative 金融衍生品]]
- [[Forward contract 远期合同 contrat à terme|Forward contract 远期合同]]
- [[Future 期货 contrat à terme normalisé|Future 期货]]
- [[Financial risks 金融风险 risques financiers|Financial risks]]
