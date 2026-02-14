# 📉 sales-profitability-analytics

This project analyzes retail sales data to quantify how discounting impacts profitability across product sub-categories and regions.  
The analysis combines Python-based data cleaning, numerical aggregation, visualization, and **AI-assisted reporting using the Groq API** to generate executive-level insights.

---

## 📂 Dataset Overview
- Source: Sample Superstore Dataset
- Total Records: 500+ retail transactions
- Key Fields:
  - Sales, Profit, Discount
  - Order Date, Ship Date
  - Region, Category, Sub-Category

---

## 🧹 Data Cleaning & Feature Engineering
- Evaluated missing data ratio (<5%) and removed incomplete rows
- Converted Order Date and Ship Date to datetime format
- Engineered **Profit Margin (%)** feature
- Ensured numerical consistency for aggregation and visualization

---

## 📊 Numerical Insights & Visual Analysis

### 1️⃣ Profitability by Sub-Category
- **Tables** incur the highest loss of approximately **₹18,000**
- **Bookcases** and **Supplies** also operate at a net loss
- **Copiers** generate the highest profit, exceeding **₹55,000**
- **Phones** and **Accessories** follow with profits above **₹40,000**

📌 Insight:  
High sales volume does not guarantee profitability; pricing strategy plays a critical role.

---

### 2️⃣ The Discount Trap: Discount vs Profit
- Discounts range from **0% to 80%**
- Orders discounted **above 60%** are predominantly loss-making
- Low or zero discount orders show profits reaching **₹8,000+**
- Regression analysis indicates a **negative correlation** between discount and profit

📌 Insight:  
Aggressive discounting erodes margins instead of creating sustainable revenue.

---

## 🔍 Deep-Dive Findings
- Loss-making sub-categories are heavily dependent on high discounts
- Profit variability is significantly higher at lower discount levels
- Regional analysis shows losses concentrated in specific regions for specific products

---

## 🤖 AI-Assisted Executive Reporting (Groq API)
- Used **Groq’s OpenAI-compatible API** to generate an executive summary
- Model leveraged: **LLaMA-3.3-70B (via Groq)**
- AI was used to:
  - Translate numerical loss data into business narratives
  - Identify discount-driven failure patterns
  - Generate region-specific strategic recommendations
- All AI insights are strictly grounded in computed metrics (no synthetic assumptions)

📌 Outcome:  
Groq-powered AI accelerated insight communication while preserving analytical accuracy.

---

## 🧠 Business Recommendations
- Eliminate blanket high-discount strategies
- Reprice or restrict discounts for structurally loss-making sub-categories
- Apply targeted promotions based on margin behavior
- Monitor discount thresholds beyond which profit turns negative

---

## 🛠 Tech Stack
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook
- **Groq API (LLM-powered reporting)**

---

## 📁 Repository Structure
├── Sample - Superstore.csv
├── retail.ipynb
├── profit_analysis.png
├── discount_impact.png
└── README.md

---

## 🚀 Skills Demonstrated
- Data Cleaning & Validation
- Pricing & Profitability Analysis
- Data Visualization & Storytelling
- AI-Augmented Business Reporting (Groq API, LLMs)

---

📌 This project demonstrates how traditional data analytics combined with Groq-powered AI reporting can uncover pricing inefficiencies and improve decision-making speed.
## ▶️ How to Execute the Project
## 1. Clone the Repository
git clone <your-repo-link>
cd sales-profitability-analytics
## 2. Install Dependencies
pip install pandas numpy matplotlib seaborn jupyter
## 3. (Optional) Setup Groq API

Create an account on Groq.

Generate an API key.

Add it to your environment variables:

export GROQ_API_KEY="your_api_key"

(Windows users can use setx GROQ_API_KEY "your_api_key")

## 4. Run the Notebook
jupyter notebook retail.ipynb

Execute all cells to reproduce the cleaning steps, analysis, visualizations, and AI-generated insights.
## 5. View Outputs

Charts will be saved as PNG files.

Review the notebook for detailed numerical analysis and executive summaries.
