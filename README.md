使用 Python 分析美国股票风险与收益特征的项目
# Stock Portfolio Risk and Return Analysis

## 项目背景 Project Background

本项目使用 Python 对 10 只美国上市股票进行风险与收益分析。分析内容包括月度收益率、年化收益率、年化波动率、相关性矩阵、投资组合累计收益、最大回撤和夏普比率等指标。

This project uses Python to analyse the risk and return characteristics of 10 selected US-listed stocks. The analysis covers monthly returns, annualised return, annualised volatility, correlation matrix, portfolio cumulative return, maximum drawdown and Sharpe Ratio.

## 项目目标 Project Objectives

本项目的主要目标包括：

- 计算每只股票的月度收益率
- 计算年化收益率和年化波动率
- 分析股票之间的相关性
- 构建一个加权股票组合
- 计算投资组合累计收益
- 计算最大回撤
- 计算 Sharpe Ratio
- 使用图表展示风险收益表现

The main objectives of this project are to calculate key risk and return indicators, evaluate portfolio performance and visualise the results using Python.

## 股票选择 Selected Stocks

本项目选择以下 10 只美国上市股票：

| Company | Ticker |
|---|---|
| Nvidia | NVDA |
| Microsoft | MSFT |
| Amazon | AMZN |
| Meta | META |
| Apple | AAPL |
| Broadcom | AVGO |
| Visa | V |
| Intuit | INTU |
| Netflix | NFLX |
| Eli Lilly | LLY |

---

## 使用工具 Tools Used

- Python
- pandas
- numpy
- matplotlib
- Jupyter Notebook
- Excel / CSV
- GitHub

## 分析内容 Methodology

本项目计划完成以下分析步骤：

1. 收集并整理股票月度价格数据
2. 计算股票月度收益率
3. 计算每只股票的年化收益率和年化波动率
4. 计算股票之间的相关性矩阵
5. 构建加权投资组合
6. 计算投资组合累计收益
7. 计算最大回撤
8. 计算 Sharpe Ratio
9. 可视化风险收益表现

## 预期输出 Expected Outputs

本项目最终将生成以下结果：

- 月度收益率表
- 年化收益率与年化波动率汇总表
- 股票相关性矩阵
- 投资组合累计收益图
- 最大回撤图
- 风险收益散点图
- 项目分析结论

## 项目结构 Project Structure

```text
stock-portfolio-risk-return-analysis
│
├── README.md
├── data
│   ├── raw
│   └── processed
├── notebooks
│   └── portfolio_analysis.ipynb
├── charts
├── outputs
└── requirements.txt
