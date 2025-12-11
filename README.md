# Multi-Scale-Deep-Learning-for-Gold-Price-Forecasting
We propose to investigate methods for forecasting gold prices (XAU/USD) using a multi-timeframe dataset (2004–2025) containing 5-minute through monthly OHLC and volume data. 
Gold Price Forecasting: Classical & Deep Learning Approaches
AAI-501 Final Team Project – University of San Diego

This repository contains the full implementation, datasets, and experimental notebooks for our project on forecasting gold prices using classical time-series models and deep learning architectures.

The goal of the project was to compare how well different model families—SARIMA, Holt–Winters, Simple RNN, LSTM, GRU, BiLSTM, Attention-LSTM, CNN, and CNN-LSTM—perform on daily and monthly gold price data.

📁 Repository Structure
├── data/
│   ├── gold_daily.csv
│   ├── gold_monthly.csv
│   └── gold_cleaned.csv
│
├── notebooks/
│   ├── Multiple working files
│
├── final_code/
│  
│
└── README.md

📌 What’s in Each Folder?
data/

Contains the three datasets used in this project:

Daily gold price data

Monthly gold price data

A cleaned and standardised version used by the combined script

These are loaded directly by the final code and notebook files.

notebooks/

This folder includes all experimental and exploratory notebooks used throughout the project:

Early EDA

STL decomposition

ACF/PACF and stationarity checks

Rolling volatility and regime analysis

Multiple deep learning architectures (RNN, LSTM, GRU, BiLSTM, Attention-LSTM, CNN, CNN-LSTM)

Model tuning and comparison

These notebooks demonstrate the iterative process, code experimentation, and model diagnostics performed collaboratively.

final_code/Gold_Forecasting_Final_Combined.py

This script contains the unified, cleaned, and final version of the entire pipeline.
It integrates:

Data loading

Preprocessing

Classical baseline models

Deep learning models

Evaluation steps

The code is structured to run end-to-end without errors.

⚠️ Note on Repeated Imports and Duplicate Blocks

Throughout the notebooks and in the final combined script, you may notice repeated import statements or code blocks that appear similar.

This is intentional.

Each collaborator worked independently on different model families, and to ensure the combined script runs seamlessly:

All imports were kept exactly as in the original notebooks

No dependency was removed or consolidated if it risked breaking any section

This guarantees compatibility, reproducibility, and error-free execution across environments

While this results in some redundancy, it preserves the stability of the full forecasting pipeline.

🚀 How to Run the Project

Clone the repository:

git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>


Install dependencies:

pip install -r requirements.txt


Run the final forecasting pipeline:

python final_code/Gold_Forecasting_Final_Combined.py


Explore experiments:
Open the notebooks in Jupyter or VS Code.

📚 Project Summary

This project demonstrates the relationship between model complexity and data geometry in time-series forecasting.
Key findings include:

Simple RNN outperforms all advanced deep learning models

Complex architectures (LSTM, GRU, Attention, CNN-LSTM) tend to overfit on smooth, slowly evolving signals like gold

Classical models provide valuable interpretability but lack flexibility

Hybrid approaches and improved feature engineering are promising for future work

👥 Contributors

Shanmug Bhanu Prakash

Ravdeep Gill

Sulabh Jain
