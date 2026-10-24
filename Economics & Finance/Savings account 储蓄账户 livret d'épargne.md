---
aliases:
  - savings account
  - livret d'épargne
  - livret
  - livrets réglementés
  - livret a
  - ldds
  - lep
  - épargne de précaution
  - 存款
summary: 本金安全、随时可取的储蓄账户；法国 Livret A 等受管制储蓄
tags: [finance, learning]
---
# Definition

**储蓄账户**（savings account, *livret d'épargne*）是银行提供的计息存款账户：名义本金不会减少，可以随时存取，利率通常低于长期风险资产的预期[[Return 收益率 rendement|收益率]]。

法国的储蓄账户分两类：

- **受管制储蓄账户**（*livrets réglementés*）：利率、存款上限和税收待遇由国家规定，各银行完全相同；
- **普通银行储蓄账户**（*livrets bancaires*, *super livrets*）：利率由银行自定，利息需按资本所得纳税。

主要的 *livrets réglementés*：

| 账户 | 适用对象 | 利率 | 上限（量级） | 税 |
|---|---|---|---|---|
| **Livret A** | 所有人，每人一个 | 国家规定 | 约 2.3 万 € | 免税 |
| **LDDS**（*livret de développement durable et solidaire*） | 成年纳税居民 | 与 Livret A 相同 | 约 1.2 万 € | 免税 |
| **LEP**（*livret d'épargne populaire*） | 收入低于门槛的家庭 | 高于 Livret A | 约 1 万 € | 免税 |

