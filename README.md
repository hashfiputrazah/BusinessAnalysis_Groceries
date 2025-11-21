# 🛒 Market Basket Analysis - Groceries Dataset

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.2.3-green.svg)](https://pandas.pydata.org/)
[![mlxtend](https://img.shields.io/badge/mlxtend-0.23.4-orange.svg)](http://rasbt.github.io/mlxtend/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> Mengungkap pola belanja tersembunyi menggunakan Association Rule Mining dengan algoritma Apriori

![MBA Banner](https://img.shields.io/badge/Data%20Science-Market%20Basket%20Analysis-red?style=for-the-badge)

---

## 📋 Overview

Proyek end-to-end **Market Basket Analysis** untuk menemukan produk yang sering dibeli bersamaan oleh pelanggan toko groceries. Analisis ini bertujuan untuk:

- 📈 Meningkatkan **Average Basket Size**
- 🎁 Menemukan pola **bundling produk** yang efektif  
- 🏪 Memberikan rekomendasi **penempatan barang** (Store Layout)
- 🎯 Mengoptimalkan **strategi promosi** berbasis data

---

## 📊 Dataset

| Metric | Value |
|--------|-------|
| Total Records | 38,765 |
| Unique Transactions | 14,963 |
| Unique Products | 167 |
| Date Range | 2014 - 2015 |

**Source:** [Kaggle - Groceries Dataset](https://www.kaggle.com/datasets/heeraldedhia/groceries-dataset)

---

## 🔍 Key Findings

### Top Association Rules (by Lift)

| Antecedents | Consequents | Support | Confidence | Lift |
|-------------|-------------|---------|------------|------|
| Whole Milk, Yogurt | Sausage | 0.001 | 13.2% | **2.183** |
| Whole Milk, Sausage | Yogurt | 0.001 | 16.4% | **1.912** |
| Specialty Chocolate | Citrus Fruit | 0.001 | 8.8% | **1.654** |
| Yogurt, Sausage | Whole Milk | 0.001 | 25.6% | **1.620** |
| Flour | Tropical Fruit | 0.001 | 11.0% | **1.617** |

### 💡 Key Insight
> Pelanggan yang membeli **Whole Milk + Yogurt** memiliki kemungkinan **2.18x lebih tinggi** untuk juga membeli **Sausage** — pola "Breakfast Trio" yang sempurna untuk bundling!

---

## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| Language | Python 3.x |
| Data Manipulation | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Association Rules | mlxtend (Apriori) |
| Dashboard | Looker Studio |

---

## 📁 Project Structure

```
📦 Market-Basket-Analysis
├── 📄 Groceries_dataset.csv        # Raw dataset
├── 📓 MBA_Analysis.ipynb           # Main analysis notebook
├── 📊 MBA_Groceries_Result.csv     # Association rules output
├── 📈 visualizations/              # Charts and plots
└── 📖 README.md
```

---

## 🚀 Quick Start

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn mlxtend
```

### Run Analysis
```python
# Clone repository
git clone https://github.com/yourusername/market-basket-analysis.git

# Navigate to directory
cd market-basket-analysis

# Run Jupyter Notebook
jupyter notebook MBA_Analysis.ipynb
```

---

## 📈 Methodology

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│  Data Loading   │ -> │  Preprocessing  │ -> │      EDA        │
│  & Inspection   │    │  & Cleaning     │    │                 │
└─────────────────┘    └─────────────────┘    └─────────────────┘
                                                      │
                                                      ▼
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│    Business     │ <- │   Evaluation    │ <- │    Modeling     │
│ Recommendations │    │   & Insights    │    │   (Apriori)     │
└─────────────────┘    └─────────────────┘    └─────────────────┘
```

---

## 📊 Dashboard

Explore the interactive dashboard:

🔗 **[View on Looker Studio](https://lookerstudio.google.com/s/sIqQGQnY7pY)**

---

## 💼 Business Recommendations

Based on the analysis:

1. **🎁 Bundling Strategy** — Create "Breakfast Trio" package (Milk + Yogurt + Sausage)
2. **🏪 Store Layout** — Cross-merchandise sausage near dairy section
3. **📱 Targeted Marketing** — Trigger personalized recommendations based on cart contents
4. **📦 Inventory Management** — Maintain synchronized stock for high-lift product combinations

---

## 👤 Author

**Hashfi Putraza Hikmat**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin)](https://linkedin.com/in/yourprofile)
[![Medium](https://img.shields.io/badge/Medium-Follow-black?style=flat&logo=medium)](https://medium.com/@yourprofile)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## ⭐ Support

If you find this project useful, please consider giving it a star!

[![Star History](https://img.shields.io/github/stars/yourusername/market-basket-analysis?style=social)](https://github.com/yourusername/market-basket-analysis)

---

*Made with ❤️ and Python*
