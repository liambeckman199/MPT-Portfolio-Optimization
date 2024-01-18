# MPT Portfolio Optimization 

## Overview
This project focuses on constructing an optimized investment portfolio using the Mean-Variance Optimization (MVO) framework. It leverages historical market data to estimate the risk and return of different assets and optimizes the asset allocation to maximize returns for a given level of risk. This project extensively utilizes the Riskfolio-Lib package for portfolio optimization and analysis. Riskfolio-Lib is a Python library dedicated to investment portfolio optimization using the latest techniques in the field. More information about Riskfolio-Lib can be found at its GitHub repository: [Riskfolio-Lib GitHub](https://github.com/dcajasn/Riskfolio-Lib).

## Installation

To use this project, clone the repository to your local machine or download the source code.

## Prerequisites

- Python 3.x
- Jupyter Notebook

## Setting Up the Environment

Create a virtual environment (optional but recommended)

## Install Required Packages

Install the required Python packages by running the following command:

```bash
pip install -r requirements.txt
```

## Running the Jupyter Notebook

Open the Jupyter Notebook (MPT Portfolio Optimization.ipynb) in your Jupyter environment:

## Refreshing the Token for Questrade's API

To interact with Questrade's API, you need a valid token. Tokens can expire, so you may need to regenerate them occasionally.

Regenerate the token by visiting: Questrade Token Generation.

Update the token in your code:

```bash
q = Questrade(refresh_token='YOUR_NEW_REFRESH_TOKEN')
```

Remember to replace 'YOUR_NEW_REFRESH_TOKEN' with the actual token you obtain from Questrade.

Questrade Account Numbers
To run this project, you will need to obtain your Questrade account numbers. Once you have your account numbers, you should set them as environment variables in your project. This is essential for retrieving account-specific positions for TFSA and RRSP portfolios.

You can set the account numbers in your code as follows

```bash
positions_1 = q.account_positions('YOUR_ACCOUNT_NUMBER_1')
positions_2 = q.account_positions('YOUR_ACCOUNT_NUMBER_2')
```

Replace 'YOUR_ACCOUNT_NUMBER_1' and 'YOUR_ACCOUNT_NUMBER_2' with your actual account numbers from Questrade.

## Usage

1. Data Collection: Gather historical return data for various assets you are considering for your portfolio.

2. Mean-Variance Optimization: Utilize the MVO framework to analyze the risk-return trade-off of different assets and determine the optimal asset allocation.

3. Efficient Frontier Visualization: Plot the efficient frontier to understand the risk-return relationship and make informed decisions.

4. Portfolio Rebalancing: Randomly resample initial weights or set specific thresholds to rebalance the portfolio.

5. Sensitivity Analysis: Perform optimizations under different conditions (e.g., varying time frames or risk measures) to test the robustness of the portfolio allocation.

