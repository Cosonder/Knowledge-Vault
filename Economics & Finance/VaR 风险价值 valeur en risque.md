---
aliases:
  - var
  - value at risk
  - valeur en risque
---
Value at risk

# Definition
**风险价值**（Value at Risk, VaR；法 valeur en risque）是衡量市场风险的统计指标：在给定的置信水平（confidence level）$\alpha$ 和持有期（holding period）$T$ 下，正常市场条件中某一资产或[[Portfolio 投资组合 portefeuille|投资组合]]可能遭受的最大损失。

形式化地，设 $L$ 为持有期内的损失，则

$$\text{VaR}_\alpha = \inf\{\, l : P(L > l) \le 1-\alpha \,\}$$

即损失超过 VaR 的概率不超过 $1-\alpha$。例如"1 天、99% VaR = 100 万元"表示：在 100 个交易日中，预计约有 1 天的损失会超过 100 万元。

# Calculation methods
1. **参数法 / 方差-协方差法**（parametric / variance–covariance）：假设收益服从正态分布，
   $$\text{VaR} = z_\alpha \cdot \sigma \cdot \sqrt{T} \cdot V$$
   其中 $V$ 为头寸价值，$\sigma$ 为日波动率，$z_{95\%} \approx 1.645$，$z_{99\%} \approx 2.326$。
2. **历史模拟法**（historical simulation）：用过去实际收益序列重估当前组合，取相应分位数，无需分布假设。
3. **蒙特卡洛模拟法**（Monte Carlo simulation）：按设定的随机过程生成大量情景，适合含期权等非线性头寸的组合。

# Example
某股票组合价值 1000 万元，日波动率 2%，则 1 天 99% VaR 约为
$$2.326 \times 0.02 \times 1000 \approx 46.5 \text{ 万元}$$
10 天 VaR 约为 $46.5 \times \sqrt{10} \approx 147$ 万元（平方根时间法则）。

# Limitations
- **不说明尾部损失大小**：只告诉"超过多少的概率"，不告诉超过时会亏多少。
- **正态假设低估肥尾**（fat tails），2008 年金融危机中 VaR 模型普遍失效。
- **不满足次可加性**（subadditivity），因而不是一致性风险度量（coherent risk measure）。
- 依赖历史数据，对结构性变化反应滞后。

补充指标：**预期亏损**（Expected Shortfall, ES，亦称 CVaR / Conditional VaR），即损失超过 VaR 时的条件期望损失 $ES_\alpha = E[L \mid L > \text{VaR}_\alpha]$。巴塞尔协议（FRTB 框架）已将市场风险资本计量从 VaR 转向 97.5% ES。VaR 也常与 [[Stress test 压力测试 test de résistance|Stress test]] 配合使用，以覆盖极端情景。

# Related
- [[Financial risks 金融风险 risques financiers|Financial risks]]
- [[Risk management 风险管理 gestion des risques|Risk management 风险管理]]
- [[Stress test 压力测试 test de résistance|Stress test]]
- [[Leverage 杠杆]]
