---
aliases:
  - index fund
  - fonds indiciel
  - passive fund
  - gestion passive
summary: 复制某一市场指数、追求市场平均收益的低成本基金
tags: [finance, learning]
---
# Definition

**指数基金**（index fund, *fonds indiciel*）是以复制某一市场指数（如[[Standard & Poor’s 500 标准普尔指数 indice S&P 500|标普500]]、MSCI World、CAC 40）的成分与权重为目标的[[Fund 基金 fonds|基金]]。它不试图"跑赢市场"，而是追求与指数一致的收益，属于**被动管理**（passive management, *gestion passive*）。

与之相对的是**主动管理**（active management, *gestion active*）：基金经理通过选股（stock picking）和择时（market timing）试图获得超过基准的超额收益（alpha）。

# Mechanism

**指数编制（市值加权）**。大多数宽基指数按自由流通市值加权（cap-weighted）。设成分股 $i$ 的价格为 $p_i$、流通股数为 $q_i$，则权重为

$$w_i = \frac{p_i q_i}{\sum_j p_j q_j}.$$

市值加权的一个重要性质：价格变动会自动调整权重，基金无需频繁调仓，换手率（turnover）和交易成本因此很低。其他方案包括等权（equal-weight）、价格加权（如道琼斯工业指数）和基本面加权。

**跟踪误差**（tracking error, *écart de suivi*）。设基金收益 $R_p$、指数收益 $R_b$，跟踪误差定义为超额收益的标准差

$$\mathrm{TE} = \sigma(R_p - R_b).$$

它来源于费用、现金拖累、抽样复制、分红再投资时点等。需区分：**跟踪差异**（tracking difference）是 $R_p - R_b$ 的平均值，通常约等于负的费率。

**为何多数主动基金长期跑输**。William Sharpe 的"主动管理算术"（1991）：所有投资者持有的总和就是市场组合；扣费前，主动投资者整体的平均收益必然等于市场收益，被动投资者亦然。因此

$$\bar R_{\text{active, net}} = R_{\text{market}} - c_{\text{active}} < R_{\text{market}} - c_{\text{passive}} = \bar R_{\text{passive, net}},$$

只要主动管理的成本 $c_{\text{active}}$ 更高。这是一个恒等式式的论证，不依赖[[Efficient market hypothesis 有效市场假说 hypothèse des marchés efficients|有效市场假说]]。实证上（如 S&P 的 SPIVA 报告），15 年期内约九成美国大盘主动基金跑输基准。

# Example

假设某指数 20 年年化收益 7%。指数基金总费率 0.2%，主动基金 1.8%，且主动基金扣费前恰好与指数持平。初始投入 10 000 欧元：

- 指数基金：$10000 \times 1.068^{20} \approx 37\,280$ 欧元；
- 主动基金：$10000 \times 1.052^{20} \approx 27\,560$ 欧元。

1.6 个百分点的费率差在[[Compound interest 复利 intérêts composés|复利]]作用下吞掉了近 1 万欧元，见 [[Investment fees 投资费用 frais|投资费用]]。

# Common misconceptions

- "指数基金没有风险。"它承担完整的市场风险（systematic risk），只是消除了选股的个股风险。
- "被动 = 不做任何决定。"选择哪个指数、以及[[Asset allocation 资产配置 allocation d'actifs|资产配置]]本身就是主动决策。
- 市值加权指数在泡沫中会提高高估股票的权重，这是其结构特征而非缺陷的"修正"。

# Vocabulaire

| français | 中文 | English |
|---|---|---|
| le fonds indiciel (m.) | 指数基金 | index fund |
| la gestion passive (f.) | 被动管理 | passive management |
| la gestion active (f.) | 主动管理 | active management |
| l'indice de référence (m.) | 基准指数 | benchmark |
| la capitalisation boursière (f.) | 市值 | market capitalisation |
| l'écart de suivi (m.) | 跟踪误差 | tracking error |
| les frais de gestion (m. pl.) | 管理费 | management fees |

# Related

- [[ETF 交易所交易基金 fonds négocié en bourse|ETF]]
- [[Mutual fund 共同基金 fonds commun de placement|共同基金]]
- [[Standard & Poor’s 500 标准普尔指数 indice S&P 500|标普500]]
- [[Diversification 分散投资 diversification|分散投资]]
- [[Efficient market hypothesis 有效市场假说 hypothèse des marchés efficients|有效市场假说]]
- [[Investment fees 投资费用 frais|投资费用]]
- [[Portfolio 投资组合 portefeuille|投资组合]]

# Self-check 自测

> [!question]- 为什么 Sharpe 的论证不需要假设市场有效？
> 它只用到会计恒等式：主动与被动投资者合起来持有市场组合，被动者扣费前获得市场收益，故主动者整体扣费前也只能获得市场收益。扣除更高费用后，平均主动投资者必然跑输平均被动投资者。个别主动基金可以跑赢，但整体不能。

> [!question]- 跟踪误差与跟踪差异有何区别？
> 跟踪差异是 $R_p - R_b$ 的均值，衡量系统性偏离（主要是费用）；跟踪误差是 $R_p - R_b$ 的标准差，衡量偏离的波动程度。一只基金可以跟踪差异稳定为 $-0.2\%$ 而跟踪误差很小。

> [!question]- 市值加权指数为何换手率低？
> 权重 $w_i \propto p_i q_i$ 随价格自动变化，持有固定股数的组合天然保持与指数一致的权重，只有成分股调整、股本变动时才需交易。
