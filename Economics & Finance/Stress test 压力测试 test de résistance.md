---
aliases:
  - stress test
  - 压力测试
  - test de résistance
---
# Definition

In [[Finance 金融 finance|finance]], a **stress test** is an analysis or simulation designed to determine the ability of a given financial instrument or financial institution to deal with an economic crisis.

**压力测试**（stress test, *test de résistance*，也常直接用 *stress test*）是一种[[Risk management 风险管理 gestion des risques|风险管理]]工具：假设出现极端但可能发生的不利情景（如股市暴跌、利率飙升、经济衰退），评估某个金融工具、[[Portfolio 投资组合 portefeuille|投资组合]]或金融机构会遭受多大损失、能否继续经营。

它弥补了 [[VaR 风险价值 valeur en risque|VaR]] 等统计模型的不足：VaR 刻画的是"正常市场"下的损失，而压力测试关注的是"尾部"（tail）的极端事件。

# Classification

- **敏感性分析**（sensitivity analysis）：只改变单一风险因子，如利率上升 200 个基点（bp）。
- **情景分析**（scenario analysis）：多个因子同时变化。
  - **历史情景**：重演 2008 年金融危机、2020 年新冠冲击等；
  - **假设情景**：构造尚未发生但合理的情景。
- **反向压力测试**（reverse stress test）：先设定"机构倒闭"等结果，倒推什么情景会导致该结果。

# Bank stress test

A **bank stress test** is a type of simulation that evaluates a financial institution's ability to withstand adverse economic or market conditions by examining its balance sheet.

**银行压力测试**由监管机构或银行自身执行，检验在不利情景下银行的资本充足率（capital adequacy ratio）是否仍高于监管最低要求。2008 年金融危机后成为常规监管工具，代表性的有：

- 美国美联储的 **CCAR / DFAST**；
- 欧洲银行管理局（EBA）的欧盟范围压力测试；
- 中国人民银行的年度银行业压力测试。

未通过测试的银行可能被要求补充资本、限制分红或回购。

# Example

某银行核心一级资本 100 亿元，风险加权资产 1000 亿元，资本充足率 10%。在"GDP 下降 5%、房价下跌 30%"的不利情景下，模拟贷款损失 40 亿元，同时风险加权资产升至 1100 亿元，则资本充足率降为 $(100-40)/1100 \approx 5.5\%$。若监管要求为 7%，则该银行未通过测试。

# Related

- [[Financial risks 金融风险 risques financiers|Financial risks]]
- [[Leverage 杠杆 effet de levier|杠杆]]
- [[Institutional investor 机构投资者 investisseur institutionnel|机构投资者]]