利率按公式计算（参考通胀与短期[[Interest rate 利率 taux d'intérêt|利率]]），由 Banque de France 提议、经济部决定，通常每年 2 月 1 日和 8 月 1 日调整，因此具体数值需查当期公告。Livret A 和 LDDS 的部分资金集中到 *Caisse des dépôts* 用于资助社会住房。

**与中国比较**：中国的**活期存款**（demand deposit）随时可取，利率极低；**定期存款**（time deposit）锁定期限换取较高利率，提前支取通常按活期计息。两国存款利率都与[[Central bank 中央银行 banque centrale|央行]]的[[Monetary policy 货币政策 politique monétaire|货币政策]]相关，但中国没有类似 Livret A 的全国统一、免税、限额的受管制产品。安全保障上，中国《存款保险条例》对每人每家银行最高赔付 50 万元；法国普通存款由 FGDR 保障每人每家银行 10 万 €，而 Livret A、LDDS、LEP 另有国家担保。

# Mechanism

储蓄账户保证的是**名义本金**，不保证**实际购买力**。按 Fisher 关系，名义利率 $i$、通胀率 $\pi$ 时实际收益率为

$$1 + r_{\text{real}} = \frac{1+i}{1+\pi}, \qquad r_{\text{real}} \approx i - \pi$$

若 $i < \pi$，账户余额上升的同时[[Purchasing power 购买力 pouvoir d'achat|购买力]]下降。

# Example

书中 P45–P46 的例子：10 000 €，$i = 1.5\%$，10 年。

- 名义：$10\,000 \times 1.015^{10} \approx 11\,605$ €；
- 设 $\pi = 2.5\%$，精确实际值：$10\,000 \times (1.015/1.025)^{10} \approx 9\,066$ €；
- 用近似 $r_{\text{real}} = -1\%$：$10\,000 \times 0.99^{10} \approx 9\,044$ €（书中 9 043 €）。

书中用的是近似式，误差约 20 €，不影响结论。

# In the book 书中

本章"成见 5"是 "**Les livrets sont plus sûrs que la Bourse**"。

- P41-U01 至 P41-S03："400 000 000 000 €… C'est le montant de l'**encours** de notre cher livret A."
- P42-S01："Ce livret, dont le taux s'élève à 1,5 % (au 1er février 2026), est le placement préféré des Français."
- P43-U01：受欢迎的原因 "montant garanti par l'État ; intérêts nets d'impôts ; plafond généreux"。
- P44-S01、P44-S02："Non, le livret A n'est pas un bon investissement. Pire, c'est un investissement catastrophique : vous avez une probabilité de 100 % de perdre en pouvoir d'achat…"
- P44-S06："Tous les investissements qui rapportent moins que l'inflation engendrent une baisse mécanique de votre pouvoir d'achat."
- P47-S01："Vous ne verrez pas cette perte… en consultant le **solde** de votre livret A, mais elle est bien réelle."
- P48-S01、P48-S02："Ne clôturez pas votre livret A tout de suite ! Il aura un rôle important dans votre patrimoine."

**评价**：

1. 作者区分了两种"安全"：**名义本金安全**（livret 确实优于股市）与**购买力安全**（长期看 livret 往往不如股市）。这个区分是本节的核心，也是正确的。
2. "probabilité de 100 %" 过强。P44-S06 的论断是条件命题：只有当 $i < \pi$ 时才成立。Livret A 的利率公式部分挂钩通胀，历史上实际利率有正有负；在通胀低于利率的时期，实际收益为正。
3. 比较 livret 与股市时应考虑**期限**。短期（如一两年内要用的钱）股市名义亏损的概率不低，livret 更合适；长期则股市的预期实际收益更高。P48 所说的"重要角色"即应急储备（*épargne de précaution*）：流动性和名义稳定性才是 livret 的功能，而不是收益。

# Common misconceptions

- **余额增加 = 变富**：需要扣除通胀（P47-S01）。
- **livret 无风险**：没有名义风险，但有通胀风险和机会成本。
- **股市"更安全"**：作者并没有这样说；股市的优势仅在长期预期实际收益，短期波动远大于 livret。
- **所有 livret 都免税**：只有受管制账户免税；*livrets bancaires* 的利息需纳税。

# Vocabulaire

| français | 中文 | English |
|---|---|---|
| un livret d'épargne (m.) | 储蓄账户 | savings account |
| les livrets réglementés (m. pl.) | 受管制储蓄账户 | regulated savings accounts |
| le plafond (m.) | 存款上限 | deposit ceiling |
| l'encours (m.) | 存续余额总额 | outstanding amount |
| le solde (m.) | 账户余额 | account balance |
| l'épargne de précaution (f.) | 应急储蓄 | emergency fund |
| le pouvoir d'achat (m.) | 购买力 | purchasing power |
| clôturer un compte | 注销账户 | to close an account |

# Related

- [[Inflation 通货膨胀 inflation|通胀]]
- [[Purchasing power 购买力 pouvoir d'achat|购买力]]
- [[Interest rate 利率 taux d'intérêt|利率]]
- [[Compound interest 复利 intérêts composés|复利]]
- [[Central bank 中央银行 banque centrale|中央银行]]
- [[Monetary policy 货币政策 politique monétaire|货币政策]]
- [[Asset allocation 资产配置 allocation d'actifs|资产配置]]
- [[Volatility 波动率 volatilité|波动率]]
- [[Budget 预算 budget|预算]]
- [[Personal finance 个人理财 finances personnelles|个人理财]]

# Self-check 自测

> [!question]- 存款利率 3%，通胀 2%，实际收益率精确值是多少？用近似式误差多大？
> $1.03/1.02 - 1 \approx 0.980\%$；近似式给出 1%，误差约 0.02 个百分点。利率和通胀越高，误差越大。

> [!question]- P44-S02 说存在 Livret A 上"100% 的概率"损失购买力，这个说法在什么条件下成立？
> 仅当整个持有期内名义利率低于通胀率时成立（P44-S06 正是这一条件形式）。若利率高于通胀，实际收益为正。这是一个经验判断，而不是数学必然。

> [!question]- 既然 Livret A 长期会损失购买力，为什么作者说不要注销它（P48）？
> 因为它的功能是应急储备：本金名义稳定、随时可取、免税、有国家担保。一笔可能在短期内要用的钱放在股市里，可能需要在下跌时卖出。作者反对的是把长期资产放在 livret 上，而不是 livret 本身。
