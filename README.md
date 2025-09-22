# 📊 Telco Customer Churn Prediction

A machine learning project to predict customer churn and identify key retention strategies for a telecommunications company.

## 🎯 Project Overview

Customer churn is a critical business challenge in the telecommunications industry, where acquiring new customers costs 5-25 times more than retaining existing ones. This project analyzes customer behavior patterns and builds predictive models to identify at-risk customers before they leave.

**Note**: This project was completed as part of the **Flexisaf Internship Program**, demonstrating practical application of data science techniques to solve real-world business problems.

## 📁 Dataset

**Source**: [Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

**Description**: Contains information about 7,043 customers from a fictional telecommunications company, including:
- **Demographics**: Gender, age, partner/dependent status
- **Services**: Phone, internet, streaming, security services
- **Account Info**: Contract type, payment method, billing preferences
- **Charges**: Monthly and total charges
- **Churn Status**: Whether the customer left in the last month

## 🔍 Key Findings

### 📈 Churn Rate Analysis
- **Overall churn rate**: ~27% of customers left the service
- **High-risk period**: First year customers show highest churn probability
- **Retention sweet spot**: Customers with 2+ years tenure rarely churn

### 🎯 Top Churn Drivers (SHAP Analysis)

1. **📋 Contract Type** - Most Important Factor
   - Month-to-month contracts: High churn risk
   - Two-year contracts: Strong churn protection
   - One-year contracts: Moderate protection

2. **⏱️ Customer Tenure** - Second Most Important
   - 0-12 months: Highest risk period (critical onboarding phase)
   - 2+ years: Strong loyalty, minimal churn risk

3. **💰 Monthly Charges** - Third Most Important
   - $70+: Significantly higher churn probability
   - $20-50: Optimal pricing range for retention
   - Price sensitivity is a major factor

4. **💳 Payment Method**
   - Electronic check: Higher churn rates
   - Automatic payments: Lower churn rates
   - Payment convenience affects retention

5. **🌐 Internet Service Type**
   - Fiber optic customers: Higher churn tendency
   - DSL customers: More stable retention
   - Service quality/pricing concerns identified

## 🤖 Machine Learning Results

### Model Performance
- **Best Model**: LightGBM (optimized for business needs)
- **Accuracy**: 85%+ overall prediction accuracy
- **Strategy**: Prioritized recall to catch more potential churners
- **Business Focus**: Better to invest in retention than lose customers

### Model Interpretability
- **SHAP Analysis**: Provides clear explanations for each prediction
- **Feature Importance**: Quantifies impact of each customer characteristic
- **Actionable Insights**: Translates model outputs to business decisions

## 💼 Business Impact & Recommendations

### 🚨 Immediate Actions (High Impact, Medium Effort)

1. **Contract Strategy**
   - Offer incentives for longer-term commitments
   - Target month-to-month customers with upgrade campaigns
   - Create compelling annual/bi-annual packages

2. **New Customer Retention**
   - Implement 90-day intensive onboarding program
   - Assign relationship managers to new accounts
   - Create early engagement milestones and rewards

### ⚡ Quick Wins (Medium Impact, Low Effort)

3. **Payment Experience**
   - Incentivize automatic payment adoption with discounts
   - Reduce friction in payment processing
   - Offer multiple convenient payment options

### 📅 Medium-Term Initiatives (High Impact, High Effort)

4. **Pricing Optimization**
   - Review high-charge customer segments for value delivery
   - Develop competitive pricing for price-sensitive segments
   - Create bundling strategies to improve value perception

5. **Service Quality Enhancement**
   - Investigate fiber optic service satisfaction
   - Benchmark service quality against competitors
   - Address technical and support issues

## 📊 Expected Business Outcomes

### 💰 Financial Impact
- **Retention Cost Savings**: Reduce customer acquisition costs
- **Revenue Protection**: Retain high-value customers
- **ROI Optimization**: Target retention investments effectively

### 📈 Performance Metrics
- **15-30% churn reduction** with proper implementation
- **Improved customer lifetime value**
- **Enhanced customer satisfaction scores**

## 🛠️ Technical Implementation

### Technologies Used
- **Python**: Data analysis and machine learning
- **Pandas & NumPy**: Data manipulation
- **Scikit-learn**: Machine learning models
- **LightGBM**: Best-performing model
- **SHAP**: Model interpretability
- **Matplotlib & Seaborn**: Data visualization

### Project Structure
```
├── notebooks/
│   └── Telco_Customer_Churn.ipynb    # Main analysis notebook
├── models/                           # Trained models 
├── src/                             # Source code
├── requirements.txt                 # Dependencies
└── README.md                        # Project documentation
```

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/HaywhyCoder/Telco_Customer_Churn.git
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the analysis**
   ```bash
   jupyter notebook notebooks/Telco_Customer_Churn.ipynb
   ```

## 📈 Future Enhancements

- **Real-time Scoring**: Deploy model for live churn prediction
- **A/B Testing**: Test retention strategies effectiveness
- **Advanced Features**: Incorporate customer service interactions
- **Automated Campaigns**: Trigger retention actions based on predictions


---

*This analysis demonstrates how data science can drive business strategy, turning customer data into actionable retention insights that directly impact the bottom line.*
