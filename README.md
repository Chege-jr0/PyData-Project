# 📊 Exploring the Relationship Between Mobile Money and Kenya’s GDP (2007–2024)
## 🧠 Overview
This project investigates the relationship between **Kenya’s Gross Domestic Product (GDP)** and the growth of **mobile money transactions** between **2007 and 2024**.  

Here is a link to my Article : https://chege-paul.hashnode.dev/exploring-the-relationship-between-kenyas-gdp-and-mobile-money-growth-20072024?showSharer=true

With Kenya being the global pioneer of mobile money through M-Pesa and other platforms, this study explores how mobile money adoption may have influenced the country's economic performance.

---

## 🎯 Objectives
- To analyze trends in **GDP** and **mobile money transaction values** over time.  
- To evaluate the **correlation** between the growth of mobile money and GDP.  
- To perform **regression analysis** to determine if mobile money activity significantly affects GDP.  
- To visualize Kenya’s economic trends using **Python data visualization tools**.

---

## 📦 Data Sources
- **World Bank API** — for Kenya’s GDP data (indicator: `NY.GDP.MKTP.CD`)
- **Central Bank of Kenya (CBK)** — for mobile money statistics (active agents, transaction volume, and transaction value)

---

## 🧰 Tech Stack
| Category | Tools / Libraries |
|-----------|-------------------|
| Language | Python 3 |
| Data Analysis | `pandas`, `numpy`, `statsmodels` |
| Visualization | `matplotlib`, `seaborn` |
| Data Source | `wbdata` (World Bank API), CBK CSV dataset |
| Exchange Rate Conversion | `requests` (via ExchangeRate API) |
| Environment | Jupyter Notebook / Google Colab |

---

## 🧩 Data Preparation

1. **Data Collection**
   - GDP data fetched using the World Bank API.
   - Mobile money data loaded from the Central Bank of Kenya CSV file.
2. **Cleaning and Transformation**
   - Converted GDP from USD → KES using real-time exchange rates.
   - Filtered data between **2010 and 2024**.
   - Merged both datasets based on year.
   - Created new derived columns:
     - `GDP_Billions`  
     - `Mobile_Money_Billions`  
     - `GDP_Growth_%`  
     - `Mobile_Money_Growth_%`
3. **Handling Missing Values**
   - Removed null entries using `dropna()`.


## 📈 Analysis Performed

### 1. **Trend Analysis**
Line and bar plots showing the steady growth in mobile money value alongside Kenya’s GDP growth over time.

### 2. **Regression Analysis**
Simple and multiple regression models were used to estimate the influence of mobile money transactions on GDP:
```python
model = sm.OLS(y, X).fit()
print(model.summary())
```
## Key Visuals

📉 Line plot: GDP vs Mobile Money (2007–2024)

📊 Bar plot: GDP vs Mobile Money Value (in billions)

🔍 Regression plot: Relationship between GDP and Mobile Money Value

🧭 3D regression surface: GDP, Active Agents, and Mobile Money Value


## 📊 Results & Insights
A strong positive correlation exists between mobile money transaction values and GDP growth.

Regression analysis shows a statistically significant relationship (p < 0.05).

The 2023 dip in GDP could be attributed to global economic slowdowns, inflationary pressures, and post-pandemic recovery effects, despite continued mobile money growth.

Mobile money remains a key driver of financial inclusion and economic activity in Kenya.

## . Conclusion

The analysis indicates that mobile money has positively impacted Kenya’s GDP, aligning with the broader narrative that digital finance contributes significantly to economic development.
By facilitating transactions, savings, and access to financial services, mobile money has reshaped Kenya’s financial landscape.

## 🚀 Future Work

Include additional economic indicators (e.g., unemployment, inflation, or trade balance)

Perform predictive modeling using machine learning (e.g., linear regression, ARIMA forecasting).

Develop a dashboard using Power BI or Streamlit for real-time data tracking.



## 👨‍💻7. Author

Paul Gikonyo
📍 Nairobi, Kenya

“Turning data into stories that drive understanding and innovati

