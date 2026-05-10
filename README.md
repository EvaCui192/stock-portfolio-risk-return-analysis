# Portfolio Completion and Risk-Return Analysis  
# 基于已有持仓的投资组合补全与风险收益分析

## 1. Project Background 项目背景

### English Version

This project uses Python to support portfolio completion and risk-return analysis. The starting point is an existing equity allocation consisting of 10 US-listed stocks, which together account for **59.40%** of the original portfolio.

The objective is to analyse the risk and return characteristics of the existing holdings, screen candidate stocks for the remaining **40.60%** allocation, construct a full portfolio, and evaluate whether the new allocation improves the overall risk-return profile.

### 中文版本

本项目使用 Python 支持投资组合补全与风险收益分析。项目起点是一个已经给定的股票持仓组合，其中包含 10 只美国上市股票，合计占原始投资组合的 **59.40%**。

项目目标是先分析已有持仓的风险收益特征，再为剩余 **40.60%** 权重筛选新增股票，构建完整投资组合，并评估新增配置是否改善了整体组合的风险收益表现。

---

## 2. Existing Holdings 已有持仓

The existing holdings account for **59.40%** of the original portfolio.

已有持仓合计占原始投资组合的 **59.40%**。

| Company | Ticker | Original Weight |
|---|---:|---:|
| Nvidia | NVDA | 9.81% |
| Microsoft | MSFT | 9.65% |
| Amazon | AMZN | 9.22% |
| Meta | META | 6.33% |
| Apple | AAPL | 5.35% |
| Broadcom | AVGO | 4.81% |
| Visa | V | 4.25% |
| Intuit | INTU | 3.68% |
| Netflix | NFLX | 3.38% |
| Eli Lilly | LLY | 2.92% |
| **Total** |  | **59.40%** |

---

## 3. Candidate Stock Screening 候选股票筛选

### English Version

To complete the remaining **40.60%** allocation, a candidate stock pool was constructed across different sectors, including financials, energy, industrials, healthcare, utilities and consumer defensive stocks.

Candidate stocks were evaluated using:

- Annualised return
- Annualised volatility
- Sharpe Ratio
- Average correlation with existing holdings
- Sector diversification potential

### 中文版本

为了补全剩余 **40.60%** 的配置，本项目构建了一个跨行业候选股票池，覆盖金融、能源、工业、医疗、公用事业和消费防御等板块。

候选股票主要基于以下指标进行筛选：

- 年化收益率
- 年化波动率
- Sharpe Ratio
- 与已有持仓的平均相关性
- 行业分散化作用

---

## 4. New Allocation 新增配置

Based on risk-return performance, Sharpe Ratio and diversification benefits, the following 6 stocks were selected for the remaining **40.60%** allocation.

基于风险收益表现、Sharpe Ratio 和分散化效果，项目最终选择以下 6 只股票配置剩余 **40.60%** 权重。

| Company | Ticker | New Allocation Weight |
|---|---:|---:|
| Caterpillar | CAT | 8.00% |
| Exxon Mobil | XOM | 7.50% |
| RTX | RTX | 7.00% |
| JPMorgan Chase | JPM | 6.50% |
| Johnson & Johnson | JNJ | 6.00% |
| Procter & Gamble | PG | 5.60% |
| **Total** |  | **40.60%** |

---

## 5. Final Portfolio 完整投资组合

The final portfolio combines the existing **59.40%** holdings with the new **40.60%** allocation.

完整组合由已有 **59.40%** 持仓和新增 **40.60%** 配置组成。

```text
Full Portfolio = Existing Holdings 59.40% + New Allocation 40.60%
