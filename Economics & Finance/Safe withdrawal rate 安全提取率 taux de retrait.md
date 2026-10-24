---
aliases:
  - safe withdrawal rate
  - swr
  - withdrawal rate
  - taux de retrait
  - 4% rule
  - règle des 4 %
  - rule of 25
  - règle des 25
  - trinity study
summary: 退休后每年可从资产中提取而大概率不耗尽的比例，如 4% 法则
tags: [finance, learning]
---
# Definition

**提取率**（withdrawal rate, *taux de retrait*）是第一年从投资组合中取出的金额占初始资产的比例 $w$；此后每年的提取额按[[Inflation 通货膨胀 inflation|通胀]]调整，保持实际购买力不变。**安全提取率**（SWR）是在历史数据或模拟中，使组合在给定期限 $T$ 内"几乎不会耗尽"的最大 $w$。

**4% 法则**（*règle des 4 %*）来自两项美国研究：

- William Bengen (1994)：用 1926 年起的美国股票与中期国债数据，发现 50/50 组合下，起始提取率约 4% 时任何历史起点都能撑过至少 30 年；
- **Trinity study**（Cooley, Hubbard & Walz, 1998，得克萨斯州 Trinity University）：给出不同组合、提取率和期限下的**成功率**（*taux de succès*）表。

**25 倍法则**（*règle des 25*）是其倒数：所需资产 $= \text{年支出} / w = 25 \times \text{年支出}$（当 $w = 1/25 = 4\%$）。

# Formula

**确定性模型**。设实际收益率恒为 $r$，初始资产 $W_0$，每年末提取 $wW_0$（实际值）。则

$$W_n = W_0(1+r)^n - wW_0\frac{(1+r)^n-1}{r}$$

令 $W_N = 0$ 得资产耗尽年数：

$$N = \frac{\ln\!\big(w/(w-r)\big)}{\ln(1+r)} \quad (w > r), \qquad N = \frac{1}{w} \quad (r = 0)$$

若 $w \le r$，资产永不耗尽（永续年金）。$w = 4\%$ 时：

| 实际收益率 $r$ | 0% | 1% | 2% | 3% | ≥4% |
|---|---|---|---|---|---|
| 耗尽年数 $N$ | 25 | 28.9 | 35.0 | 46.9 | ∞ |

**序列风险**（sequence-of-returns risk）：确定性模型只依赖平均收益，但真实收益是随机序列，且有提取时**顺序很重要**。初始 100，每年初提取 5，三年收益率：

- 先好后坏 $(+25\%, +10\%, -25\%)$：期末 90.1；
- 先坏后好 $(-25\%, +10\%, +25\%)$：期末 84.8。

不提取时两者都是 $100 \times 1.25 \times 1.1 \times 0.75 = 103.1$（乘法交换律）。提取打破了交换性：早期下跌时被迫低价卖出，损失的份额无法再参与反弹。退休头几年的收益对结果影响最大。

# Example

年支出 40 000 €：

- 4% 法则：$40\,000 / 0.04 = 100$ 万 €；
- 3% 法则：$40\,000 / 0.03 \approx 133$ 万 €。

提取率从 4% 降到 3%，所需资产增加 $1/3$。这是用资产换取更长期限与更高成功率。

# In the book 书中

- P04-S02、P04-S03："il faut économiser 25 fois vos dépenses annuelles… Ensuite, vous consommerez 4 % de votre capital chaque année (100/25 = 4)."
- P06-U01 至 P07-S01：公式 *revenu passif mensuel × 12 / 4 %*；4 000 €/月 → 120 万 €，再除以 0.7（30% *flat tax*）→ 170 万 €。
- P07-S03："Je peux être **quasi certain** de ne jamais épuiser ce dernier."
- P08-S01 至 P12-S04：Trinity study，模拟五种股债组合（P09），使用 1929–1995 年历史数据并考虑通胀（P11）。"un portefeuille 50 % actions et 50 % obligations a une probabilité de 100 % de suffire à couvrir 25 ans de dépenses"（P12-S01）；30 年降至 95%（P12-S03）；要保持 100% 需降到 3%（P12-S04）。
- P14-S02、P17-S02：作者建议保守地使用 3% 并加安全边际。

