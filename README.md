# Retail Sales Analysis with AI

**IBM SkillsBuild – Data Analytics with AI Academic Internship** (BharatCares in association with AICTE)

**Author:** Bavisetti Mamatha

## Project Description
This project analyses retail order data to understand what drives sales and profit. It cleans the data, explores trends with charts, groups customers into behaviour-based segments using **K-Means clustering (RFM analysis)**, and predicts the profit of an order using a **Random Forest regression model**. The project ends with business insights and recommendations.

## Dataset
- **File:** `retail_sales_data.csv` (included in this repository, about 5,000 orders, 2023–2025)
- **Type:** Simulated retail (superstore-style) dataset generated with a fixed random seed (`seed=42`) so results are reproducible. The notebook regenerates the file automatically if it is missing.
- **Columns:** Order_ID, Order_Date, Customer_ID, Segment, Region, Category, Quantity, Unit_Price, Discount, Sales, Profit
- **Data quality:** a few missing values (Region, Discount) and duplicate rows are included on purpose to demonstrate data cleaning.
- **Dataset link:** https://github.com/<your-username>/<your-repo-name>/blob/main/retail_sales_data.csv  *(replace with your repository link after upload)*

## Technologies Used
Python 3, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Jupyter Notebook

## Project Workflow
1. Load the dataset
2. Understand and clean the data (remove duplicates, fix dates, fill missing values, create new features)
3. Exploratory data analysis (monthly trend, category and region performance, discount impact, correlation)
4. Customer segmentation with K-Means on Recency, Frequency and Monetary value
5. Profit prediction with Linear Regression (baseline) and Random Forest
6. Insights and recommendations

## Setup and Run Instructions
```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>

# 2. (Optional) create a virtual environment
python -m venv venv
venv\Scripts\activate        # Windows
source venv/bin/activate     # Mac / Linux

# 3. Install the required libraries
pip install -r requirements.txt

# 4. Open the notebook and run all cells
jupyter notebook Bavisetti_Mamatha_RetailSalesAnalysis.ipynb
```
You can also upload the notebook to **Google Colab** and choose *Runtime → Run all*. No extra setup is needed.

## Key Results
| Item | Result |
|---|---|
| Total sales / profit | 7.51 million / 0.87 million (overall margin 11.55%) |
| Most profitable category | Technology (margin 15.9%); Furniture is lowest (3.7%) |
| Effect of discounts | Orders with 20%+ discount are loss-making 69% of the time vs 1% with no discount |
| Customer segments (K-Means) | Loyal High-Value (297), Regular (372), At-Risk / Inactive (130) |
| Best prediction model | Random Forest, R² = 0.882, MAE = 65.66 (Linear Regression R² = 0.588) |

## Files in this Repository
| File | Purpose |
|---|---|
| `Bavisetti_Mamatha_RetailSalesAnalysis.ipynb` | Complete project code with outputs |
| `requirements.txt` | Python libraries needed |
| `Bavisetti_Mamatha_ProjectReport.docx` | Full project report |
| `retail_sales_data.csv` | Dataset |
| `README.md` | This file |

## Key Information
- Results are reproducible because random seeds are fixed.
- The dataset is simulated for learning purposes; findings illustrate the analysis method and should not be treated as real company data.
