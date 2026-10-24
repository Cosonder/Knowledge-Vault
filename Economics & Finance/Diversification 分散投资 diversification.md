---
aliases:
  - diversification
  - diversify
  - systematic risk
  - idiosyncratic risk
  - risque systématique
summary: 持有相关性不完全的多种资产以降低组合波动，只能消除非系统性风险
tags: [finance, learning]
---
# Definition

**分散投资**（diversification）指在[[Portfolio 投资组合 portefeuille|投资组合]]中持有多种相关性不完全的资产，使各自的特有波动部分相互抵消，从而在不必降低期望收益的前提下降低组合[[Volatility 波动率 volatilité|波动率]]。俗语"不要把所有鸡蛋放在一个篮子里"（*ne pas mettre tous ses œufs dans le même panier*）。

资产的总风险可分解为：

- **系统性风险**（systematic / market risk, *risque systématique*）：影响整个市场的共同因素（经济周期、利率、战争），无法通过分散消除；
- **非系统性风险**（idiosyncratic / specific risk, *risque spécifique*）：个别公司或行业特有的事件（管理失误、诉讼、产品失败），可通过分散消除。

# Formula

## 组合方差

权重 $w_i$（$\sum w_i=1$），资产波动率 $\sigma_i$，相关系数 $\rho_{ij}$，协方差 $\sigma_{ij}=\rho_{ij}\sigma_i\sigma_j$：

$$\sigma_p^2 = \mathbf w^\top\Sigma\,\mathbf w = \sum_i w_i^2\sigma_i^2 + \sum_{i\ne j} w_iw_j\rho_{ij}\sigma_i\sigma_j.$$

两资产情形：$\sigma_p^2 = w_1^2\sigma_1^2 + w_2^2\sigma_2^2 + 2w_1w_2\rho\,\sigma_1\sigma_2$。由于 $\rho\le1$，有 $\sigma_p \le w_1\sigma_1 + w_2\sigma_2$，等号仅当 $\rho = 1$。而组合期望收益恰为加权平均 $\mu_p = \sum w_i\mu_i$。这一不对称性就是分散化的"免费午餐"。

## $n$ 项等权资产的极限

设 $n$ 项资产方差均为 $\sigma^2$、两两相关系数均为 $\rho$，取 $w_i = 1/n$：

$$\sigma_p^2 = \frac{1}{n}\sigma^2 + \frac{n(n-1)}{n^2}\rho\sigma^2 = \rho\sigma^2 + \frac{(1-\rho)\sigma^2}{n}.$$

当 $n\to\infty$，

$$\sigma_p^2 \;\longrightarrow\; \rho\,\sigma^2.$$

第二项 $(1-\rho)\sigma^2/n$ 是可分散的非系统性部分；$\rho\sigma^2$ 是不可分散的系统性部分。更一般地，在单因子模型 $R_i = \alpha_i + \beta_i R_m + \varepsilon_i$ 下，$\sigma_p^2 \to \beta_p^2\sigma_m^2$。

# Example

个股年化波动率 $\sigma = 30\%$，两两相关 $\rho = 0.3$：

| $n$ | $\sigma_p$ |
|---|---|
| 1 | 30.0% |
| 10 | $\sqrt{0.027 + 0.063/10}\approx 18.2\%$ |
| 30 | $\sqrt{0.027 + 0.0021}\approx 17.1\%$ |
| $\infty$ | $\sqrt{0.027}\approx 16.4\%$ |

从 1 只到 30 只，波动率下降约 43%，此后边际效果很小，极限由 $\rho$ 决定。[[Index fund 指数基金 fonds indiciel|指数基金]]与[[ETF 交易所交易基金 fonds négocié en bourse|ETF]]以低成本实现了大规模分散。

# Common misconceptions

- **"持有很多只就算分散"**：若资产高度相关（同一行业、同一国家），$\rho$ 大，极限 $\rho\sigma^2$ 仍然高。真正有效的是降低相关性，例如跨地区、跨[[Asset allocation 资产配置 allocation d'actifs|资产类别]]。
- **"分散化能消除所有风险"**：系统性风险无法分散；而且危机中相关性往往上升，分散效果在最需要时减弱。
- **"分散会降低收益"**：等权组合的期望收益是平均值，不是最小值；被"放弃"的只是押中单一赢家的可能，同时也避开了押中输家。

# Vocabulaire

| français | 中文 | English |
|---|---|---|
| *la diversification* (f.) | 分散投资 | diversification |
| *le risque systématique* (m.) | 系统性风险 | systematic risk |
| *le risque spécifique* (m.) | 非系统性（特有）风险 | idiosyncratic risk |
| *la corrélation* (f.) | 相关性 | correlation |
| *la covariance* (f.) | 协方差 | covariance |
| *le panier* (m.) | 篮子 | basket |
| *la pondération* (f.) | 权重 | weighting |

# Related

- [[Portfolio 投资组合 portefeuille|投资组合]]
- [[Volatility 波动率 volatilité|波动率]]
- [[Asset allocation 资产配置 allocation d'actifs|资产配置]]
- [[Index fund 指数基金 fonds indiciel|指数基金]]
- [[ETF 交易所交易基金 fonds négocié en bourse|ETF]]
- [[Risk management 风险管理 gestion des risques|风险管理]]
- [[Hedge 对冲 couverture|对冲]]
- [[Efficient market hypothesis 有效市场假说 hypothèse des marchés efficients|有效市场假说]]

# Self-check 自测

> [!question]- 两资产 $\sigma_1=\sigma_2=\sigma$，$\rho=-1$，等权组合波动率是多少？
> $\sigma_p^2 = \tfrac14\sigma^2+\tfrac14\sigma^2 - 2\cdot\tfrac14\sigma^2 = 0$。完全负相关时可构造无风险组合。

> [!question]- 等权 $n$ 资产组合方差公式中，为什么协方差项最终主导？
> 方差项共 $n$ 个，每个权重 $1/n^2$，合计 $O(1/n)$；协方差项共 $n(n-1)$ 个，每个权重 $1/n^2$，合计趋于 $\rho\sigma^2$，为 $O(1)$。

> [!question]- 为什么 CAPM 认为只有系统性风险能获得风险溢价？
> 非系统性风险可以零成本地分散掉，均衡中市场不会为投资者自愿承担的可消除风险支付补偿；只有不可分散的 $\beta$ 风险才被定价。
