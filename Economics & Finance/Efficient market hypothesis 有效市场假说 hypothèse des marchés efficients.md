---
aliases:
  - efficient market hypothesis
  - hypothèse des marchés efficients
  - emh
  - market efficiency
  - efficience des marchés
summary: 资产价格充分反映可得信息，难以持续获得超额收益
tags: [finance, learning]
---
# Definition

**有效市场假说**（efficient market hypothesis, EMH, *hypothèse des marchés efficients*）由 Eugene Fama（1970）系统表述：在有效市场中，资产价格**充分反映**所有可得信息。推论是：仅凭这些信息，投资者无法在经风险调整后持续获得超额收益。

形式化表述：设 $\Phi_t$ 为 $t$ 时的信息集，$R_{t+1}$ 为下一期收益，$\mathbb{E}^m$ 为某个均衡定价模型给出的期望收益，则

$$\mathbb{E}\big[R_{t+1} - \mathbb{E}^m(R_{t+1}\mid\Phi_t)\,\big|\,\Phi_t\big] = 0,$$

即超额收益相对于 $\Phi_t$ 是一个**鞅差**（martingale difference），不可预测。

# Classification

按信息集 $\Phi_t$ 的大小分为三种形式（嵌套关系：强式 ⇒ 半强式 ⇒ 弱式）：

| 形式 | 信息集 | 含义 |
|---|---|---|
| **弱式**（weak, *faible*） | 历史价格与成交量 | 技术分析无效 |
| **半强式**（semi-strong, *semi-forte*） | 所有公开信息（财报、新闻） | 基本面分析无法持续获得超额收益；价格对新消息迅速调整 |
| **强式**（strong, *forte*） | 包括内幕信息在内的全部信息 | 连内幕人士也无法获利；实证上普遍被否定 |

# Mechanism

**随机游走**（random walk, *marche aléatoire*）。若价格已包含当前信息，价格变化只能来自新信息，而新信息本身不可预测，因此对数价格近似

$$\ln P_{t+1} = \ln P_t + \mu + \varepsilon_{t+1}, \qquad \varepsilon_{t+1} \text{ 不可预测}.$$

注意 EMH 只要求超额收益是鞅差，比 i.i.d. 随机游走更弱：[[Volatility 波动率 volatilité|波动率]]可以随时间变化（如波动聚集），期望收益也可随风险变化。

**套利与竞争**是效率的来源：一旦存在可预测的利润机会，大量投资者的交易会把它消除。由此有 Grossman–Stiglitz 悖论（1980）：若市场完全有效，没人有动力付费收集信息，市场也就不会有效。均衡中必须保留恰好补偿信息成本的少量低效。

**联合假设问题**（joint-hypothesis problem）。检验"超额收益"必须先指定"正常收益"模型 $\mathbb{E}^m$（如 CAPM）。因此任何异常结果既可能说明市场无效，也可能说明定价模型错误，二者无法单独检验。

# Anomalies and behavioral critique

实证中发现的**异象**（anomalies）：

- **动量效应**（momentum）：过去 3–12 个月表现好的股票未来仍倾向于表现好（Jegadeesh–Titman 1993）；
- **价值效应与规模效应**：低市净率、小市值股票长期收益偏高（Fama–French 1992）；有效市场派解释为风险补偿，行为派解释为错误定价；
- **盈余公告后漂移**（post-earnings-announcement drift）；
- **泡沫与过度波动**：Shiller（1981）指出股价波动远大于后续股息变化所能解释的程度。

**行为金融**（behavioral finance）的批评：投资者存在过度自信、损失厌恶、羊群效应等系统性偏差（Kahneman–Tversky），而**套利限制**（limits to arbitrage，如卖空成本、噪声交易者风险、资金约束，见[[Short selling 做空 vente à découvert|做空]]）使错误定价可以持续。正如常引的那句话：市场保持非理性的时间可能比你保持偿付能力的时间更长。

# Implication for index investing

即使市场并不完全有效，只要异象在扣除交易成本、税和费用后难以被普通投资者稳定利用，结论就和 EMH 相近：选股与择时的期望净收益为负。这为[[Index fund 指数基金 fonds indiciel|指数基金]]提供了理论支持；另一个独立的支持是 Sharpe 的主动管理算术（不依赖 EMH）。2013 年诺贝尔经济学奖同时授予 Fama 与 Shiller，反映了这一问题的两面。

# Example

假设一则利好消息使某公司内在价值从 50 欧元升至 55 欧元。半强式有效市场中，消息公布后几秒到几分钟内价格就跳到约 55 欧元。若投资者在第二天早上读到新闻后以 55 欧元买入，其期望超额收益为 0。实证的事件研究（event study）通过计算公告前后的累计异常收益 $\mathrm{CAR} = \sum_t (R_t - \hat R_t)$ 检验这一点：多数研究发现价格调整集中在公告日，但存在部分漂移。

# Common misconceptions

- "有效市场意味着价格总是正确的。"EMH 只说价格偏离无法被可预测地利用，并不保证价格等于"真实价值"。
- "有效市场意味着无法赚钱。"投资者仍可获得与风险相应的正常收益，只是不能持续获得超额收益。
- "有人连续多年跑赢市场，所以 EMH 错了。"在大量基金经理中，靠运气产生若干长期赢家是统计上预期之中的（幸存者偏差）。

# Vocabulaire

| français | 中文 | English |
|---|---|---|
| l'efficience des marchés (f.) | 市场有效性 | market efficiency |
| la marche aléatoire (f.) | 随机游走 | random walk |
| le délit d'initié (m.) | 内幕交易 | insider trading |
| l'arbitrage (m.) | 套利 | arbitrage |
| la finance comportementale (f.) | 行为金融 | behavioral finance |
| le biais cognitif (m.) | 认知偏差 | cognitive bias |
| la bulle spéculative (f.) | 投机泡沫 | speculative bubble |

# Related

- [[Index fund 指数基金 fonds indiciel|指数基金]]
- [[Market 市场 marché|市场]]
- [[Stock market 股票市场 marché boursier|股票市场]]
- [[Speculation 投机 spéculation|投机]]
- [[Return 收益率 rendement|收益率]]
- [[Volatility 波动率 volatilité|波动率]]
- [[Investment strategy 投资策略 stratégie d'investissement|投资策略]]

# Self-check 自测

> [!question]- 为什么说 EMH 不可单独检验？
> 这是联合假设问题：判断收益是否"超额"必须先假定一个正常收益模型。检验拒绝时，无法区分是市场无效还是模型设定错误。

> [!question]- 弱式有效与随机游走模型是什么关系？
> 弱式有效要求超额收益相对于历史价格不可预测（鞅差性质）。i.i.d. 随机游走是更强的特例；波动率随时间变化（波动聚集）与弱式有效相容，但与 i.i.d. 随机游走不相容。

> [!question]- Grossman–Stiglitz 悖论说的是什么？
> 若价格已完全反映信息，收集信息无利可图，便没人收集信息，价格也就无法反映信息。因此均衡中市场只能"近似有效"，残留的低效恰好补偿信息成本。
