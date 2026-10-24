---
aliases:
  - monetary policy
  - politique monétaire
  - qe
  - quantitative easing
  - assouplissement quantitatif
summary: 央行通过利率和货币供给调节经济、稳定物价的政策
tags: [finance, learning]
---
# Definition

**货币政策**（monetary policy, *politique monétaire*）是[[Central bank 中央银行 banque centrale|中央银行]]通过调节短期[[Interest rate 利率 taux d'intérêt|利率]]、准备金和资产负债表规模，影响信贷条件、总需求，进而实现物价稳定（及就业等）目标的政策。**宽松**（expansionary, *accommodante*）指降息、扩表；**紧缩**（contractionary, *restrictive*）指加息、缩表。它区别于由政府实施的**财政政策**（fiscal policy）。

# Instruments

**1. 政策利率**（policy rate, *taux directeur*）。央行设定其向银行借贷或为准备金付息的利率，如 ECB 的存款便利利率、Fed 的联邦基金利率目标区间、人民银行的 7 天逆回购利率。在准备金充裕的体系中，央行通过"利率走廊"（corridor）把隔夜市场利率夹在贷款便利利率与存款便利利率之间。

**2. 公开市场操作**（open market operations, *opérations d'open market*）。央行买卖证券或进行回购（repo），增减银行准备金。买入资产 → 准备金增加 → 短期利率下行。

**3. 存款准备金率**（reserve requirement ratio, *taux de réserves obligatoires*）。银行须按存款的一定比例 $\rho$ 存放于央行。教科书的货币乘数为 $m = 1/\rho$，但现代实践中银行先放贷后获取准备金，乘数模型只是粗略近似。ECB 准备金率仅 1%，Fed 自 2020 年起为 0；人民银行仍把准备金率作为常用工具。

**4. 量化宽松**（quantitative easing, QE, *assouplissement quantitatif*）。当政策利率接近零下限（zero lower bound）时，央行大规模购买长期国债乃至公司债，压低长期利率和期限溢价，并向市场发出"长期维持低利率"的信号。反向操作称为量化紧缩（QT）。

**5. 前瞻指引**（forward guidance）：公开承诺未来利率路径，影响预期。

# Inflation targeting

**通胀目标制**（inflation targeting, *ciblage d'inflation*）：央行公开承诺一个数值目标（ECB、Fed 均为 2%），以此锚定通胀预期。常用的描述性规则是 **Taylor 规则**（1993）：

$$i_t = r^* + \pi_t + 0.5\,(\pi_t - \pi^*) + 0.5\,(y_t - y_t^*),$$

其中 $i_t$ 为名义政策利率，$r^*$ 为中性实际利率，$\pi_t$ 为通胀，$\pi^*$ 为目标，$y_t - y_t^*$ 为产出缺口。"Taylor 原则"要求通胀上升 1 点时名义利率上升超过 1 点，使实际利率 $i - \pi$ 上升，从而抑制需求。

# Transmission to asset prices

利率变化通过几个渠道传导：

- **折现率渠道**：资产价格是未来现金流的折现，$P = \sum_t \frac{CF_t}{(1+r)^t}$，$r$ 下降则 $P$ 上升，久期越长越敏感（成长股、长期[[Bond 债券 obligation|债券]]）；见[[Time value of money 货币时间价值 valeur temps de l'argent|货币时间价值]]。
- **信贷渠道**：贷款利率和银行放贷意愿变化，影响房地产与企业投资；
- **汇率渠道**：降息使本币贬值，提振出口与进口价格；
- **风险承担渠道**：低利率促使投资者追逐收益（search for yield），压缩风险溢价；
- **预期渠道**：影响通胀预期和长期利率。

# Example

设 $r^* = 1\%$，$\pi^* = 2\%$，当前通胀 $\pi = 5\%$，产出缺口为 0。Taylor 规则建议

$$i = 1\% + 5\% + 0.5\times 3\% + 0 = 7.5\%.$$

再看折现率渠道：一张 10 年期零息债券面值 100，收益率从 2% 升至 4%，价格从 $100/1.02^{10} \approx 82.0$ 跌至 $100/1.04^{10} \approx 67.6$，下跌约 18%。这解释了 2022 年加息周期中长期债券的大幅亏损。

# Common misconceptions

- "央行直接控制所有利率。"央行主要控制隔夜利率，长期利率还取决于预期和期限溢价。
- "QE 就是印钞，必然导致恶性通胀。"QE 增加的是银行准备金而非直接增加流通现金；2009–2020 年欧美大规模 QE 期间通胀长期低于目标。
- "降息一定推高股价。"若降息是因为经济衰退预期，盈利下修可能抵消折现率下降的影响。

# Vocabulaire

| français | 中文 | English |
|---|---|---|
| la politique monétaire (f.) | 货币政策 | monetary policy |
| le taux directeur (m.) | 政策利率 | policy rate |
| l'assouplissement quantitatif (m.) | 量化宽松 | quantitative easing |
| le ciblage d'inflation (m.) | 通胀目标制 | inflation targeting |
| la masse monétaire (f.) | 货币供应量 | money supply |
| le resserrement monétaire (m.) | 货币紧缩 | monetary tightening |
| les anticipations (f. pl.) | 预期 | expectations |

# Related

- [[Central bank 中央银行 banque centrale|中央银行]]
- [[Interest rate 利率 taux d'intérêt|利率]]
- [[Inflation 通货膨胀 inflation|通胀]]
- [[Bond 债券 obligation|债券]]
- [[Purchasing power 购买力 pouvoir d'achat|购买力]]
- [[Time value of money 货币时间价值 valeur temps de l'argent|货币时间价值]]
- [[Savings account 储蓄账户 livret d'épargne|储蓄账户]]

# Self-check 自测

> [!question]- 什么是 Taylor 原则？为什么系数必须大于 1？
> 通胀每上升 1 个百分点，名义利率应上升超过 1 个百分点。只有这样实际利率 $i - \pi$ 才会上升，抑制需求、使通胀回落；若系数小于 1，通胀上升反而使实际利率下降，加剧通胀。

> [!question]- 为什么长期债券和成长股对利率更敏感？
> 它们的现金流集中在远期，折现因子 $(1+r)^{-t}$ 对 $r$ 的敏感度随 $t$ 增大：$\partial \ln P / \partial r \approx -t/(1+r)$。久期越长，利率变动造成的价格变化越大。

> [!question]- 零利率下限时，央行还有哪些工具？
> 量化宽松（购买长期资产）、前瞻指引、负利率（ECB 2014–2022 年曾设负存款利率）、定向长期再融资操作（TLTRO）等。
