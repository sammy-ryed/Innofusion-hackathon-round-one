# 🛒 E-Commerce Consumer Behavior Analysis

## 📊 Project Overview

Advanced ML-powered analysis of 1,000 e-commerce customers to predict discount usage patterns and generate actionable business insights through 10 professional visualizations.

---

## 🎯 Key Objectives

- **Predict Discount Usage** using customer behavioral data
- **Identify Key Drivers** of purchasing decisions
- **Generate Visual Insights** for stakeholder presentations
- **Provide Data-Driven Recommendations** for business strategy

---

## 📁 Project Structure

```
📦 E-Commerce Analysis
├── ecommerce_visualizations.ipynb    # Google Colab notebook (10 visualizations)
├── test_improved_models.py           # ML model comparison script
├── Ecommerce_Consumer_Behavior_Analysis_Data.csv
├── outputs/
│   └── visualizations/               # 10 PNG charts
│       ├── viz_age_distribution.png
│       ├── viz_income_vs_purchase.png
│       ├── viz_top10_categories.png
│       └── ... (7 more)
└── BUSINESS_RECOMMENDATIONS.md       # Strategic insights
```

---

## 🚀 Quick Start

### **Option 1: Google Colab (Recommended)**
1. Upload `ecommerce_visualizations.ipynb` to Google Colab
2. Upload dataset when prompted
3. Run all cells → generates 10 visualizations
4. Download ZIP archive with all charts

### **Option 2: Local Python**
```bash
# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn catboost scipy

# Run visualization generator
jupyter notebook ecommerce_visualizations.ipynb

# Or test ML models
python test_improved_models.py
```

---

## 📊 Dataset Features

- **Rows:** 1,000 customers
- **Features:** 27 attributes
  - Demographics: Age, Gender, Income Level, Location
  - Behavioral: Purchase Amount, Frequency, Category
  - Engagement: Social Media Influence, Ad Engagement
  - Loyalty: Program Membership, Satisfaction Score
  - Preferences: Discount Sensitivity, Purchase Intent
- **Target:** `Discount_Used` (Binary: Yes/No)

---

## 🤖 ML Models Tested

| Model | Accuracy | F1-Score | Status |
|-------|----------|----------|--------|
| Baseline Random Forest | 50.5% | 0.552 | Baseline |
| Balanced Random Forest | 50.5% | 0.154 | No improvement |
| SMOTE + Random Forest | **51.5%** | **0.565** | Best |
| CatBoost | 51.5% | 0.531 | Tied best |

**Key Findings:**
- ✅ Removed feature leakage (`Total_Spend`)
- ⚠️ Models perform near random baseline (50-52%)
- 🔍 Discount usage appears weakly correlated with available features
- 💡 Suggests need for external data or different modeling approach

---

## 🎨 10 Generated Visualizations

1. **Age Distribution** — Customer demographics with KDE overlay
2. **Income vs Purchase** — Box plots + average spend by income tier
3. **Top 10 Categories** — Frequency & spending by product category
4. **Channel Breakdown** — Purchase channel distribution (donut + bar)
5. **Satisfaction Heatmap** — Satisfaction × Income correlation
6. **Loyalty Spending** — Members vs non-members comparison
7. **Social Media Influence** — Impact on purchase behavior
8. **Discount Sensitivity** — Usage patterns & spend comparison
9. **Confusion Matrix** — Model performance metrics
10. **Feature Importance** — Top 15 predictive features (CatBoost)

**All charts use professional dark theme** with consistent color palette.

---

## 📈 Key Insights

### **Customer Segmentation**
- **Age:** Broad distribution (18-70), median ~44 years
- **Income:** Balanced across Low/Middle/High tiers
- **Loyalty:** ~48% enrolled in loyalty program

### **Purchase Behavior**
- **Average Purchase:** $272
- **Top Categories:** Electronics, Clothing, Home Goods
- **Channels:** Online dominates (65%), followed by in-store (25%)

### **Discount Patterns**
- **52.1%** of customers use discounts regularly
- **High sensitivity** customers show 85% discount usage rate
- **Social media influence** has moderate impact on purchasing

### **Model Performance**
- **Weak predictive power** suggests discount usage is largely behavioral/external
- **Top features:** Purchase Amount, Age, Frequency, Income Level
- **Recommendation:** Collect additional data (browsing history, email engagement)

---

## 💼 Business Applications

1. **Marketing Campaigns** — Target high-sensitivity segments with personalized offers
2. **Inventory Planning** — Stock popular categories based on purchase patterns
3. **Channel Strategy** — Optimize online experience (primary channel)
4. **Loyalty Programs** — Redesign to increase member engagement & spending
5. **Pricing Strategy** — Use insights for dynamic pricing and promotion timing

---

## 🔧 Technical Stack

- **Python 3.11+**
- **Data:** pandas, numpy
- **ML:** scikit-learn, imbalanced-learn, CatBoost
- **Viz:** matplotlib, seaborn
- **Stats:** scipy

---

## 📝 Next Steps

### **To Improve Model Accuracy (50% → 70%+):**
1. **Feature Engineering** — Create interaction terms, time-based features
2. **External Data** — Add browsing history, email clicks, cart abandonment
3. **Advanced Algorithms** — Try AutoML (TPOT, mljar-supervised)
4. **Ensemble Stacking** — Combine multiple models
5. **Hyperparameter Tuning** — GridSearchCV optimization

### **For Business Impact:**
- Implement A/B testing based on discount sensitivity segments
- Deploy real-time prediction API for personalized offers
- Create dashboard for marketing team (Tableau/Power BI)

---

## 👥 Team Structure

**For Hackathon Presentation:**
- **Member 1 (Data Engineer):** Data cleaning, preprocessing, feature engineering
- **Member 2 (ML Engineer):** Model development, evaluation, optimization
- **Member 3 (Analyst):** Visualizations, insights, business recommendations

---

## 📄 License

MIT License — Free for educational and commercial use

---

## 🎉 Results Summary

✅ **10 professional visualizations** generated  
✅ **4 ML models** tested and compared  
✅ **Business recommendations** documented  
✅ **Google Colab ready** for presentation  
✅ **Reproducible pipeline** with clear documentation  

**Project Status:** ✅ Complete and presentation-ready!

---

*For detailed business recommendations, see [BUSINESS_RECOMMENDATIONS.md](BUSINESS_RECOMMENDATIONS.md)*
