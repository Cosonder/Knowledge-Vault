---
aliases:
  - portfolio
  - portefeuille
---
# Definition

In [[Finance 金融 finance|finance]], a **portfolio** is a collection of [[Investment 投资 investissement|investments]].

**投资组合**（portfolio, *portefeuille*）是投资者所持有的各类[[Asset 资产 actif|资产]]的集合，如[[Stock 股票 action|股票]]、债券、现金、[[Fund 基金 fonds|基金]]、[[Real estate 不动产 immobilier|不动产]]、[[Commodity 商品 matière première|商品]]等。研究的重点不是单个资产，而是资产**组合在一起**之后的整体收益与风险。

# Core ideas

**资产配置**（asset allocation）：决定各大类资产所占比例，通常被认为是决定组合长期表现的最重要因素。

**分散化**（diversification）：不同资产的价格变动并不完全同步，组合在一起可以降低整体波动。风险可分为：

- **非系统性风险**（idiosyncratic risk）：单个公司或行业特有，可通过分散化消除；
- **系统性风险**（systematic / market risk）：影响整个市场，无法通过分散化消除。

**现代投资组合理论**（Modern Portfolio Theory, Markowitz 1952）：在给定风险下最大化预期收益，所有最优组合构成**有效前沿**（efficient frontier）。

两资产组合的预期收益与方差：

$$E[R_p] = w_1 E[R_1] + w_2 E[R_2]$$

$$\sigma_p^2 = w_1^2\sigma_1^2 + w_2^2\sigma_2^2 + 2w_1w_2\rho_{12}\sigma_1\sigma_2$$

其中 $w_i$ 为权重，$\sigma_i$ 为标准差，$\rho_{12}$ 为相关系数。只要 $\rho_{12} < 1$，组合的标准差就小于两者标准差的加权平均。

# Example

资产 A：预期收益 10%，标准差 20%；资产 B：预期收益 4%，标准差 5%；相关系数 0。各配 50%：

- $E[R_p] = 0.5\times10\% + 0.5\times4\% = 7\%$
- $\sigma_p = \sqrt{0.25\times0.04 + 0.25\times0.0025} \approx 10.3\%$

低于两者加权平均的 12.5%。

**再平衡**（rebalancing）：定期将偏离目标比例的组合调整回去。

# Related

- [[Investment strategy 投资策略 stratégie d'investissement|投资策略]]
- [[Risk management 风险管理 gestion des risques|风险管理]]
- [[Investment fund 证券投资基金 fonds d'investissement|证券投资基金]]
- [[VaR 风险价值 valeur en risque|VaR]]
- [[Diversification 分散投资 diversification|分散投资]]
- [[Asset allocation 资产配置 allocation d'actifs|资产配置]]
