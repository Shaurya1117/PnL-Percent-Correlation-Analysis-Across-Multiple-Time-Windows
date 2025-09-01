# PnL-Percent-Correlation-Analysis-Across-Multiple-Time-Windows
Correlation analysis of PnL percentage metrics across multiple time windows using Python (Pandas, NumPy, Seaborn).

# PnL Percent Correlation Analysis Across Multiple Time Windows

This project analyzes the correlations between profit & loss (PnL) percentage metrics across different time windows (e.g., `:120:`) using Python.  
The goal is to uncover dependencies among trading performance indicators that can support financial strategy evaluation and risk analysis.

---

## 📌 Overview
- Filters PnL percentage columns (`:pnlPercent`) for specific time windows
- Computes **Pearson correlation** matrices between features
- Generates visualizations (heatmaps) to highlight strong/weak relationships
- Demonstrates exploratory financial data analysis in **Google Colab**

---

## ⚙️ Technologies Used
- **Python**  
- **Pandas, NumPy** – data manipulation & numerical computing  
- **Matplotlib, Seaborn** – visualization  
- **Google Colab** – notebook execution environment  

---

## 📊 Dataset
- The **original dataset (`ivs3.feather`) is ~2.7 GB** and **not included** in this repository.  
- To run this notebook, upload your own dataset to **Google Drive** and mount it in Colab:
  ```python
  from google.colab import drive
  drive.mount('/content/drive')

  import pandas as pd
  file_path = '/content/drive/MyDrive/ivs3.feather'
  df = pd.read_feather(file_path)
