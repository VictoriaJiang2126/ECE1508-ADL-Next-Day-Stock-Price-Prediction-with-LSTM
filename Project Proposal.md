# Topic: Next-Day Stock Price Prediction with LSTM

## **Objective**

Build an LSTM model to predict the next-day stock price using past 30 days’ daily prices. Use a clean pipeline in PyTorch, download data from Alpha Vantage, save input CSV files, and evaluate results with clear metrics and plots. The final deliverable includes a runnable Jupyter Notebook, required datasets, a short presentation and a report.

## **Motivation**

Stock prices are time series data with trends and short-term patterns. LSTM is designed to learn patterns from sequences, so it fits this task well. This project helps practice an end-to-end deep learning workflow: data collection, cleaning, normalization, dataset split without leakage, model training, and evaluation. It also matches real-world needs in quantitative research while keeping the scope manageable for a course project.

## Requirements

### 1. Implementation

- Use PyTorch to build and train an LSTM regression model
- Fetch daily prices via Alpha Vantage API
- Build windowed dataset (e.g., past 30 days → next day)
- Build a full pipeline: data → train → validate → predict → plots

### 2. Environment Modification

- Use Python 3.8+ with conda
- Install: numpy, pandas etc libraries
- Save downloaded data as CSV in the project folder
- Provide one notebook that runs end-to-end without manual steps

### 3. Evaluation

- Report MSE and MAE on validation set to measure the error between the actual prices and the predicted prices.
- Plot actual vs predicted for train and validation

### 4. Analysis and Discussion

- Show learning curves (train/val loss) and note overfitting signs
- Explain the impact of different hyperparameters: window size, hidden size, dropout, and learning rate.
- Describe limits: noisy market, missing features, non-stationary data
- Explain what types of stocks this system works best for, and its practical limitations.

### 5. Future Work

- If time allows, add optional improvements:
    - Add volume and technical indicators (e.g., RSI, MACD, moving averages) as additional inputs.
    - Do multi-step forecasting (predict the next 5 or 10 days, not only the next day).
    - Train/test on multiple stocks to check whether the model can generalize.

## Milestones

### 1. Literature Review and Setup

- Read 3–5 LSTM time-series papers/tutorials; set up conda + API access

### 2. Implementation

- Build dataset pipeline + LSTM model; train and save best checkpoint

### 3. Evaluation and Analysis

- Run metrics + plots; compare to baseline; write key findings

### 4. Final Report and Presentation

- Prepare the final report
- Present findings and insights