**评价**：

1. **P07-S03 夸大了结论**。Trinity 的"成功"是在 $T$ 年内不耗尽，而不是"永不耗尽"；书中自己的表格也显示 30 年成功率仅 95%。对 40–50 年的提前退休，4% 偏激进，作者在 P17-S02 推荐 3% 是更一致的做法。
2. **P12-S02 混淆了两个 25**："Ces fameux 25 ans qui expliquent la règle des 25"。25 倍来自 $1/0.04$，与 25 年期限并无因果关系；唯一的联系是上表中 $r=0$ 时恰好 $N = 1/w = 25$。
3. **美国样本偏差**：20 世纪美国市场表现在全球名列前茅（幸存者偏差）。多国数据研究（如 Wade Pfau, 2010）发现许多国家的历史安全提取率低于 4%。原论文数据起点一般记为 1926 年，书中写 1929。
4. **未计费用与税**：研究使用指数收益。每年 1% 的[[Investment fees 投资费用 frais|费用]]大致相当于把 $r$ 降低 1 个百分点，对应上表左移一列。
5. **税的处理偏保守**：P07-S01 把全部提取额按 30% 计税，但出售资产时只有利得部分（*plus-value*）征税，本金部分不征税。

# Common misconceptions

- **4% 是每年剩余资产的 4%**：不是。是初始资产的 4%，之后按通胀调整；按当前资产比例提取是另一种（永不耗尽但收入波动的）规则。
- **成功率 95% = 5% 的情况略有不足**：失败意味着资产在期限内归零。
- **4% 适用于任何期限**：期限越长，安全提取率越低。
- **平均收益足够就安全**：序列风险说明，同样的平均收益可产生不同结果。

# Vocabulaire

| français | 中文 | English |
|---|---|---|
| le taux de retrait (m.) | 提取率 | withdrawal rate |
| le taux de succès (m.) | 成功率 | success rate |
| la règle des 25 (f.) | 25 倍法则 | rule of 25 |
| épuiser son capital | 耗尽本金 | to deplete one's capital |
| un portefeuille (m.) | 投资组合 | portfolio |
| une obligation (f.) | 债券 | bond |
| conservateur, -trice (adj.) | 保守的 | conservative |
| une marge de sécurité (f.) | 安全边际 | safety margin |

# Related

- [[Financial independence 财务自由 indépendance financière|财务自由]]
- [[Passive income 被动收入 revenu passif|被动收入]]
- [[Asset allocation 资产配置 allocation d'actifs|资产配置]]
- [[Volatility 波动率 volatilité|波动率]]
- [[Return 收益率 rendement|收益率]]
- [[Time value of money 货币时间价值 valeur temps de l'argent|货币时间价值]]（年金公式）
- [[Inflation 通货膨胀 inflation|通胀]]
- [[Investment fees 投资费用 frais|投资费用]]
- [[Compound interest 复利 intérêts composés|复利]]

# Self-check 自测

> [!question]- 实际收益率恒为 2%，按 5% 提取，资产能维持多少年？
> $N = \ln(0.05/0.03)/\ln(1.02) = \ln(5/3)/\ln 1.02 \approx 0.511/0.0198 \approx 25.8$ 年。

> [!question]- 为什么提款会让收益顺序变得重要，而纯持有时不会？
> 纯持有时 $W_T = W_0\prod(1+g_t)$，乘积与顺序无关。有提款时 $W_T$ 中每笔提款只乘以其之后的增长因子，早期的低收益作用于更大比例的资产且迫使低价卖出，因此先跌后涨的结果更差。

> [!question]- P12-S02 说 25 年期限"解释了"25 倍法则，这个说法对吗？
> 不对。25 倍是 $1/4\%$ 的代数结果。只有在实际收益率为 0 时，25 倍资产按 4% 提取才恰好维持 25 年；正收益时会更久。作者把两个数字的巧合当成了解释。
