---
aliases:
  - asset allocation
  - allocation d'actifs
  - efficient frontier
  - rebalancing
  - rééquilibrage
summary: 在股票、债券、现金等资产类别之间分配资金的比例与规则
tags: [finance, learning]
---
# Definition

**资产配置**（asset allocation, *allocation d'actifs*）是决定[[Portfolio 投资组合 portefeuille|投资组合]]在各**资产类别**（asset classes, *classes d'actifs*）之间分配比例的过程。主要资产类别：

- **股票**（[[Stock 股票 action|actions]]）：长期期望收益最高，[[Volatility 波动率 volatilité|波动率]]也最高；
- **债券**（[[Bond 债券 obligation|obligations]]）：收益与波动居中，与股票的相关性随时期而变；
- **现金及等价物**（cash, *liquidités*）：如货币基金、[[Savings account 储蓄账户 livret d'épargne|储蓄账户]]，名义波动接近零，但实际收益常接近零或为负；
- 其他：[[Real estate 不动产 immobilier|不动产]]、[[Commodity 商品 matière première|商品]]等。

研究表明，在分散良好的组合中，收益**波动**的大部分来自资产类别比例的选择，而不是具体证券的挑选（Brinson 等，1986）。

# Mechanism

## 均值–方差框架与有效前沿

Markowitz（1952）将配置问题形式化：给定期望收益向量 $\boldsymbol\mu$ 与协方差矩阵 $\Sigma$，对每个目标收益 $m$ 求

$$\min_{\mathbf w}\ \mathbf w^\top\Sigma\mathbf w \quad \text{s.t.}\quad \mathbf w^\top\boldsymbol\mu = m,\ \ \mathbf w^\top\mathbf 1 = 1.$$

这是一个凸二次规划。解集在 $(\sigma_p,\mu_p)$ 平面上构成双曲线的上支，称为**有效前沿**（efficient frontier, *frontière efficiente*）：前沿上的组合在给定风险下收益最高。加入无风险资产（利率 $r_f$）后，最优风险组合是使**夏普比率** $(\mu_p - r_f)/\sigma_p$ 最大的切点组合，所有有效组合都是它与无风险资产的线性组合（两基金分离定理）。

实践局限：$\boldsymbol\mu$ 的估计误差极大，优化器会放大误差、给出极端权重（"误差最大化器"）。因此实务中常用约束、收缩估计或直接采用简单的固定比例。

## 再平衡（rebalancing）

市场波动使实际权重偏离目标权重。**再平衡**（*rééquilibrage*）是定期（如每年）或在偏离超过阈值（如 ±5 个百分点）时，卖出超配资产、买入低配资产，把权重拉回目标。其作用主要是**控制风险**，使组合的风险特征不随行情漂移；它在机制上要求"卖高买低"，但不保证提高收益。成本包括交易[[Investment fees 投资费用 frais|费用]]与税收；用新增资金买入低配资产可减少卖出。

## 基于年龄的规则（仅为启发式）

常见经验法则如"股票比例 $= 100 - \text{年龄}$"（或 110、120 − 年龄），以及目标日期基金的下滑路径（glide path）。它们的逻辑是：年轻人剩余的人力资本（未来工资）类似债券，可承担更多股票风险。这些只是**启发式**（heuristics），未考虑个人的收入稳定性、负债、投资期限、风险承受力与[[Financial independence 财务自由 indépendance financière|财务目标]]，不是最优解。

# Example

目标 60% 股票 / 40% 债券，初始 100 000 欧元。一年后股票涨 20%、债券跌 2%：

- 股票 $60\,000\times1.2 = 72\,000$，债券 $40\,000\times0.98 = 39\,200$，合计 $111\,200$；
- 实际权重：股票 $72000/111200 \approx 64.7\%$；
- 再平衡：目标股票 $0.6\times111200 = 66\,720$，需卖出股票 $5\,280$ 欧元买入债券。

若股票波动率 18%、债券 6%、相关系数 0.1，则 60/40 组合波动率 $\sqrt{0.36\cdot0.0324 + 0.16\cdot0.0036 + 2\cdot0.24\cdot0.1\cdot0.0108}\approx 11.3\%$，低于加权平均 $13.2\%$。

# Common misconceptions

- **"存在一个适合所有人的最优配置"**：最优比例依赖个人约束与偏好；均值–方差最优还依赖不可靠的参数估计。
- **"债券永远对冲股票"**：股债相关性并不稳定，在通胀冲击期（如 2022 年）可同时下跌。
- **"再平衡是为了提高收益"**：其首要目的是维持风险水平。

# Vocabulaire

| français | 中文 | English |
|---|---|---|
| *l'allocation d'actifs* (f.) | 资产配置 | asset allocation |
| *la classe d'actifs* (f.) | 资产类别 | asset class |
| *les liquidités* (f. pl.) | 现金 | cash |
| *le rééquilibrage* (m.) | 再平衡 | rebalancing |
| *la frontière efficiente* (f.) | 有效前沿 | efficient frontier |
| *le ratio de Sharpe* (m.) | 夏普比率 | Sharpe ratio |
| *l'horizon de placement* (m.) | 投资期限 | investment horizon |
| *l'aversion au risque* (f.) | 风险厌恶 | risk aversion |

# Related

- [[Diversification 分散投资 diversification|分散投资]]
- [[Portfolio 投资组合 portefeuille|投资组合]]
- [[Volatility 波动率 volatilité|波动率]]
- [[Return 收益率 rendement|收益率]]
- [[Stock 股票 action|股票]]
- [[Bond 债券 obligation|债券]]
- [[Investment strategy 投资策略|投资策略]]
- [[Index fund 指数基金 fonds indiciel|指数基金]]
- [[Financial independence 财务自由 indépendance financière|财务自由]]

# Self-check 自测

> [!question]- 为什么加入无风险资产后，所有投资者都持有同一个风险组合？
> 资本配置线 $\mu = r_f + \frac{\mu_T - r_f}{\sigma_T}\sigma$ 在切点组合 $T$ 处斜率最大，任何其他风险组合与无风险资产的组合都位于其下方。投资者只通过 $T$ 与无风险资产的比例来调整风险（两基金分离）。

> [!question]- 不做再平衡，长期看 60/40 组合会如何漂移？后果是什么？
> 若股票长期收益更高，股票权重会逐渐上升，组合波动率与回撤风险随之增大，偏离最初设定的风险水平。

> [!question]- "100 − 年龄"规则忽略了哪些因素？
> 收入稳定性与人力资本的性质、已有资产与负债、投资期限与目标、心理上的风险承受能力，以及养老金等其他收入来源。
