#  Market Sentiment vs Trader Behavior Analysis

##  Overview

This project analyzes how Bitcoin market sentiment (Fear/Greed Index) influences trader behavior and performance on Hyperliquid. It combines sentiment data with historical trading activity to uncover patterns in profitability, risk-taking, and trading strategies.

---

##  Project Structure

```
├── data/
│   ├── fear_greed_index.csv
│   ├── historical_data.csv
│   └── merged_data.csv
├── notebook/
│   └── analysis.ipynb
├── requirements.txt
└── README.md
```

---

##  Setup Instructions

### 1. Clone the repository

```
git clone <your-repo-link>
cd <your-project-folder>
```

### 2. Create a virtual environment (recommended)

```
python -m venv venv
```

Activate it:

-> Windows:

```
venv\Scripts\activate
```

-> Mac/Linux:

```
source venv/bin/activate
```

---

### 3. Install dependencies

```
pip install -r requirements.txt
```

If `requirements.txt` is not present, install manually:

```
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

##  How to Run

### Run Data Processing & Analysis

Open and run the notebook:

```
notebook/analysis.ipynb
```

This will:

-> Clean and preprocess data
-> Merge sentiment and trading datasets
-> Generate key metrics and insights
-> Save processed data as:

```
data/merged_data.csv
```

---

## Features:

-> Sentiment vs PnL analysis
-> Win rate and trade behavior insights
->  Risk analysis using trade size (proxy for leverage)
->  Trader segmentation (clustering)
->  Predictive model for next-day profitability
->  Interactive Streamlit dashboard

---

##  Key Insights

* Traders perform best during **Extreme Greed** phases
* Risk-taking increases during **Fear**, but leads to lower efficiency
* Overtrading reduces consistency
* Sentiment strongly influences trading behavior and outcomes

---

##  Strategy Takeaways

* Follow momentum during Greed with controlled risk
* Reduce exposure and avoid overtrading during Fear
* Focus on disciplined and selective trading strategies

---

##  Tech Stack

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn


---

##  Notes

* Trade size (`Size USD`) is used as a proxy for leverage due to lack of explicit leverage data
* Data is aggregated at a daily level for consistency

---

## 👤 Author

Yogita
