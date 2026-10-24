---
aliases:
  - volatility
  - volatilité
  - vol
  - sigma
  - implied volatility
summary: 收益率的标准差，度量价格波动的幅度，不等同于永久亏损的风险
tags: [finance, learning]
---
# Definition

**波动率**（volatility, *volatilité*）是资产[[Return 收益率 rendement|收益率]]的标准差 $\sigma$，通常按年化表示。它度量收益围绕均值的离散程度，是现代金融中最常用的风险代理量。

- **历史波动率**（historical / realized volatility, *volatilité historique*）：由过去收益率样本估计；
- **隐含波动率**（implied volatility, *volatilité implicite*）：由[[Option 期权 option|期权]]市场价格反解定价模型（如 Black–Scholes）得到的 $\sigma$，反映市场对未来波动的预期（含风险溢价）。VIX、VSTOXX 等指数即基于此。

# Formula

## 样本估计

给定 $n$ 个周期对数收益率 $r_1,\dots,r_n$：

$$\hat\sigma = \sqrt{\frac{1}{n-1}\sum_{t=1}^{n}(r_t-\bar r)^2}.$$

## $\sqrt{T}$ 缩放

若各期收益率独立同分布（i.i.d.），方差 $\sigma_1^2$，则 $T$ 期对数收益率之和的方差为 $T\sigma_1^2$，故

$$\sigma_T = \sigma_1\sqrt{T}.$$

日波动率年化：$\sigma_{\text{ann}} = \sigma_{\text{day}}\sqrt{252}$（约 252 个[[Trading day 交易日|交易日]]）；月度：$\sigma_{\text{ann}} = \sigma_{\text{month}}\sqrt{12}$。

注意：这依赖独立性。实际收益率存在波动聚集（volatility clustering）和一定的序列相关，$\sqrt{T}$ 规则只是近似。

## 年化收益率的离散度随期限缩小

$T$ 年的**年化**平均对数收益率的标准差为 $\sigma\sqrt{T}/T = \sigma/\sqrt{T}$，随 $T$ 增大而减小；但**累计**收益（财富水平）的不确定性 $\sigma\sqrt{T}$ 随 $T$ 增大。两者不可混淆。

# Example

某股票指数日收益率标准差为 $1.1\%$，则年化波动率约 $1.1\%\times\sqrt{252} \approx 17.5\%$。若年化期望对数收益率为 $6\%$，在正态近似下：

- 1 年：年化收益落在 $6\%\pm17.5\%$（约 68% 概率区间），亏损概率 $\Phi(-6/17.5)\approx 37\%$；
- 20 年：年化收益的标准差 $17.5\%/\sqrt{20}\approx 3.9\%$，年化收益为负的概率 $\Phi(-6/3.9)\approx 6\%$。

（以上假设 i.i.d. 正态且参数已知，现实中的尾部更厚，参数也不确定。）

# Common misconceptions

- **波动率 ≠ 永久亏损的风险**：波动率度量的是路径上的上下起伏。永久亏损（*perte en capital définitive*）来自发行企业破产、在低点被迫卖出、使用[[Leverage 杠杆|杠杆]]被强平、或集中持有单一资产。一个分散化的指数在长期内可以经历高波动而未出现永久损失；一只低波动的个股也可能突然归零。
- **"Bourse = casino"**：赌场游戏的期望收益为负且固定（庄家优势），结果独立于任何经济产出；而持有分散的[[Stock 股票 action|股票]]组合，是对企业利润和[[Dividend 股息 dividende|股息]]的所有权，长期期望实际收益历史上为正。短期价格波动大，并不意味着期望为负。将其等同于赌博，混淆了**方差**与**期望**。不过，短线高频交易、高杠杆或[[Speculation 投机|投机]]行为在结构上可以更接近赌博。
- **"低波动 = 安全"**：现金的名义波动接近零，但实际购买力受[[Inflation 通货膨胀 inflation|通货膨胀]]持续侵蚀。
- **标准差刻画全部风险**：它是对称的，不区分上行与下行，也无法描述厚尾；[[VaR 风险价值 valeur en risque|VaR]]、最大回撤（*drawdown maximal*）等是补充指标。

# Vocabulaire

| français | 中文 | English |
|---|---|---|
| *la volatilité* (f.) | 波动率 | volatility |
| *l'écart-type* (m.) | 标准差 | standard deviation |
| *la volatilité implicite* (f.) | 隐含波动率 | implied volatility |
| *le krach* (m.) | 崩盘 | crash |
| *le drawdown / la perte maximale* (f.) | 最大回撤 | maximum drawdown |
| *la perte en capital* (f.) | 本金损失 | capital loss |
| *le casino* (m.) | 赌场 | casino |

# Related

- [[Return 收益率 rendement|收益率]]
- [[Diversification 分散投资 diversification|分散投资]]
- [[Asset allocation 资产配置 allocation d'actifs|资产配置]]
- [[Option 期权 option|期权]]
- [[VaR 风险价值 valeur en risque|VaR]]
- [[Financial risks 金融风险 risques financiers|金融风险]]
- [[Speculation 投机|投机]]
- [[Efficient market hypothesis 有效市场假说 hypothèse des marchés efficients|有效市场假说]]

# Self-check 自测

> [!question]- 月波动率 5%，年化波动率约多少？需要什么假设？
> $5\%\times\sqrt{12}\approx 17.3\%$。假设各月收益率独立同分布（至少不相关且方差相同）。

> [!question]- 为什么说"持有越久，股票风险越小"只对一半？
> 年化收益率的标准差 $\sigma/\sqrt T$ 随期限下降，但终值财富的不确定性 $\sigma\sqrt T$ 随期限上升；而且两者都依赖 i.i.d. 假设与参数的稳定性。

> [!question]- 用期望与方差的语言区分轮盘赌与分散的股票指数。
> 轮盘赌：每次下注期望收益为负（欧式轮盘约 $-1/37$），方差大。分散的股票指数：期望实际收益（历史上）为正，方差也大。两者都有高方差，但期望的符号不同。
