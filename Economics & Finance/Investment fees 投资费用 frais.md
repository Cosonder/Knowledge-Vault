---
aliases:
  - investment fees
  - fees
  - frais
  - frais de gestion
  - frais d'entrée
  - ter
  - total expense ratio
  - commission
  - fee drag
summary: 管理费、申购费、佣金等投资成本及其复利侵蚀
tags: [finance, learning]
---
# Definition

**投资费用**（investment fees, *frais*）是投资者为购买、持有和卖出金融产品向中介支付的全部成本。主要类型：

- **管理费 / 总费用率**（management fee, TER = total expense ratio, *frais de gestion*, *frais courants*）：按资产规模每年收取的比例，从[[Fund 基金|基金]]净值中直接扣除，投资者不会收到账单；
- **申购费 / 入场费**（entry fee, *frais d'entrée* / *droits d'entrée*）：买入时一次性扣除，赎回时还可能有 *frais de sortie*；
- **交易佣金**（brokerage commission, *frais de courtage*）：每笔买卖支付给券商；
- **账户费**（*droits de garde*, *frais de tenue de compte*）：托管或账户维护费用；
- **业绩报酬**（*commission de surperformance*）：超过基准时提取的分成，常见于[[Hedge fund 对冲基金 gestion alternative|对冲基金]]。

**顾问的收费模式**决定了利益冲突：

- **佣金制**（*rémunéré à la commission*）：顾问的报酬来自其推荐产品的申购费和管理费分成（*rétrocessions*）。咨询看似免费，实则通过产品费用支付，顾问有动机推荐费用高的产品；
- **收费制**（*rémunéré en honoraires*, fee-only）：客户直接支付咨询费，顾问不从产品中获利，利益冲突较小。

# Formula

**费用拖累**（fee drag）。总收益率 $r$，年费率 $f$，期限 $T$。近似地，净收益率为 $r - f$，则期末财富之比为

$$\frac{(1+r-f)^T}{(1+r)^T} = \left(1 - \frac{f}{1+r}\right)^T \approx e^{-fT/(1+r)}$$

费用损失 $1 - (1-\tfrac{f}{1+r})^T$ 随 $T$ 增长并趋近 1（剩余财富比例随 $T$ 指数衰减）；对小 $f$，损失约为 $fT$ 的量级，而不是 $f$。一次性入场费 $e$ 则只是乘以常数 $(1-e)$，不随时间复合，因此长期而言经常性费用远比一次性费用重要。

# Example

初始 10 000 €，总收益率 7%，30 年：

| 年费率 $f$ | 期末财富 | 相对无费用的损失 |
|---|---|---|
| 0% | $10\,000 \times 1.07^{30} \approx 76\,123$ € | — |
| 0.2%（典型[[Index fund 指数基金 fonds indiciel\|指数]] [[ETF 交易所交易基金 fonds négocié en bourse\|ETF]]） | $\approx 72\,000$ € | 约 5.5% |
| 1% | $10\,000 \times 1.06^{30} \approx 57\,435$ € | 24.5% |
| 2% | $10\,000 \times 1.05^{30} \approx 43\,219$ € | 43.2% |

对比：3% 的一次性入场费只造成 3% 的损失。

# In the book 书中

本章"成见 3"（*Je dois déléguer la gestion de mon argent*）集中讨论费用和顾问的激励：

