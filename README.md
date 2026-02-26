# Portfolio Optimization with CVaR (Linear Programming)

A comprehensive portfolio optimization project using Conditional Value at Risk (CVaR) constraints and linear programming techniques.

## Project Overview

This project implements portfolio optimization strategies using CVaR (Conditional Value at Risk) as a risk measure. The analysis spans multiple phases of data preparation, optimization, sensitivity analysis, and rolling window rebalancing.

**Key Concept:** CVaR (also known as Expected Shortfall) is a tail risk measure that captures the average loss in the worst-case scenarios, making it a more conservative risk metric than traditional standard deviation.

## Repository Structure

```
.
├── README.md                           # This file
├── notebooks/                          # Jupyter notebooks with analysis
│   ├── parts_1_2.ipynb                # Data prep & portfolio optimization (β=0.95)
│   ├── part_3.ipynb                   # Sensitivity analysis for β = 0.90, 0.95, 0.99
│   ├── part_4.ipynb                   # Conservative min-max monthly CVaR (2019)
│   ├── parts_5_6.ipynb                # Monthly re-optimization (2020 rolling windows)
│   ├── combined_submission.ipynb       # Master notebook (end-to-end workflow)
│   └── Project_1_Darius.ipynb          # Reference implementation
├── data/                               # Historical stock price data
│   ├── stocks2019.csv                  # 2019 stock prices
│   └── stocks2020.csv                  # 2020 stock prices
└── docs/                               # Documentation
    └── project 1 - cvar - overview.pdf # Project overview and requirements
```

## Project Phases

| Part | Description | Status | Owner |
|------|-------------|--------|-------|
| 1–2 | Data preparation & return calculation; Portfolio optimization (β=0.95, in/out-of-sample) | ✓ Complete | Darius |
| 3 | Sensitivity analysis for β = 0.90, 0.95, 0.99 | ✓ Complete | Archie |
| 4 | Conservative min–max monthly CVaR (2019) | ✓ Complete | Archie |
| 5-6 | Monthly re-optimization (2020 rolling windows) | ✓ Complete | Zan |
| 7 | Final report assembly (PDF with graphs & recommendations) | In Progress | Rizvee |
| Combined | End-to-end workflow notebook | ✓ Complete | Rizvee |

## Quick Start

### Run Notebooks Locally
1. Clone the repository
2. Install dependencies: `pip install pandas numpy scipy cvxpy matplotlib`
3. Open and run notebooks in Jupyter:
   ```bash
   jupyter notebook notebooks/parts_1_2.ipynb
   ```

### Run in Google Colab
Click on the Colab links in the project table below. Notebooks will automatically download data from GitHub.

## Key Findings

The project analyzes portfolio optimization using CVaR constraints with:
- **2019 Data:** Out-of-sample validation and sensitivity analysis
- **2020 Data:** Rolling window re-optimization for monthly rebalancing
- **Risk Levels:** β = 0.90, 0.95, 0.99 (confidence levels)

## Technologies Used

- **Python** (pandas, NumPy)
- **Optimization:** CVXPY (convex optimization)
- **Data Analysis:** Jupyter Notebooks
- **Visualization:** Matplotlib

## Team

- **Darius:** Parts 1-2 (Data preparation & optimization)
- **Archie:** Parts 3-4 (Sensitivity analysis & conservative strategies)
- **Zan:** Parts 5-6 (Rolling window re-optimization)
- **Rizvee:** Combined notebook & final report

## Notes

- Notebooks use remote data URLs as fallback if local files are unavailable
- All notebooks are compatible with Google Colab
- For collaboration, notebooks should be saved to GitHub using Colab's native save feature

## License

Academic project for MSBA optimization course
