# Trade & Ahead | Stock Segmentation with Unsupervised Learning

**Portfolio project:** Financial analytics · Exploratory data analysis · K-means clustering · Hierarchical clustering

## Business question
How can a financial consultancy group stocks by similar financial characteristics to help advisors understand different investment profiles and potential risks?

## Dataset
The supplied `stock_data.csv` contains **340 stocks and 15 columns**, including ticker, sector, stock-price indicators, volatility, profitability, cash-flow measures, and valuation ratios. The data is a project dataset; its observation period and current market applicability are not independently established.

## Approach
1. Explore stock-price, volatility, financial-ratio, and sector patterns.
2. Check duplicates, missing values, and outliers; retain observed extremes and standardize numeric features.
3. Explore K-means cluster counts using elbow and silhouette diagnostics; profile a four-cluster solution.
4. Compare hierarchical linkage methods using dendrograms and cophenetic correlations; profile a four-cluster Ward solution.
5. Compare the clustering approaches and translate group profiles into potential advisory considerations.

## Reported findings in the notebook
The analysis describes four segments: **Core Diversified Large-Caps**, **High-Growth/High-Valuation**, **Energy-Heavy Underperformers**, and **Mega-Cap Blue Chips**. These labels and interpretations are drawn from the author's notebook; they are exploratory group descriptions, **not verified predictions of future investment returns**. The notebook highlights potential risk differences across groups and recommends periodic re-evaluation as financial indicators change.

## Tools
Python, pandas, NumPy, matplotlib, seaborn, scikit-learn, SciPy, Yellowbrick, Jupyter Notebook.

## Run locally
1. Download or clone this repository.
2. Create a Python environment and install dependencies: `pip install -r requirements.txt`.
3. Launch Jupyter: `jupyter notebook`.
4. Open `Trade_Ahead_Stock_Clustering.ipynb` and run the cells in order. Keep `stock_data.csv` in the same folder.

## Files
- `Trade_Ahead_Stock_Clustering.ipynb`: original project analysis, saved under a portfolio-friendly filename
- `stock_data.csv`: supplied project dataset
- `requirements.txt`: Python packages needed to run the analysis
- `README.md`: project overview

## Limitations and responsible interpretation
- Clustering identifies **similarities in selected indicators**, not causal relationships, portfolio suitability, or future returns.
- Grouping stocks into different clusters does **not by itself demonstrate low return correlation or diversification benefit**; this would require return-history and correlation analysis.
- Standardization balances feature scales but does not eliminate the influence of extreme outliers.
- Notebook outputs and conclusions have **not been independently rerun or audited** as part of this packaging step.
- Educational portfolio analysis only; **not investment advice**.
