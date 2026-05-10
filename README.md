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

Candidate stocks were evaluated using the following criteria:

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
```

---

## 6. Tools Used 使用工具

- Python
- pandas
- numpy
- matplotlib
- yfinance
- Jupyter Notebook
- GitHub

---

## 7. Methodology 分析方法

### English Version

The analysis follows these steps:

1. Download monthly price data using yfinance
2. Calculate monthly returns
3. Evaluate existing holdings using annualised return, annualised volatility, Sharpe Ratio and maximum drawdown
4. Analyse the correlation structure of the existing holdings
5. Screen candidate stocks for the remaining **40.60%** allocation
6. Select additional stocks based on risk-return performance, Sharpe Ratio and diversification benefits
7. Construct the full portfolio using the original **59.40%** existing holdings and the new **40.60%** allocation
8. Compare the existing holdings sleeve portfolio with the full portfolio

### 中文版本

本项目按照以下步骤进行：

1. 使用 yfinance 下载月度股票价格数据
2. 计算月度收益率
3. 使用年化收益率、年化波动率、Sharpe Ratio 和最大回撤评估已有持仓
4. 分析已有持仓之间的相关性结构
5. 对剩余 **40.60%** 配置的候选股票进行筛选
6. 基于风险收益表现、Sharpe Ratio 和分散化作用选择新增股票
7. 使用原有 **59.40%** 持仓和新增 **40.60%** 配置构建完整投资组合
8. 比较已有持仓 sleeve portfolio 与完整组合的表现

---

## 8. Key Results 核心结果

| Portfolio | Annualised Return | Annualised Volatility | Sharpe Ratio | Maximum Drawdown |
|---|---:|---:|---:|---:|
| Existing Holdings Sleeve Portfolio | 33.23% | 24.66% | 1.19 | -37.53% |
| Full Portfolio | 27.47% | 18.79% | 1.26 | -25.47% |

### English Version

The existing holdings sleeve portfolio generated a higher annualised return of **33.23%**, but it also carried higher annualised volatility of **24.66%** and a larger maximum drawdown of **-37.53%**.

After adding the selected stocks for the remaining **40.60%** allocation, the full portfolio achieved a lower annualised return of **27.47%**, but annualised volatility decreased from **24.66%** to **18.79%**. The Sharpe Ratio improved from **1.19** to **1.26**, and the maximum drawdown improved from **-37.53%** to **-25.47%**.

This suggests that the new allocation improved diversification, reduced downside risk and produced a more balanced risk-return profile.

### 中文版本

已有持仓 sleeve portfolio 的年化收益率较高，为 **33.23%**，但同时也伴随更高的年化波动率 **24.66%** 和更大的最大回撤 **-37.53%**。

在加入剩余 **40.60%** 的新增配置后，完整组合的年化收益率下降至 **27.47%**，但年化波动率从 **24.66%** 降至 **18.79%**。Sharpe Ratio 从 **1.19** 提升至 **1.26**，最大回撤也从 **-37.53%** 改善至 **-25.47%**。

这说明新增配置改善了组合分散化效果，降低了下行风险，并形成了更加均衡的风险收益特征。

---

## 9. Project Structure 项目结构

```text
stock-portfolio-risk-return-analysis
│
├── README.md
├── requirements.txt
│
├── data
│   ├── raw
│   │   ├── monthly_stock_prices.csv
│   │   └── candidate_monthly_stock_prices.csv
│   │
│   └── processed
│       ├── monthly_returns.csv
│       └── candidate_monthly_returns.csv
│
├── notebooks
│   └── portfolio_analysis.ipynb
│
├── outputs
│   ├── risk_return_summary.csv
│   ├── risk_return_summary_with_sharpe.csv
│   ├── cumulative_returns_stocks.csv
│   ├── existing_holdings_weights.csv
│   ├── existing_sleeve_portfolio_summary_with_sharpe.csv
│   ├── existing_holdings_correlation_matrix.csv
│   ├── stock_max_drawdown.csv
│   ├── candidate_risk_return_summary.csv
│   ├── candidate_screening_table.csv
│   ├── new_allocation_weights.csv
│   ├── full_portfolio_weights.csv
│   ├── full_portfolio_summary.csv
│   └── portfolio_comparison_summary.csv
│
└── charts
    ├── risk_return_scatter.png
    ├── cumulative_returns_stocks.png
    ├── existing_sleeve_portfolio_cumulative_return.png
    ├── existing_holdings_contribution_cumulative_return.png
    ├── existing_holdings_correlation_heatmap.png
    ├── existing_sleeve_drawdown.png
    ├── sharpe_ratio_ranking.png
    ├── candidate_risk_return_scatter.png
    ├── candidate_average_correlation_with_existing.png
    ├── full_portfolio_cumulative_return.png
    ├── full_portfolio_drawdown.png
    ├── cumulative_return_comparison.png
    └── drawdown_comparison.png