- P26-S03 至 P27-S02："le conseil est gratuit ! Mais si c'est gratuit, c'est vous le produit. Sa rémunération dépend des commissions qu'il va générer." 作者主张：免费咨询的成本隐藏在产品费用里。
- P27-S03："des frais qui vont être **ponctionnés** au moment de l'investissement ou sur la durée de vie du produit"——即入场费与持续管理费两类。
- P27-S05："On est plus proche d'un vendeur que d'un conseiller."
- P28-S01、P28-S02："Les frais sont un poison pour votre patrimoine. Si vous payez 2 % de frais par an, votre manque à gagner au bout de 30 ans s'élèvera à 43 % !" 上表验证：该数字与 7% 总收益的假设一致。
- P30-S01 至 P30-S05：95% 的 CGP 靠产品佣金获得收入；只有不足 5% 的 CGPI "au conseil indépendant" 收取 *honoraires*，无利益冲突。
- P32-U01 至 P34-S01：客户 1 由 "un CGP rémunéré à la commission" 服务，年表现低 1.7%；40 年后客户 2 多 84%，初始 10 万 € 加每年 1 200 € 时多约 75 万 €。验算：设总收益 $r$，客户 1 的净收益 $r - 1.7\%$，按"初始 10 万 € + 每年末 1 200 €"计算终值之比。$r = 6\%$ 或 $7\%$ 时比值均约 1.84，差额分别约 55 万 € 与 79 万 €，与书中 84% 和 75 万 € 一致（对应 $r$ 约 6.8%）。单看一次性本金，$(1.07/1.053)^{40} \approx 1.90$。
- P66-S02、P66-S03：减税型房地产佣金 "s'élèvent en moyenne à 5 % dès la signature"，25 万 € 项目即 12 500 €。P68-S02：顾问不推荐低费用产品，"car ils ne seront pas commissionnés dessus"。

**评价**：费用复利的数学是正确的，而且是投资中少数确定的事情：未来收益不确定，费用却是确定的。但"−1.7%"是一个平均估计，具体取决于产品；收费制顾问的 *honoraires* 本身也是成本，比较时需计入。作者是 Finary 的创办人（P35-S01），其产品同样收费，读者可以用同样的批判标准审视。

# Common misconceptions

- **1% 很少**：1% 是每年对全部资产收取，在 7% 收益下相当于吃掉约七分之一的收益，30 年后损失约四分之一财富。
- **免费咨询**：没有直接账单不等于没有成本。
- **高费用 = 更好的管理**：大量研究表明主动管理基金扣费后平均跑输指数，见[[Efficient market hypothesis 有效市场假说 hypothèse des marchés efficients|有效市场假说]]。
- **只看入场费**：长期而言经常性费用更重要。

# Vocabulaire

| français | 中文 | English |
|---|---|---|
| les frais (m. pl.) | 费用 | fees |
| les frais de gestion (m. pl.) | 管理费 | management fees |
| les frais d'entrée (m. pl.) | 申购费、入场费 | entry fees |
| une commission (f.) | 佣金 | commission |
| les honoraires (m. pl.) | 专业服务费 | fees (for professional services) |
| un conflit d'intérêts (m.) | 利益冲突 | conflict of interest |
| le manque à gagner (m.) | 少赚的部分、机会损失 | shortfall, lost earnings |
| ponctionner (v.) | 抽取、扣除 | to levy, to skim off |

# Related

- [[Compound interest 复利 intérêts composés|复利]]
- [[Return 收益率 rendement|收益率]]
- [[Index fund 指数基金 fonds indiciel|指数基金]]
- [[ETF 交易所交易基金 fonds négocié en bourse|ETF]]
- [[Mutual fund 共同基金 fonds commun de placement|共同基金]]
- [[Investment fund 证券投资基金 fonds d'investissement|证券投资基金]]
- [[Safe withdrawal rate 安全提取率 taux de retrait|安全提取率]]（费用降低可持续提取率）
- [[Efficient market hypothesis 有效市场假说 hypothèse des marchés efficients|有效市场假说]]
- [[Personal finance 个人理财 finances personnelles|个人理财]]

# Self-check 自测

> [!question]- 总收益 6%，年费 1.5%，40 年后财富是无费用情形的多少？
> $(1.045/1.06)^{40} = (0.98585)^{40} \approx e^{40 \times (-0.01425)} \approx e^{-0.570} \approx 0.57$，即损失约 43%。

> [!question]- 为什么长期投资中，1% 的年费比 5% 的一次性入场费损害更大？
> 入场费只乘一次常数 $0.95$；年费每年复合，$T$ 年后损失约 $1-(1-\tfrac{f}{1+r})^T$。$r=7\%$、$T=30$ 时 1% 年费的损失约 24.5%，远超 5%。只有持有期很短时一次性费用才更重要。

> [!question]- 佣金制顾问的利益冲突具体体现在哪里？
> 其收入来自所推荐产品的费用（P27-S02、P30-S01），因此有动机推荐费用高、佣金高的产品（如 P66 的减税房产），而不推荐低费用的指数基金（P68-S02）。收费制顾问的收入与产品选择无关，冲突较小。
