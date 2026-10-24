---
aliases:
  - bond
  - obligation
  - fixed income
  - ytm
  - yield to maturity
summary: 发行人借款并承诺按期付息、到期还本的债务证券
tags: [finance, learning]
---
# Definition

**债券**（bond, *obligation*）是一种债务证券：发行人（国家、地方政府、企业）向投资者借款，承诺在约定日期支付利息并在到期日偿还本金。持有人是**债权人**（*créancier*），而[[Stock 股票 action|股票]]持有人是所有者；破产清算时债权人优先于股东受偿。

基本要素：

- **面值**（face value / par, *valeur nominale*）$F$：到期偿还的金额；
- **票面利率**（coupon rate, *taux du coupon*）$c$：每期**票息**（coupon）$C = cF$（按年或半年支付）；
- **到期日**（maturity, *échéance*）$T$；
- **价格**（price）$P$：在[[Secondary market 二级市场 marché secondaire|二级市场]]上的成交价，常以面值的百分比报价。

# Formula

## 价格与到期收益率

年付息债券（剩余 $n$ 期）在收益率 $y$ 下的价格为未来现金流的[[Time value of money 货币时间价值 valeur temps de l'argent|现值]]：

$$P(y) = \sum_{k=1}^{n}\frac{C}{(1+y)^k} + \frac{F}{(1+y)^n} = \frac{C}{y}\left[1-(1+y)^{-n}\right] + F(1+y)^{-n}.$$

**到期收益率**（yield to maturity, YTM, *taux de rendement actuariel*）是使上式等于市场价格的 $y$，即债券的内部收益率。它假设持有至到期、无违约、票息以 $y$ 再投资。

## 价格–收益率反向关系

$P(y)$ 是 $y$ 的严格递减凸函数（$P'<0$，$P''>0$）。因此：

- 市场利率上升 $\Rightarrow$ 已发行债券价格下跌；
- $y = c$ 时平价（$P = F$）；$y > c$ 时折价；$y < c$ 时溢价。

## 久期（duration）

**Macaulay 久期**是现金流时点按现值加权的平均：

$$D = \frac{1}{P}\sum_{k=1}^{n} k\,\frac{CF_k}{(1+y)^k}.$$

**修正久期** $D^* = D/(1+y)$ 给出一阶敏感度：

$$\frac{\Delta P}{P} \approx -D^*\,\Delta y.$$

二阶修正由**凸性**（convexity）给出：$\frac{\Delta P}{P}\approx -D^*\Delta y + \tfrac12\,\mathcal{C}\,(\Delta y)^2$。零息债券的 Macaulay 久期等于其期限。

## 信用风险

**信用风险**（credit risk, *risque de crédit*）是发行人违约或评级下调的风险。投资者为此要求**信用利差**（credit spread, *spread de crédit*）：$y_{\text{corporate}} = y_{\text{government}} + s$。

- **国债**（government bonds, 法国称 *OAT*）：以本币发行时通常被视为信用风险最低，作为无风险利率的近似；
- **公司债**（corporate bonds）：分为投资级（investment grade，BBB−及以上）与高收益/投机级（high yield）。

# Example

面值 1 000 欧元、票面利率 3%、剩余 5 年、年付息。若市场收益率 $y = 3\%$，$P = 1000$。若收益率升至 $4\%$：

$$P = \frac{30}{0.04}\left[1-1.04^{-5}\right] + 1000\times 1.04^{-5} \approx 133.55 + 821.93 = 955.48.$$

价格下跌约 4.45%。该债券在 $y=3\%$ 时 Macaulay 久期约 4.72 年，修正久期约 4.58，久期近似给出 $-4.58\times1\% = -4.58\%$，与实际的 $-4.45\%$ 之差由凸性解释。

# Common misconceptions

- **"债券没有风险"**：持有到期且不违约时名义回报确定，但中途卖出面临利率风险，且名义回报仍受[[Inflation 通货膨胀 inflation|通货膨胀]]侵蚀。
- **"高票息 = 高收益"**：决定回报的是买入价对应的 YTM，而非票面利率。
- **混淆当期收益率与 YTM**：当期收益率 $C/P$ 忽略了价格向面值的回归。

# Vocabulaire

| français | 中文 | English |
|---|---|---|
| *l'obligation* (f.) | 债券 | bond |
| *la valeur nominale* (f.) | 面值 | face value |
| *le coupon* (m.) | 票息 | coupon |
| *l'échéance* (f.) | 到期日 | maturity |
| *le taux de rendement actuariel* (m.) | 到期收益率 | yield to maturity |
| *l'émetteur* (m.) | 发行人 | issuer |
| *la duration* (f.) | 久期 | duration |
| *l'emprunt d'État* (m.) | 国债 | government bond |

# Related

- [[Interest rate 利率 taux d'intérêt|利率]]
- [[Time value of money 货币时间价值 valeur temps de l'argent|货币时间价值]]
- [[Stock 股票 action|股票]]
- [[Asset allocation 资产配置 allocation d'actifs|资产配置]]
- [[Financial risks 金融风险 risques financiers|金融风险]]
- [[Central bank 中央银行 banque centrale|中央银行]]
- [[Securities market 证券市场 marché des valeurs mobilières|证券市场]]

# Self-check 自测

> [!question]- 票面利率 5% 的债券以 102 报价，其 YTM 高于还是低于 5%？
> 低于 5%。溢价债券的价格高于面值，持有到期时会有资本损失，抵消部分票息，故 $y < c$。

> [!question]- 修正久期 8 的债券，收益率上升 0.5 个百分点，价格约变化多少？
> $\Delta P/P \approx -8 \times 0.005 = -4\%$（凸性会使实际跌幅略小）。

> [!question]- 为什么零息债券的 Macaulay 久期等于其期限？
> 唯一现金流发生在 $T$，权重全在 $T$ 上，加权平均时间即 $T$。
