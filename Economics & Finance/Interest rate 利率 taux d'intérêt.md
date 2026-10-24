---
aliases:
  - interest rate
  - taux d'intérêt
  - rate
  - taux
summary: 借用资金的价格，以单位时间内利息占本金的比例表示
tags: [finance, learning]
---
# Definition

**利率**（interest rate, *taux d'intérêt*）是借用资金的价格：借款人在单位时间内为使用本金 $P$ 而支付的利息 $I$ 与本金之比，通常以年化百分比表示，$r = I/P$。对贷款人而言，它是放弃当前消费、承担违约风险与[[Inflation 通货膨胀 inflation|通货膨胀]]风险的补偿。

利率总是相对于某个**计息约定**而言：期限、复利频率（见[[Compound interest 复利 intérêts composés|复利]]）、计日规则（如 Act/360、Act/365）。比较两个利率之前必须先统一这些约定，例如换算成实际年利率 $\left(1+\frac{r}{n}\right)^n-1$。

# Mechanism

## 名义利率与实际利率（nominal vs real）

**名义利率** $i$（*taux nominal*）以货币单位计量收益；**实际利率** $r$（*taux réel*）以[[Purchasing power 购买力 pouvoir d'achat|购买力]]计量收益。设通胀率为 $\pi$，**Fisher 方程**（*équation de Fisher*）为

$$1+i = (1+r)(1+\pi) \quad\Longleftrightarrow\quad r = \frac{1+i}{1+\pi}-1,$$

一阶近似 $r \approx i - \pi$（误差项为 $r\pi$，在高通胀下不可忽略）。事前（ex ante）使用预期通胀 $\pi^e$，事后（ex post）使用实现的通胀。实际利率可以为负：名义利率低于通胀时，存款的购买力在下降。

## 政策利率与市场利率

- **政策利率**（policy rate, *taux directeur*）：由[[Central bank 中央银行 banque centrale|中央银行]]设定的短期利率，如欧洲央行的存款便利利率（*taux de la facilité de dépôt*）、美联储的联邦基金利率目标区间。它是[[Monetary policy 货币政策 politique monétaire|货币政策]]的主要工具。
- **市场利率**（market rates）：在货币市场与[[Bond 债券 obligation|债券]]市场上由供求决定，如银行间利率 €STR、国债收益率。短端市场利率紧跟政策利率，长端则反映对未来短期利率的预期加上**期限溢价**（term premium）。

## 收益率曲线（yield curve）

**收益率曲线**（*courbe des taux*）是同一发行人（通常是国家）不同期限零息债券收益率 $y(T)$ 关于期限 $T$ 的函数。常见形态：

- 向上倾斜（*pentue*）：长期利率高于短期，为常态；
- 平坦（*plate*）；
- 倒挂（*inversée*）：短期高于长期，常被解读为市场预期未来降息，历史上与经济衰退有一定相关性，但不是确定的预测。

# Example

某储蓄产品名义利率 $i = 3\%$，当年通胀 $\pi = 5\%$。实际利率

$$r = \frac{1.03}{1.05} - 1 \approx -1.90\%,$$

近似公式给出 $3\%-5\% = -2\%$。即 10 000 欧元存一年后账面为 10 300 欧元，但以年初价格计量只值约 $10300/1.05 \approx 9\,810$ 欧元。

# Common misconceptions

- **"利率为正就是在赚钱"**：决定购买力变化的是实际利率，而非名义利率。
- **"央行决定所有利率"**：央行直接控制的是极短期利率；长期利率由市场决定，只受政策间接影响。
- **把不同复利频率的利率直接比较**：月复利 4.9% 的实际年利率约为 5.01%，高于年复利 5%。

# Vocabulaire

| français | 中文 | English |
|---|---|---|
| *le taux d'intérêt* (m.) | 利率 | interest rate |
| *le taux directeur* (m.) | 政策利率 | policy rate |
| *le taux nominal* (m.) | 名义利率 | nominal rate |
| *le taux réel* (m.) | 实际利率 | real rate |
| *la courbe des taux* (f.) | 收益率曲线 | yield curve |
| *l'emprunteur* (m.) | 借款人 | borrower |
| *le prêteur* (m.) | 贷款人 | lender |

# Related

- [[Compound interest 复利 intérêts composés|复利]]
- [[Time value of money 货币时间价值 valeur temps de l'argent|货币时间价值]]
- [[Bond 债券 obligation|债券]]
- [[Inflation 通货膨胀 inflation|通货膨胀]]
- [[Purchasing power 购买力 pouvoir d'achat|购买力]]
- [[Central bank 中央银行 banque centrale|中央银行]]
- [[Monetary policy 货币政策 politique monétaire|货币政策]]
- [[Savings account 储蓄账户 livret d'épargne|储蓄账户]]

# Self-check 自测

> [!question]- 名义利率 6%，通胀 4%，精确的实际利率是多少？近似公式误差多大？
> $r = 1.06/1.04 - 1 \approx 1.923\%$。近似值 $2\%$，误差约 $0.077$ 个百分点，即 $r\pi \approx 0.019 \times 0.04$ 的量级（精确地，$i-\pi-r = r\pi$）。

> [!question]- 为什么倒挂的收益率曲线常被解读为降息预期？
> 在预期假说下，长期利率近似为未来各期预期短期利率的平均（加期限溢价）。若长期利率低于当前短期利率，则市场预期未来短期利率会下降，而降息通常发生在经济走弱时。

> [!question]- 政策利率与 10 年期国债收益率哪个更直接受央行控制？
> 政策利率。10 年期收益率反映对未来十年短期利率路径的预期和期限溢价，央行只能通过前瞻指引、资产购买等方式间接影响。
