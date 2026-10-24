---
aliases:
  - forward contract
  - contrat à terme
  - contrat à terme de gré à gré
---
# Definition

**远期合同**（forward contract, *contrat à terme de gré à gré*）是买卖双方约定在**未来某一确定日期**、以**事先确定的价格**（远期价格 forward price, $F$）买卖一定数量标的资产的协议。它是最基本的[[Derivative 金融衍生品 produit dérivé|金融衍生品]]。

- 同意在未来买入的一方持有**多头**（long position），见 [[Long 做多 position longue|做多]]；
- 同意在未来卖出的一方持有**空头**（short position）。

# Mechanism

远期合同在**场外**（OTC）由双方私下签订，条款（数量、品质、交割日、交割地点）可完全定制。签约时通常不付任何费用，合约初始价值为 0；到期时按约定价格交割实物或进行现金差额结算。

到期时多头的收益（payoff）为：

$$\text{Payoff}_{\text{long}} = S_T - F, \qquad \text{Payoff}_{\text{short}} = F - S_T$$

其中 $S_T$ 为到期日标的的即期价格（spot price）。

在无套利条件下，不付收益的资产的远期价格为

$$F_0 = S_0\, e^{rT}$$

其中 $S_0$ 为当前现货价格，$r$ 为无风险利率（连续复利，见 [[Compound interest 复利 intérêts composés|复利]]），$T$ 为期限（年）。

# Forward vs. Futures

| 维度 | 远期 | [[Future 期货 contrat à terme normalisé|期货]] |
|---|---|---|
| 交易场所 | 场外 | 交易所 |
| 标准化 | 定制 | 标准化 |
| 结算 | 到期一次结算 | 每日盯市（marking to market） |
| 信用风险 | 存在对手方风险（counterparty risk） | 由清算所担保，风险很小 |
| 流动性 | 低，难以转让 | 高 |

# Example

一家中国出口企业 3 个月后将收到 100 万美元，担心人民币升值，于是与银行签订远期合同，约定 3 个月后以 7.10 的汇率卖出美元。到期时即期汇率若为 7.00，企业仍按 7.10 结汇，多得 $100\text{万}\times(7.10-7.00)=10$ 万元；若即期汇率为 7.20，则少得 10 万元。无论哪种情况，企业都锁定了收入，这就是[[Hedge 对冲 couverture|对冲]]。

# Related

- [[Swap 交换交易 swap|交换交易]]
- [[Risk management 风险管理 gestion des risques|风险管理]]
- [[Currency 通货 monnaie|通货]]
