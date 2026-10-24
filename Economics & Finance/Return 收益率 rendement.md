---
aliases:
  - return
  - rendement
  - rate of return
  - log return
  - cagr
  - total return
summary: 一段时间内投资的价值变化（含分红）与初始价值之比
tags: [finance, learning]
---
# Definition

**收益率**（return, *rendement*）衡量一项投资在一段时间内的相对价值变化。设期初价格 $P_0$、期末价格 $P_1$、期间收到的现金分配（如[[Dividend 股息 dividende|股息]]、票息）$D_1$，则该期的**总收益率**（total return, *rendement total*）为

$$R = \frac{P_1 + D_1 - P_0}{P_0}.$$

只看 $(P_1-P_0)/P_0$ 的是**价格收益率**（price return）。指数也分价格指数与**全收益指数**（total return index，股息再投资）；长期比较必须用后者。

# Formula

## 简单收益率与对数收益率

**简单收益率** $R_t = P_t/P_{t-1} - 1$；**对数收益率**（log return, *rendement logarithmique*）$r_t = \ln(P_t/P_{t-1}) = \ln(1+R_t)$。

- 多期复合：简单收益率**相乘** $1+R_{0\to n} = \prod_t (1+R_t)$；对数收益率**相加** $r_{0\to n} = \sum_t r_t$。
- 跨资产聚合：组合的简单收益率是成分简单收益率的加权和 $R_p = \sum_i w_i R_i$；对数收益率不满足这一点。
- $r \le R$，且 $r \approx R - R^2/2$（$|R|$ 小时）。

## 算术平均与几何平均

$n$ 期收益率 $R_1,\dots,R_n$：

$$\bar R_A = \frac1n\sum_t R_t, \qquad \bar R_G = \Big(\prod_t (1+R_t)\Big)^{1/n} - 1.$$

由 AM–GM 不等式，$\bar R_G \le \bar R_A$，等号当且仅当各期相同。近似关系 $\bar R_G \approx \bar R_A - \tfrac12\sigma^2$（$\sigma$ 为[[Volatility 波动率 volatilité|波动率]]），即"波动拖累"（volatility drag）。投资者实际获得的财富增长由几何平均决定，后者也称**年复合增长率**（CAGR, *taux de croissance annuel composé*, TCAC）。

## 年化（annualization）

$T$ 年的累计收益率 $R_{\text{cum}}$ 的年化值为 $(1+R_{\text{cum}})^{1/T}-1$。月度对数收益率均值 $\mu_m$ 年化为 $12\mu_m$；月度简单收益率则应复合：$(1+R_m)^{12}-1$。

## 名义与实际收益率

与 [[Interest rate 利率 taux d'intérêt|Fisher 方程]] 相同：$1+R_{\text{real}} = \dfrac{1+R_{\text{nom}}}{1+\pi}$。衡量[[Purchasing power 购买力 pouvoir d'achat|购买力]]增长的是实际收益率；扣除[[Investment fees 投资费用 frais|费用]]与税后则是净收益率。

# Example

某资产两年收益率为 $+50\%$、$-50\%$。

- 算术平均：$(50\%-50\%)/2 = 0\%$；
- 几何平均：$\sqrt{1.5\times0.5}-1 = \sqrt{0.75}-1 \approx -13.4\%$；
- 实际财富：100 → 150 → 75，亏损 25%。

对数收益率为 $\ln 1.5 + \ln 0.5 = \ln 0.75 \approx -0.288$，相加即得总对数收益率，一致。

# Common misconceptions

- **"平均收益率 10% 就意味着每年财富增长 10%"**：报告的若是算术平均，财富的复合增长率更低。
- **"跌 50% 后涨 50% 就回本"**：需要涨 100% 才能回本；一般地，跌 $d$ 需涨 $d/(1-d)$。
- **忽略股息**：长期看，股息再投资占股票总收益的相当部分，只比较价格指数会严重低估。

# Vocabulaire

| français | 中文 | English |
|---|---|---|
| *le rendement* (m.) | 收益率 | return, yield |
| *la rentabilité* (f.) | 回报率、盈利能力 | profitability, return |
| *la plus-value* (f.) | 资本利得 | capital gain |
| *la moins-value* (f.) | 资本损失 | capital loss |
| *la moyenne géométrique* (f.) | 几何平均 | geometric mean |
| *le rendement réel* (m.) | 实际收益率 | real return |
| *le dividende réinvesti* (m.) | 再投资的股息 | reinvested dividend |

# Related

- [[Compound interest 复利 intérêts composés|复利]]
- [[Volatility 波动率 volatilité|波动率]]
- [[Dividend 股息 dividende|股息]]
- [[Inflation 通货膨胀 inflation|通货膨胀]]
- [[Interest rate 利率 taux d'intérêt|利率]]
- [[Investment fees 投资费用 frais|投资费用]]
- [[Index fund 指数基金 fonds indiciel|指数基金]]
- [[Portfolio 投资组合 portefeuille|投资组合]]

# Self-check 自测

> [!question]- 证明组合的简单收益率等于成分简单收益率的加权和。
> 设初始财富 $W_0$，权重 $w_i$，则 $W_1 = \sum_i w_iW_0(1+R_i)$，于是 $W_1/W_0 - 1 = \sum_i w_i(1+R_i) - 1 = \sum_i w_iR_i$（用到 $\sum w_i = 1$）。

> [!question]- 年化算术平均 8%、年化波动率 20%，几何平均约为多少？
> $\bar R_G \approx 8\% - \tfrac12(0.2)^2 = 8\% - 2\% = 6\%$。

> [!question]- 10 年累计收益 100%，年化收益率是多少？
> $2^{1/10}-1 \approx 7.18\%$。
