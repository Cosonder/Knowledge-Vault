---
aliases:
  - derivative
  - produit dérivé
---
# Definition

**金融衍生品**（derivative, *produit dérivé*）是一种金融合约，其价值取决于（derived from）某个**标的资产**（underlying asset）的价格或某个指标的变化。标的可以是 [[Stock 股票 action|股票]]、债券、[[Commodity 商品 matière première|商品]]、[[Currency 通货 monnaie|货币]]、利率、股价指数（如 [[Standard & Poor’s 500 标准普尔指数 indice S&P 500|S&P 500]]），甚至是信用事件或天气。

衍生品本身不代表对标的的所有权，而是对未来某种权利或义务的约定。

# Classification

按合约形式，常见的基本衍生品有四类：

| 类型 | 英文 / français | 特点 |
|---|---|---|
| 远期 | forward / *contrat à terme de gré à gré* | 场外（OTC）、非标准化，双方约定未来以固定价格交割，见 [[Forward contract 远期合同 contrat à terme\|远期合同]] |
| 期货 | futures / *contrat à terme standardisé* | 交易所交易、标准化、每日盯市结算，见 [[Future 期货 contrat à terme normalisé\|期货]] |
| 期权 | option / *option* | 买方支付权利金，获得在未来以约定价格买入（call）或卖出（put）的**权利**而非义务 |
| 互换 | swap / *swap* | 双方交换一系列现金流，如固定利率换浮动利率，见 [[Swap 交换交易 swap\|交换交易]] |

按交易场所可分为**场内**（exchange-traded）与**场外**（over-the-counter, OTC）衍生品。

# Mechanism

衍生品的两个核心特征：

1. **杠杆性**：通常只需支付保证金（margin）或权利金即可获得对较大名义本金（notional）的风险敞口，因此收益和亏损都被放大，见 [[Leverage 杠杆 effet de levier|杠杆]]。
2. **零和性**（在不计交易成本时）：一方的盈利即另一方的亏损。

# Uses

- **对冲**（hedging）：用衍生品抵消现有头寸的价格风险，见 [[Hedge 对冲 couverture|对冲]]。如航空公司买入原油期货锁定燃油成本。
- **投机**（speculation）：利用杠杆押注价格方向，见 [[Speculation 投机 spéculation|投机]]。
- **套利**（arbitrage）：利用衍生品与现货之间的定价偏差获取无风险或低风险收益。

# Example

某投资者以 2 元/股的权利金买入一份行权价 50 元、对应 100 股的看涨期权，成本 200 元。到期时股价为 60 元，则行权收益为 $(60-50)\times 100 = 1000$ 元，净利润 800 元，收益率 400%；若股价低于 50 元，则期权作废，最大损失为 200 元权利金。

# Related

- [[Asset 资产 actif|资产]]
- [[Financial risks 金融风险 risques financiers|Financial risks]]
- [[Risk management 风险管理 gestion des risques|风险管理]]
- [[Hedge fund 对冲基金 gestion alternative|对冲基金]]
- [[Securities market 证券市场 marché des valeurs mobilières|证券市场]]
- [[Option 期权 option|期权]]
