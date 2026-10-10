# HW3 — Recurrent Networks for Time Series and Text

**Goal:** Apply sequence models to forecasting and to text classification.

## Part 1 — Crude-oil price forecasting
Forecast daily crude-oil futures prices (WTI, `CL=F`) with four recurrent architectures, evaluated with MAE, MAPE, RMSE and R²:

| Model | MAE | RMSE | R² |
|---|---|---|---|
| RNN | 1.69 | 2.08 | 0.89 |
| LSTM | 1.61 | 1.98 | 0.90 |
| Bi-LSTM | 1.72 | 2.09 | 0.89 |
| **GRU** | **1.33** | **1.67** | **0.93** |

**Bonus:** an explanation of ARIMA vs. SARIMA, and an ARIMA baseline (R² 0.87).

Notebook: [`HW3_Part1_Oil_Price_Forecasting.ipynb`](HW3_Part1_Oil_Price_Forecasting.ipynb)

## Part 2 — Suicidal-intent detection in tweets
Binary classification of tweets (a public Twitter suicidal-intention dataset):
- Text preprocessing, plus a write-up on word embeddings (Word2Vec, GloVe, FastText, contextual embeddings).
- Six models comparing **Word2Vec vs. FastText** embeddings: LSTM, 2-layer LSTM, and CNN + 2-layer LSTM.
- The best test accuracy, **0.88**, comes from LSTM with Word2Vec. Word2Vec generally outperformed FastText.

Notebook: [`HW3_Part2_Suicidal_Tweet_Classification.ipynb`](HW3_Part2_Suicidal_Tweet_Classification.ipynb)