```

---

## 10. Main Outputs 主要输出

Key output files include:

主要输出文件包括：

- `notebooks/portfolio_analysis.ipynb`
- `outputs/portfolio_comparison_summary.csv`
- `outputs/candidate_screening_table.csv`
- `outputs/full_portfolio_weights.csv`
- `outputs/full_portfolio_summary.csv`
- `charts/cumulative_return_comparison.png`
- `charts/drawdown_comparison.png`
- `charts/full_portfolio_cumulative_return.png`
- `charts/full_portfolio_drawdown.png`

---

## 11. Key Charts 主要图表

The project generates several charts to support the analysis:

本项目生成了多张图表用于支持分析：

- Risk-return profile of existing holdings  
  已有持仓风险收益散点图

- Cumulative returns of selected stocks  
  个股累计收益对比图

- Correlation matrix of existing holdings  
  已有持仓相关性矩阵图

- Existing holdings sleeve portfolio drawdown  
  已有持仓 sleeve portfolio 回撤图

- Candidate stocks average correlation with existing holdings  
  候选股票与已有持仓平均相关性图

- Full portfolio cumulative return  
  完整组合累计收益图

- Full portfolio drawdown  
  完整组合回撤图

- Cumulative return comparison  
  累计收益对比图

- Drawdown comparison  
  回撤对比图

---

## 12. Conclusion 结论

### English Version

This project shows that portfolio construction should not focus only on maximising return. Although the existing holdings sleeve portfolio achieved a higher annualised return, it also carried higher volatility and larger downside risk.

By allocating the remaining **40.60%** to selected stocks from different sectors, the full portfolio achieved lower volatility, a smaller maximum drawdown and a higher Sharpe Ratio. This indicates that the additional allocation improved risk-adjusted performance and portfolio stability.

The results suggest that diversification across sectors can help reduce downside risk and improve the balance between return and risk.

### 中文版本

本项目说明，投资组合构建不应只关注收益最大化。虽然已有持仓 sleeve portfolio 实现了更高的年化收益率，但其波动率和下行风险也更高。

通过将剩余 **40.60%** 配置到不同行业的筛选股票中，完整组合实现了更低的波动率、更小的最大回撤和更高的 Sharpe Ratio。这表明新增配置改善了组合的风险调整后表现和整体稳定性。

结果说明，跨行业分散配置有助于降低下行风险，并改善收益与风险之间的平衡。

---

## 13. Notes 说明

### English Version

This project is for educational and portfolio demonstration purposes only. It is not investment advice.

The analysis is based on historical monthly price data from 2020 to 2025. Historical performance does not guarantee future results.

### 中文版本

本项目仅用于学习和作品集展示目的，不构成投资建议。

本项目分析基于 2020 年至 2025 年的历史月度价格数据。历史表现不代表未来结果。

完整组合由已有 **59.40%** 持仓和新增 **40.60%** 配置组成。

```text
Full Portfolio = Existing Holdings 59.40% + New Allocation 40.60%
