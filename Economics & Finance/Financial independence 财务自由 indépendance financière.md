---
aliases:
  - financial independence
  - indépendance financière
  - fire
  - financial independence retire early
  - fi number
  - chiffre d'indépendance
  - 财务独立
summary: 资产产生的收入足以覆盖支出，工作变为可选
tags: [finance, learning]
---
# Definition

**财务自由**（financial independence, FI, *indépendance financière*）指可投资资产在可持续的[[Safe withdrawal rate 安全提取率 taux de retrait|提取率]]下产生的[[Passive income 被动收入 revenu passif|被动收入]]足以覆盖生活支出，因而工作变为可选。它是一个**不等式**而不是财富绝对值：

$$w \cdot W \ \ge\ E$$

其中 $W$ 为可投资[[Net worth 净资产 patrimoine|净资产]]，$E$ 为年支出，$w$ 为提取率。满足等号的 $W^* = E/w$ 称为**独立数字**（FI number, *chiffre d'indépendance*）。

**FIRE**（Financial Independence, Retire Early）是 2010 年代在美国兴起的运动，思想源于 Vicki Robin 与 Joe Dominguez 的 *Your Money or Your Life* (1992)，经博客 Mr. Money Mustache 等普及。核心做法是极高的储蓄率加低成本[[Index fund 指数基金 fonds indiciel|指数基金]]。变体包括 *Lean FIRE*（低支出）、*Fat FIRE*（高支出）、*Coast FIRE*（已存够、靠复利"滑行"到退休）、*Barista FIRE*（兼职补足）。

# Formula

**储蓄率决定年数**。把税后收入标准化为 1，储蓄率为 $s$，则年支出 $E = 1-s$，每年末投入 $s$。设实际收益率恒为 $r$，从零开始，$N$ 年后资产为年金终值 $s\,\frac{(1+r)^N-1}{r}$。令其等于 $W^* = (1-s)/w$：

$$N(s) = \frac{\ln\!\left(1 + \dfrac{r\,(1-s)}{s\,w}\right)}{\ln(1+r)}, \qquad N(s)\big|_{r=0} = \frac{1-s}{s\,w}$$

$N$ 只依赖于 $s, r, w$，与收入的绝对水平无关。储蓄率起**双重作用**：$s$ 越高，每年投入越多，同时目标 $(1-s)/w$ 越小。

取 $r = 5\%$，$w = 4\%$：

| 储蓄率 $s$ | 10% | 20% | 25% | 50% | 75% |
|---|---|---|---|---|---|
| 年数 $N$ | 51.4 | 36.7 | 31.9 | 16.6 | 7.1 |

模型假设：实际收益恒定（忽略[[Volatility 波动率 volatilité|波动]]与序列风险）、实际收入与支出不变、退休后支出等于工作期支出、无初始资产、无税。

# Example

书中例子（P05–P07）：目标月净收入 4 000 €，年 48 000 €。

$$W^* = \frac{48\,000}{0.04} = 120\text{ 万 €}, \qquad \frac{120\text{ 万}}{0.7} \approx 171\text{ 万 €}$$

若按作者推荐的 3%（P17-S02），税前即为 160 万 €，含税约 229 万 €。

# In the book 书中

本章第一个"成见"（*idée reçue n° 1*）就是 "**L'indépendance financière est une illusion**"。

- P03-S01 至 P03-S04：读者会联想到 "quelqu'un sirotant un cocktail sur une plage de sable fin"，并认为自由的代价 "n'est probablement pas calculable…"。
- P04-S01："Figurez-vous que si, grâce à la règle des 25 !" 作者的主张：财务自由不是幻想，而是可以计算的目标。
- P14-S01："Il est relativement simple de calculer le patrimoine dont vous aurez besoin…"
- P17-S01、P17-S02：第一项任务是计算 "chiffre d'indépendance"，并 "être conservateur en utilisant la règle des 3 %"。
- P19-S01："il faut commencer à investir le plus tôt possible, même un petit montant"；P69-S01、P69-S02："Le meilleur moment… c'était hier. Le deuxième meilleur moment, c'est aujourd'hui."

**评价**：作者成功地把模糊愿望变成一个可计算的不等式，这是有价值的。但本章只讲了目标 $W^*$，没有讲**到达目标所需的时间**，而后者主要由储蓄率决定（上式）。由上表，在 5% 实际收益、4% 提取率下，即使储蓄率达到 50% 也需约 17 年；储蓄率 10% 则需半个世纪。书中 P21–P22 的复利例子用 8% 名义收益且忽略通胀与税（P22-S04 自己承认），容易高估速度。所以"不是幻觉"在数学上成立，但在实践上的难度主要来自储蓄率，而不是投资技巧。

# Common misconceptions

- **财务自由 = 很有钱**：它是相对于个人支出而言的；支出低的人可以用较少资产实现。
- **提高收益率是最主要的杠杆**：在合理范围内，$N$ 对 $s$ 的敏感度远高于对 $r$ 的敏感度。
- **FIRE = 永不工作**：多数实践者把它理解为"工作可选"，许多人继续从事收入较低但喜欢的工作。
- **退休后支出不变**：医疗、税收、家庭变化都可能使支出上升，因此需要安全边际（P17-S02）。

# Vocabulaire

| français | 中文 | English |
|---|---|---|
| l'indépendance financière (f.) | 财务自由 | financial independence |
| une idée reçue (f.) | 成见、流行误解 | received idea, misconception |
| le chiffre d'indépendance (m.) | 独立数字 | FI number |
| le taux d'épargne (m.) | 储蓄率 | savings rate |
| les dépenses annuelles (f. pl.) | 年支出 | annual expenses |
| le train de vie (m.) | 生活水平、开销规模 | lifestyle, standard of living |
| la retraite anticipée (f.) | 提前退休 | early retirement |

# Related

- [[Safe withdrawal rate 安全提取率 taux de retrait|安全提取率]]
- [[Passive income 被动收入 revenu passif|被动收入]]
- [[Net worth 净资产 patrimoine|净资产]]
- [[Budget 预算 budget|预算]]
- [[Personal finance 个人理财 finances personnelles|个人理财]]
- [[Compound interest 复利 intérêts composés|复利]]
- [[Dollar cost averaging 平均成本法 (定投)|定投]]
- [[Index fund 指数基金 fonds indiciel|指数基金]]
- [[Investment fees 投资费用 frais|投资费用]]

# Self-check 自测

> [!question]- 年支出 30 000 €，按 3.5% 提取，独立数字是多少？
> $W^* = 30\,000 / 0.035 \approx 857\,000$ €。

> [!question]- 在 $r = 0$ 的情况下，储蓄率从 25% 提高到 50%，达到财务自由的年数如何变化？
> $N = (1-s)/(sw)$，$w=4\%$：$s=25\%$ 时 $N = 0.75/0.01 = 75$ 年；$s=50\%$ 时 $N = 0.5/0.02 = 25$ 年。储蓄率翻倍，年数降为原来的三分之一，体现了双重作用。

> [!question]- 为什么 $N(s)$ 与收入的绝对水平无关？这一结论在什么条件下失效？
> 因为投入与目标都与收入成比例，收入在 $N$ 的方程中约掉了。若支出有刚性下限（如房租）、税收为累进制、或退休后支出与工作期不同，则收入水平会重新进入方程。
