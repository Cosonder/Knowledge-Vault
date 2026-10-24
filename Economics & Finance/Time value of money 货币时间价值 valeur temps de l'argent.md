---
aliases:
  - time value of money
  - valeur temps de l'argent
  - tvm
  - present value
  - npv
  - valeur actuelle nette
  - van
summary: 今天的一元钱比未来的一元钱更值钱；用贴现在不同时点之间比较现金流
tags: [finance, learning]
---
# Definition

**货币时间价值**（time value of money, TVM, *valeur temps de l'argent*）指：在存在正的[[Interest rate 利率 taux d'intérêt|利率]]时，今天的一笔钱可以投资生息，因此它比未来同等金额更有价值。不同时点的现金流不能直接相加，必须先换算到同一时点。

- **终值**（future value, FV, *valeur future/acquise*）：把现在的金额"推"到未来；
- **现值**（present value, PV, *valeur actuelle*）：把未来的金额"拉"回现在，这一操作称为**贴现**（discounting, *actualisation*），所用利率称为**贴现率**（discount rate, *taux d'actualisation*）。

# Formula

单期利率 $r$，$t$ 期：

$$FV = PV\,(1+r)^t, \qquad PV = \frac{FV}{(1+r)^t}.$$

$(1+r)^{-t}$ 称为贴现因子（discount factor）。连续复利下为 $e^{-rt}$。

**年金**（annuity, *annuité*）：每期期末支付 $C$，共 $n$ 期。由等比级数求和，

$$PV = \sum_{k=1}^{n}\frac{C}{(1+r)^k} = \frac{C}{r}\left[1-(1+r)^{-n}\right], \qquad FV = C\,\frac{(1+r)^n-1}{r}.$$

**永续年金**（perpetuity, *rente perpétuelle*）：令 $n\to\infty$（需 $r>0$），

$$PV = \frac{C}{r}.$$

若现金流以速率 $g<r$ 增长（首期 $C$），则 $PV = \dfrac{C}{r-g}$（Gordon 增长模型）。

**净现值**（net present value, NPV, *valeur actuelle nette*, VAN）：项目在 $t=0,\dots,n$ 的现金流 $CF_t$（初始投资为负）的现值之和，

$$NPV = \sum_{t=0}^{n}\frac{CF_t}{(1+r)^t}.$$

决策准则：$NPV>0$ 表示该项目在贴现率 $r$ 下创造价值。使 $NPV=0$ 的 $r$ 称为**内部收益率**（IRR, *taux de rendement interne*, TRI）。

# Example

每月末投入 500 欧元，月利率 $r = 0.4\%$（约 4.9% 年化），持续 $n=240$ 个月（20 年）：

$$FV = 500\times\frac{1.004^{240}-1}{0.004} \approx 500\times\frac{2.6067-1}{0.004} \approx 200\,838 \text{ 欧元},$$

而投入本金合计 $120\,000$ 欧元。反过来，若想每年从一笔资金中永续取出 20 000 欧元，在 4% 的实际回报假设下所需现值为 $20000/0.04 = 500\,000$ 欧元——这正是[[Safe withdrawal rate 安全提取率 taux de retrait|安全提取率]]讨论的起点（实际情形中回报有波动，不能直接套用此公式）。

# Common misconceptions

- **把名义现金流用实际利率贴现（或反之）**：名义现金流配名义贴现率，实际现金流配实际贴现率，二者需一致。
- **"贴现率是一个客观常数"**：贴现率反映机会成本与风险，选择不同会显著改变 NPV，尤其是长期现金流。
- **忽略支付时点**：期初年金（annuity due）的现值是期末年金的 $(1+r)$ 倍。

# Vocabulaire

| français | 中文 | English |
|---|---|---|
| *la valeur actuelle* (f.) | 现值 | present value |
| *la valeur future / acquise* (f.) | 终值 | future value |
| *l'actualisation* (f.) | 贴现 | discounting |
| *le taux d'actualisation* (m.) | 贴现率 | discount rate |
| *l'annuité* (f.) | 年金（每期付款） | annuity payment |
| *la rente perpétuelle* (f.) | 永续年金 | perpetuity |
| *la valeur actuelle nette* (f.) | 净现值 | net present value |
| *le taux de rendement interne* (m.) | 内部收益率 | internal rate of return |

# Related

- [[Compound interest 复利 intérêts composés|复利]]
- [[Interest rate 利率 taux d'intérêt|利率]]
- [[Bond 债券 obligation|债券]]（债券价格即现金流现值）
- [[Inflation 通货膨胀 inflation|通货膨胀]]
- [[Safe withdrawal rate 安全提取率 taux de retrait|安全提取率]]
- [[Dollar cost averaging 平均成本法 investissement programmé|定投]]
- [[Investment 投资 investissement|投资]]

# Self-check 自测

> [!question]- 推导期末年金现值公式。
> 令 $v = (1+r)^{-1}$，则 $PV = C(v+v^2+\dots+v^n) = Cv\frac{1-v^n}{1-v}$。由于 $\frac{v}{1-v} = \frac{1}{r}$，得 $PV = \frac{C}{r}(1-v^n)$。

> [!question]- 贴现率 5% 下，第 30 年收到的 100 000 元现值是多少？贴现率升到 7% 呢？
> $100000/1.05^{30} \approx 23\,138$；$100000/1.07^{30} \approx 13\,137$。长期现金流的现值对贴现率高度敏感。

> [!question]- 一个项目今天投入 1 000，一年后收回 1 080。在贴现率 10% 下是否应接受？IRR 是多少？
> $NPV = -1000 + 1080/1.1 \approx -18.2 < 0$，不接受。IRR 满足 $1080/(1+\text{IRR}) = 1000$，即 8%，低于 10%。
