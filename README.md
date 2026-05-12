# Financial News Exploratory Data Analysis (EDA)

## Project Overview

This project focuses on Exploratory Data Analysis (EDA) of a financial news dataset. The objective is to analyze textual and temporal patterns in financial news headlines using Python, data analysis libraries, and Natural Language Processing (NLP) techniques.

The project includes:

* Descriptive statistical analysis
* Publisher activity analysis
* Keyword and topic extraction
* Time series analysis of news publication frequency
* Data visualization
* GitHub version control and CI/CD workflow setup

---

# Repository Structure

```text
financial-news-eda/
│
├── .github/
│   └── workflows/
│       └── unittests.yml
│
├── notebooks/
│   └── EDA.ipynb
│
├── data/
│   └── news.csv
│
├── requirements.txt
├── README.md
```

---

# Task-1 Objectives

The following tasks were completed:

* Created GitHub repository
* Created `task-1` branch
* Configured Python virtual environment
* Added `requirements.txt`
* Configured GitHub Actions CI/CD workflow
* Performed Exploratory Data Analysis (EDA)
* Conducted text analysis using NLP techniques
* Performed publisher analysis
* Conducted time-series analysis of publication frequency
* Created data visualizations
* Used descriptive Git commit messages following Conventional Commits

---

# Technologies Used

## Programming Language

* Python 3.11

## Libraries

* pandas
* numpy
* matplotlib
* seaborn
* scikit-learn
* nltk
* jupyter

---

# Environment Setup

## Clone Repository

```bash
git clone <repository_link>
cd financial-news-eda
```

## Create Virtual Environment

### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

# Running the Notebook

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
notebooks/EDA.ipynb
```

---

# Exploratory Data Analysis

The notebook includes the following analyses:

## 1. Descriptive Statistics

* Headline length distribution
* Statistical summary of text length
* Publisher article counts

## 2. Publisher Analysis

* Most active publishers
* Publisher contribution comparison
* Email domain extraction and analysis

## 3. Text Analysis

* Common keyword extraction
* TF-IDF and CountVectorizer analysis
* Topic identification from financial headlines

## 4. Time Series Analysis

* Publication frequency over time
* Daily news volume trends
* Publishing hour analysis
* Spike identification during major market events

---

# Visualizations

The notebook includes at least three visualizations:

1. Publisher activity bar chart
2. News publication frequency over time
3. Headline keyword frequency visualization

---

# GitHub Actions CI/CD

The project uses GitHub Actions for Continuous Integration.

Workflow file location:

```text
.github/workflows/unittests.yml
```

The workflow automatically:

* Checks repository updates
* Sets up Python environment
* Installs dependencies from `requirements.txt`

---

# Example Commit Messages

Conventional commit examples used in this project:

```bash
feat: add exploratory data analysis notebook
feat: add publisher analysis visualization
feat: implement topic modeling using CountVectorizer
ci: configure github actions workflow
docs: update project README
```

---

# Key Insights

Some important findings from the analysis include:

* Certain publishers contribute significantly more financial news articles.
* News publication frequency changes over time and may spike around important financial events.
* Common financial topics include earnings reports, market forecasts, FDA approvals, and stock price targets.
* Publishing activity varies depending on the time of day.

---

# Author

Yordanos Birhanu

---

# License

This project is developed for educational and research purposes.
## Task 2: Quantitative Analysis

In this section, I implemented technical analysis using TA-Lib to extract market signals from financial data.

### Technical Indicators Used:
- Simple Moving Average (SMA 20 & 50)
- Relative Strength Index (RSI)
- MACD (Moving Average Convergence Divergence)
- Bollinger Bands

### Objective:
To analyze stock trends, momentum, and volatility using quantitative indicators.
