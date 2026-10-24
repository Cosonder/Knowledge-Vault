---
aliases:
  - option
  - call option
  - put option
  - option d'achat
  - option de vente
summary: 在约定日期以约定价格买入或卖出标的资产的权利而非义务
tags: [finance, learning]
---
# Definition

**期权**（option, *option*）是一种[[Derivative 金融衍生品 produit dérivé|衍生品]]合约：买方支付**权利金**（premium, *prime*）后，获得在到期日 $T$（或之前）以**行权价**（strike, *prix d'exercice*）$K$ 买入或卖出标的资产的**权利**，但没有义务。卖方（writer）收取权利金，承担相应义务。

- **看涨期权**（call, *option d'achat*）：以 $K$ **买入**的权利；
- **看跌期权**（put, *option de vente*）：以 $K$ **卖出**的权利；
- **欧式**（European）只能在到期日行权，**美式**（American）可在到期前任意时刻行权。

与[[Future 期货 contrat à terme normalisé|期货]]和[[Forward contract 远期合同 contrat à terme|远期]]的关键区别：期货双方都有义务，收益关于 $S_T$ 是线性的；期权收益是非线性的（"凸"的）。

# Formula

**到期收益**（payoff）。记到期时标的价格为 $S_T$：

$$\text{call: } \max(S_T - K, 0) = (S_T - K)^+, \qquad \text{put: } \max(K - S_T, 0) = (K - S_T)^+.$$

扣除权利金 $c$ 或 $p$ 后，买方的**损益**（profit）为 $(S_T-K)^+ - c$ 或 $(K-S_T)^+ - p$；卖方损益为其相反数。看涨买方最大亏损为 $c$，潜在收益无上限；看涨卖方（裸卖）潜在亏损无上限。

**看涨–看跌平价**（put–call parity）。对同一标的、同一 $K$ 和 $T$ 的欧式期权（标的无股息），由恒等式 $(S_T-K)^+ - (K-S_T)^+ = S_T - K$ 和无套利可得

$$c - p = S_0 - K e^{-rT},$$

其中 $r$ 是连续复利无风险[[Interest rate 利率 taux d'intérêt|利率]]。含义：多一个 call、空一个 put 等价于一份行权价为 $K$ 的远期多头。

**Black–Scholes 的直觉**。假设标的价格服从几何布朗运动 $dS = \mu S\,dt + \sigma S\,dW$。关键观察是：在每一瞬间，持有 $\Delta = \partial c / \partial S$ 份股票可以完全对冲期权的随机部分，于是"期权 − $\Delta$ 股股票"的组合是无风险的，只能获得无风险利率 $r$。由此得到的价格**不依赖** $\mu$（预期收益），只依赖[[Volatility 波动率 volatilité|波动率]] $\sigma$。等价地，价格是风险中性测度下的折现期望：

$$c = e^{-rT}\,\mathbb{E}^{\mathbb{Q}}\big[(S_T - K)^+\big] = S_0 N(d_1) - K e^{-rT} N(d_2),$$

$$d_{1,2} = \frac{\ln(S_0/K) + (r \pm \tfrac12\sigma^2)T}{\sigma\sqrt{T}}.$$

由于 payoff 是凸函数，由 Jensen 不等式，$\sigma$ 越大期权越值钱。市场上由期权价格反推出的 $\sigma$ 称为**隐含波动率**（implied volatility）。

# Example

股票现价 $S_0 = 100$ 欧元，买入 $K = 105$、一年期看涨期权，权利金 $c = 6$ 欧元。

- 若 $S_T = 120$：payoff $= 15$，损益 $= 15 - 6 = 9$ 欧元，相对权利金收益 150%；而直接持股收益 20%，体现了[[Leverage 杠杆|杠杆]]效应；
- 若 $S_T = 100$：payoff $= 0$，损失全部权利金 6 欧元；
- 盈亏平衡点：$S_T = K + c = 111$ 欧元。

设 $r = 3\%$，由平价，同条件看跌期权价格应为 $p = c - S_0 + K e^{-rT} = 6 - 100 + 105 e^{-0.03} \approx 7.90$ 欧元。

# Common misconceptions

- "买期权最多亏权利金，所以很安全。"短期价外期权大部分到期归零，亏损概率很高。
- "期权价格取决于股票的预期涨幅。"在 Black–Scholes 框架下与 $\mu$ 无关，因为可以动态对冲。
- 卖出期权收取的权利金不是"无风险收入"，而是承担尾部风险的补偿。

# Vocabulaire

| français | 中文 | English |
|---|---|---|
| l'option d'achat (f.) | 看涨期权 | call option |
| l'option de vente (f.) | 看跌期权 | put option |
| le prix d'exercice (m.) | 行权价 | strike price |
| la prime (f.) | 权利金 | premium |
| l'échéance (f.) | 到期日 | expiry, maturity |
| le sous-jacent (m.) | 标的资产 | underlying |
| la volatilité implicite (f.) | 隐含波动率 | implied volatility |

# Related

- [[Derivative 金融衍生品 produit dérivé|衍生品]]
- [[Future 期货 contrat à terme normalisé|期货]]
- [[Forward contract 远期合同 contrat à terme|远期合同]]
- [[Hedge 对冲 couverture|对冲]]
- [[Volatility 波动率 volatilité|波动率]]
- [[Leverage 杠杆|杠杆]]
- [[Short selling 做空 vente à découvert|做空]]

# Self-check 自测

> [!question]- 证明恒等式 $(S_T-K)^+ - (K-S_T)^+ = S_T - K$，并说明它如何导出平价公式。
> 对 $S_T \ge K$，左边 $= (S_T - K) - 0$；对 $S_T < K$，左边 $= 0 - (K - S_T) = S_T - K$。故"多 call + 空 put"在 $T$ 的现金流与"持有一股 + 借入 $K e^{-rT}$"完全相同；无套利要求两者今天价格相等，即 $c - p = S_0 - K e^{-rT}$。

> [!question]- 为什么 Black–Scholes 价格与股票的预期收益 $\mu$ 无关？
> 因为期权可以由股票和无风险资产动态复制：组合 期权 $-\Delta$ 股 在每一瞬间无风险，只能赚 $r$。价格由复制成本决定，而复制成本只依赖于价格路径的波动 $\sigma$，不依赖漂移 $\mu$。

> [!question]- 上例中看涨期权买方的盈亏平衡点是多少？最大亏损是多少？
> 盈亏平衡点 $K + c = 111$ 欧元；最大亏损为权利金 6 欧元（当 $S_T \le 105$ 时）。
