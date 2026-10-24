---
aliases:
  - purchasing power
  - pouvoir d'achat
  - real value
  - valeur réelle
summary: 一定数量货币能购买的商品与服务的数量，随通胀下降
tags: [finance, learning]
---
# Definition

**购买力**（purchasing power, *pouvoir d'achat*）是一定数量的货币所能购买的商品和服务的数量。它是货币的**实际价值**（real value, *valeur réelle*），与票面上的**名义价值**（nominal value, *valeur nominale*）相对。

购买力与价格水平成反比。[[Inflation 通货膨胀 inflation|通货膨胀]]即价格总水平的持续上升，意味着每单位货币的购买力持续下降。价格水平通常用消费者价格指数（CPI；法国为 INSEE 发布的 *indice des prix à la consommation*, IPC）衡量。

注意：宏观经济学中"家庭购买力"（*le pouvoir d'achat des ménages*）指实际可支配收入，即收入增长与价格增长之差，与本页讨论的"一单位货币的购买力"相关但不同。

# Formula

设年通胀率 $\pi$（假设恒定），名义金额 $N$ 在 $t$ 年后的实际价值（以今日价格计）为

$$V_{\text{real}} = \frac{N}{(1+\pi)^t}.$$

若通胀率逐年变化，则 $V_{\text{real}} = N\big/\prod_{k=1}^{t}(1+\pi_k) = N\cdot\dfrac{\text{CPI}_0}{\text{CPI}_t}$。

一笔以名义利率 $i$ 生息的资金，实际价值演化为

$$V_t = N_0\left(\frac{1+i}{1+\pi}\right)^t = N_0\,(1+r)^t,$$

其中 $r$ 是 [[Interest rate 利率 taux d'intérêt|Fisher 方程]] 中的实际利率。购买力不下降当且仅当 $i \ge \pi$（税后、扣费后）。

购买力减半所需时间：$t_{1/2} = \ln 2/\ln(1+\pi) \approx 72/(100\pi)$，与[[Compound interest 复利 intérêts composés|复利]]的 72 法则同构。

# Mechanism

**为什么现金与储蓄账户会损失购买力**：

1. **现金**（纸币、活期账户）名义利率 $i = 0$，因此实际收益 $r = -\pi/(1+\pi) < 0$（当 $\pi>0$）。只要通胀为正，购买力必然逐年下降。
2. **[[Savings account 储蓄账户 livret d'épargne|储蓄账户]]**（如法国 *Livret A*）的名义利率通常与短期利率挂钩，长期平均往往接近甚至低于通胀率，扣税后（视产品而定）实际收益在零附近或为负。
3. 由于 $V_t$ 是指数形式，即使年度差距 $i-\pi$ 只有 $-1\%$，数十年后的累积损失也很显著。

能否跑赢通胀取决于资产的实际[[Return 收益率 rendement|收益率]]。历史上分散化的股票组合长期实际收益为正，但伴随较高[[Volatility 波动率 volatilité|波动率]]；通胀挂钩债券（法国 *OATi / OAT€i*）直接按物价指数调整本金。这里不构成任何配置建议。

# Example

今天的 10 000 欧元，若年通胀 2.5%：

- 10 年后实际价值 $10000/1.025^{10}\approx 7\,812$ 欧元；
- 30 年后 $10000/1.025^{30}\approx 4\,767$ 欧元，购买力不足一半；
- 购买力减半时间 $\ln2/\ln1.025\approx 28.1$ 年。

若这笔钱放在名义年利率 1.5% 的账户中，30 年后的实际价值为 $10000\times(1.015/1.025)^{30}\approx 7\,452$ 欧元，账面上却显示 $10000\times1.015^{30}\approx 15\,631$ 欧元。

# Common misconceptions

- **货币幻觉**（money illusion, *illusion monétaire*）：以名义数额判断财富变化，忽视价格水平。账户余额增长不等于变富。
- **"现金零风险"**：现金名义上无波动，但在正通胀下有确定的实际损失。
- **"通胀率 2% 就几乎没影响"**：在 35 年的时间尺度上，2% 通胀使购买力下降一半。

# Vocabulaire

| français | 中文 | English |
|---|---|---|
| *le pouvoir d'achat* (m.) | 购买力 | purchasing power |
| *la valeur réelle* (f.) | 实际价值 | real value |
| *la hausse des prix* (f.) | 物价上涨 | price increase |
| *l'indice des prix à la consommation* (m.) | 消费者价格指数 | consumer price index |
| *l'érosion monétaire* (f.) | 货币贬值侵蚀 | monetary erosion |
| *l'épargne* (f.) | 储蓄 | savings |
| *l'illusion monétaire* (f.) | 货币幻觉 | money illusion |

# Related

- [[Inflation 通货膨胀 inflation|通货膨胀]]
- [[Interest rate 利率 taux d'intérêt|利率]]
- [[Compound interest 复利 intérêts composés|复利]]
- [[Return 收益率 rendement|收益率]]
- [[Savings account 储蓄账户 livret d'épargne|储蓄账户]]
- [[Currency 通货 monnaie|通货]]
- [[Time value of money 货币时间价值 valeur temps de l'argent|货币时间价值]]
- [[Net worth 净资产 patrimoine|净资产]]

# Self-check 自测

> [!question]- 通胀 3%，现金每年损失多少购买力？是 3% 吗？
> 不完全是。实际价值变为 $1/1.03\approx0.9709$，即每年损失约 $2.91\%$。$3\%$ 是物价的上涨率，购买力的下降率是 $\pi/(1+\pi)$。

> [!question]- 储蓄利率 3%，通胀 2%，利息税率 30%，实际税后收益是多少？
> 税后名义利率 $3\%\times0.7 = 2.1\%$，实际收益 $1.021/1.02 - 1 \approx 0.10\%$，几乎为零。

> [!question]- 已知 $\text{CPI}_{2015}=100$，$\text{CPI}_{2025}=125$，2015 年的 1 000 欧元相当于 2025 年多少欧元？
> $1000\times125/100 = 1250$ 欧元。反之，2025 年的 1 000 欧元以 2015 年价格计只值 800 欧元。
