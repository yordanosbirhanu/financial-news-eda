# Financial News and Stock Market Analysis

## Project Overview

This project analyzes the relationship between financial news sentiment and stock market behavior using Exploratory Data Analysis (EDA), technical analysis indicators, and statistical correlation methods.

The project is divided into three major tasks:

- Task 1: Exploratory Data Analysis (EDA) of financial news
- Task 2: Quantitative stock analysis using TA-Lib and PyNance
- Task 3: Correlation analysis between news sentiment and stock price movements

The project uses Python, Pandas, NLP techniques, TA-Lib, and statistical analysis to explore financial news trends and their impact on stock returns.

---

# Project Structure

```text
financial-news-eda/
│
├── .github/
│   └── workflows/
│       └── unittests.yml
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── task1_eda.ipynb
│   ├── task2_quantitative_analysis.ipynb
│   └── task3_sentiment_correlation.ipynb
│
├── src/
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- NLTK
- VADER Sentiment Analyzer
- TA-Lib
- PyNance
- Scikit-learn
- Git & GitHub
- GitHub Actions

---

# Task 1: Exploratory Data Analysis (EDA)

## Objective

The objective of Task 1 was to explore and understand the financial news dataset using descriptive statistics, NLP techniques, and time-series analysis.

---

## Activities Performed

### Environment and Version Control Setup

- Created GitHub repository
- Created `task-1` branch
- Configured Python virtual environment
- Added `requirements.txt`
- Configured GitHub Actions CI/CD workflow
- Used descriptive Git commit messages

---

## Descriptive Statistics

The following analyses were performed:

- Headline character length distribution
- Average headline length
- Article counts per publisher
- Publication trends over time
- Missing value analysis

---

## Text Analysis and Topic Modeling

Natural Language Processing (NLP) techniques were used to identify important keywords and recurring topics in financial headlines.

Methods used:

- CountVectorizer
- TF-IDF
- Word frequency analysis

Common financial themes identified included:

- Earnings reports
- FDA approvals
- Price target changes
- Market forecasts
- Stock upgrades and downgrades

---

## Time Series Analysis

Publication frequency was analyzed over time to identify:

- News volume spikes
- Daily publication trends
- Publishing behavior during major market events

Publishing hours were also analyzed to determine peak news release times.

---

## Publisher Analysis

The most active publishers were identified and compared.

Additional analysis included:

- Publisher contribution frequency
- Extraction of email domains from publisher names
- Organizational activity patterns

---

## Key Visualizations

Task 1 included multiple visualizations such as:

- Headline length distribution
- Top publishers bar chart
- News publication frequency over time
- Word frequency visualization

---

# Task 2: Quantitative Analysis Using TA-Lib and PyNance

## Objective

The objective of Task 2 was to analyze stock market behavior using technical indicators and financial metrics.

---

## Data Preparation

The stock datasets were loaded and cleaned using Pandas.

Steps included:

- Data type correction
- Missing value handling
- Date formatting
- Sorting by trading date

The following stock datasets were analyzed:

- AAPL
- AMZN
- GOOG
- META
- MSFT

---

## Technical Indicators Computed

### Moving Averages

- Simple Moving Average (SMA)
- Exponential Moving Average (EMA)

Multiple window sizes were analyzed to identify trend direction.

---

### Relative Strength Index (RSI)

RSI was used to identify:

- Overbought conditions
- Oversold conditions

---

### MACD (Moving Average Convergence Divergence)

MACD analysis was used to identify:

- Momentum shifts
- Trend reversals
- Bullish and bearish signals

---

## Financial Metrics with PyNance

PyNance was used to compute additional financial metrics beyond standard technical indicators.

---

## Visualizations

Task 2 visualizations included:

- Closing prices with SMA and EMA overlays
- RSI charts
- MACD plots
- Trend visualization charts

---

# Task 3: Correlation Between News Sentiment and Stock Movement

## Objective

The objective of Task 3 was to investigate the relationship between financial news sentiment and daily stock returns.

---

## Date Alignment

News publication dates were aligned with stock trading days.

Special handling was implemented for:

- Weekends
- Holidays
- Non-trading days

News articles published outside trading days were aligned to the next valid trading day.

---

## Sentiment Analysis

Sentiment analysis was performed using the VADER sentiment analyzer from NLTK.

### Why VADER?

VADER was selected because:

- It performs well on short text
- It is effective for headline sentiment analysis
- It generates normalized sentiment scores between -1 and +1

Each headline received a compound sentiment score.

---

## Daily Stock Returns

Daily stock returns were calculated using:

\[
\frac{Close_t - Close_{t-1}}{Close_{t-1}} \times 100
\]

This allowed direct comparison between sentiment and market performance.

---

## Correlation Analysis

The following analyses were performed:

- Average daily sentiment calculation
- Pearson correlation analysis
- Scatter plot visualization
- Sentiment category analysis

Days were classified as:

- Positive
- Neutral
- Negative

Average daily returns were compared across these sentiment categories.

---

## Key Findings

The analysis identified weak-to-moderate relationships between financial news sentiment and stock returns depending on the company analyzed.

Positive news sentiment generally corresponded with positive stock returns, though the relationship was not consistently strong across all stocks.

---

## Limitations

Several limitations were identified:

- Financial markets are influenced by many external factors
- News sentiment effects may appear with delays
- Headlines may not fully represent article meaning
- Sentiment models may misinterpret financial language

---

# How to Run the Project

## Clone Repository

```bash
git clone <your-repository-url>
```

---

## Create Virtual Environment

### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

### Linux/Mac

```bash
python3 -m venv venv
source venv/bin/activate
```

---

## Install Requirements

```bash
pip install -r requirements.txt
```

---

## Run Jupyter Notebook

```bash
jupyter notebook
```

Open notebooks from the `notebooks/` directory.

---

# Git Workflow

Branches used:

- `main`
- `task-1`
- `task-2`
- `task-3`

Development followed Git best practices using:

- Pull Requests (PR)
- Feature branches
- Descriptive commit messages
- Continuous Integration with GitHub Actions

---

# Results Summary

This project successfully:

- Explored financial news datasets using EDA
- Computed technical indicators using TA-Lib
- Applied NLP-based sentiment analysis
- Investigated relationships between sentiment and stock movement
- Visualized stock market trends and sentiment correlations

---

# Author

Yordanos Birhanu
