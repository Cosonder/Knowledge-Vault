---
aliases:
  - financial risks
  - financial risk
  - risques financiers
---
# Definition
**金融风险**（financial risk，法 risque financier）指在金融活动中，由于各种不确定因素导致经济主体的实际收益偏离预期、遭受损失的可能性。在现代金融理论中，风险常以收益的波动性（如标准差 $\sigma$）或潜在损失（如 [[VaR 风险价值 valeur en risque|VaR]]）来度量。

# Classification
常见分类（参照巴塞尔协议 Basel 框架）：
- **市场风险**（market risk，法 risque de marché）：因市场价格变动造成的损失。
  - 利率风险（interest rate risk）
  - 汇率风险（currency / FX risk）：见 [[Currency 通货 monnaie|Currency 通货]]
  - 股票价格风险（equity risk）
  - 商品价格风险（commodity risk）：见 [[Commodity 商品 matière première|Commodity 商品]]
- **信用风险**（credit risk，法 risque de crédit）：交易对手或借款人违约（default）、无法履约的风险；衍生品中又称交易对手风险（counterparty risk）。
- **流动性风险**（liquidity risk，法 risque de liquidité）：
  - 市场流动性风险：无法以合理价格迅速变现资产。
  - 融资流动性风险：无法及时获得资金偿还到期债务。
- **操作风险**（operational risk，法 risque opérationnel）：内部流程、人员、系统失误或外部事件（如欺诈、IT 故障）造成的损失。
- 其他：法律与合规风险、模型风险（model risk）、系统性金融风险（systemic risk，区别于下文的 systematic risk）。

另一种重要区分：
- **系统性风险**（systematic risk，不可分散风险）：影响整个市场，如经济衰退、利率变化，用 β 衡量。
- **非系统性风险**（idiosyncratic / specific risk，可分散风险）：特定公司或行业特有，可通过分散化的[[Portfolio 投资组合 portefeuille|投资组合]]降低。

# Measurement
- 波动率（volatility）、β 系数
- [[VaR 风险价值 valeur en risque|VaR]]（风险价值）及预期亏损（Expected Shortfall）
- [[Stress test 压力测试 test de résistance|Stress test]]（压力测试）：模拟极端情景下的损失
- 信用风险中：违约概率 PD、违约损失率 LGD、违约风险暴露 EAD，预期损失 $EL = PD \times LGD \times EAD$

# Example
某银行向企业贷款 1000 万元，违约概率 $PD = 2\%$，违约损失率 $LGD = 40\%$，则预期损失 $EL = 0.02 \times 0.4 \times 1000 = 8$ 万元。

# Related
- [[Risk management 风险管理 gestion des risques|Risk management 风险管理]]
- [[Hedge 对冲 couverture|Hedge 对冲]]
- [[Leverage 杠杆 effet de levier]]：放大各类风险敞口。
- [[Derivative 金融衍生品 produit dérivé|Derivative 金融衍生品]]
