---
aliases:
  - compound interest
  - intérêts composés
---
# Definition

**复利**（compound interest, *intérêts composés*）是指每一期产生的利息加入本金，在下一期一同计息的计息方式，俗称"利滚利"。与之相对的是**单利**（simple interest, *intérêts simples*）：只对初始本金计息。

# Formula

设本金 $P$，年利率 $r$，每年复利 $n$ 次，期限 $t$ 年，则终值（future value）为

$$A = P\left(1+\frac{r}{n}\right)^{nt}$$

当 $n \to \infty$ 时得到**连续复利**（continuous compounding）：

$$A = P\,e^{rt}$$

单利终值则为 $A = P(1+rt)$，随时间线性增长；复利终值随时间指数增长。

**名义利率与实际年利率**：名义年利率 $r$ 每年复利 $n$ 次，对应的实际年利率（effective annual rate, EAR）为 $\left(1+\frac{r}{n}\right)^n - 1$。

# Rule of 72

估算资产翻倍所需年数的经验法则：

$$t_{\text{double}} \approx \frac{72}{100\,r}$$

例如年收益率 6%，约 $72/6 = 12$ 年翻倍。（精确值为 $\ln 2 / \ln(1.06) \approx 11.9$ 年。）

# Example

本金 10 000 元，年利率 5%，30 年：

- 单利：$10000\times(1+0.05\times30) = 25\,000$ 元；
- 年复利：$10000\times1.05^{30} \approx 43\,219$ 元。

两者差距随时间迅速扩大，这就是复利的作用。反过来，复利同样作用于债务（如信用卡欠款）和[[Inflation 通货膨胀 inflation|通货膨胀]]对购买力的侵蚀。

# Related

- [[Investment 投资 investissement|投资]]
- [[Personal finance 个人理财 finances personnelles|个人理财]]
- [[Dollar cost averaging 平均成本法 investissement programmé|定投]]
- [[Forward contract 远期合同 contrat à terme|远期合同]]（远期定价使用连续复利）
- [[Time value of money 货币时间价值 valeur temps de l'argent|货币时间价值]]
- [[Interest rate 利率 taux d'intérêt|利率]]
