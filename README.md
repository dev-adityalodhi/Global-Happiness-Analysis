# 🌍 Global Happiness Data Analysis

This project analyzes the **World Happiness Report dataset** to uncover insights about happiness levels across different countries and regions. Using Python, Pandas, NumPy, and Matplotlib, it explores relationships between happiness scores and key socio-economic factors such as GDP, health, and social support.

---

## 🧠 Project Concept

The goal of this project is to understand what influences happiness globally.  
The dataset includes approximately **158 countries**, with metrics such as:

| Column | Description |
|--------|-------------|
| Country | Name of country |
| Happiness Score | Overall happiness level |
| Happiness Rank | Position compared to other countries |
| Economy (GDP per Capita) | Economic wealth indicator |
| Social Support | Support from family/community |
| Healthy Life Expectancy | Expected years of healthy life |
| Freedom | Freedom to make life decisions |
| Generosity | Willingness to help others |
| Perceptions of Corruption | Trust in society & government |

---

## 📦 Technologies Used

- **Python**
- **Pandas** – data handling & cleaning
- **NumPy** – numerical computations
- **Matplotlib** – data visualization

---

## 📊 Key Analysis Performed

- Calculated mean and standard deviation of happiness rank
- Computed correlations:
  - Happiness Rank vs GDP
  - Happiness Rank vs Happiness Score
- Identified:
  - Top 10 happiest countries
  - Bottom 10 least happy countries
  - Best and worst happiness score countries
- Regional happiness comparison
- Generated multiple visualizations

---

## 📈 Visualizations Included

| Chart | Description |
|--------|------------|
| Bar Chart | Average Happiness Score by Region |
| Scatter Plot | Happiness Score vs GDP |
| Bar Chart | Top 10 happiest countries |
| Boxplot | Distribution of Happiness Scores |
| Line Plot | Regional happiness trend |

Plots are saved automatically into a `charts/` folder.

---

## 🧪 Sample Code Used

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

df = pd.read_csv('D:/python/data/happiness.csv')
mean = df['Happiness Rank'].mean()
sd = df['Happiness Rank'].std()

happiness = df['Happiness Rank']
gdp = df['Economy (GDP per Capita)']
score = df['Happiness Score']

corr = np.corrcoef(happiness, gdp)[0, 1]
corr2 = np.corrcoef(happiness, score)[0, 1]

## 📂 Project Structure

Global-Happiness-Analysis/
│
├── happiness.csv
├── charts/
│   ├── happiness_by_region.png
│   ├── happiness_vs_gdp.png
│   ├── happiness_bar.png
│   ├── happiness_boxplot.png
│   └── happiness_plot.png
└── happiness_analysis.py

## 🚀 How to Run
`pip install pandas numpy matplotlib`


Place happiness.csv in your working directory, then run:

python happiness_analysis.py

## 📍 Findings Summary

Countries with higher GDP generally show higher happiness scores.

Regional disparities are visible, with certain regions consistently ranking higher.

Happiness scores vary significantly across the globe.

## 🙌 Future Improvements

Add machine learning models to predict happiness score

Include data for multiple years and analyze trends

Build a dashboard using Streamlit or Tableau

## 📧 Author

Aditya Lodhi
📍 Location
✉️ Email: adityalodhiofficial09@gmail.com

GitHub: https://github.com/dev-adityalodhi

## Thank You


