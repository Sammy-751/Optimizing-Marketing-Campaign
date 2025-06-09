
# Optimizing Market Campaigns: Predicting Term Deposit Subscriptions

## 📌 Overview
The bank runs large-scale phone campaigns to promote term deposits. However, only a small fraction of customers subscribe. This project builds a predictive model to help the marketing team better target potential customers, reduce unnecessary calls, and increase the effectiveness of their campaigns.

> 📊 *[Visualization suggestion: Include a graph of total calls vs success rate]*

## 🧠 Business and Data Understanding

**Stakeholders**: Marketing managers and campaign strategists.

**Dataset**: Contains customer profiles, campaign interaction details, and outcomes.

**Business Questions**:
1. What characteristics drive subscription?
2. Can we reduce wasted calls?
3. Can we predict customer responses?

> 📊 *[Visualization: Class imbalance bar chart (yes vs no), feature overview]*

## 🔬 Modeling

- Logistic Regression and Decision Tree were used.
- Data preprocessing included encoding and scaling.
- SMOTE addressed class imbalance.
- Features used: `duration`, `month`, `previous contact`, `poutcome`, and others.

> 📊 *[Visualization: Preprocessing flow, correlation heatmap, tree diagram]*

## 📈 Evaluation

| Metric       | Logistic Regression | Decision Tree |
|--------------|---------------------|----------------|
| Accuracy     | 85%                 | 87%            |
| ROC AUC      | 0.89                | 0.82           |
| Precision    | 42%                 | 46%            |
| Recall       | 78%                 | 57%            |

> 📊 *[Visualization: ROC curves, precision-recall curve, confusion matrix]*

## 💡 Key Insights

- Clients with past successful outcomes → 9x more likely to say yes.
- March and October had highest conversion rates.
- Longer calls correlated strongly with positive outcomes.

> 📊 *[Visualization: Odds ratios bar plot, success rate by month and duration]*

## ✅ Conclusion

Classification helped identify high-potential customers. The model enables:
- Cost reduction in marketing
- Better targeting
- Higher ROI

## 📌 Recommendations

- Prioritize calling clients with:
  - Past successful contact
  - Higher predicted probability scores
  - Interaction in peak months

- Use probability thresholds and lift charts to guide segmentation.

> 📊 *[Visualization: Lift chart, gain chart, customer prioritization by score]*

## 🚀 Next Steps

- Integrate predictions into marketing operations.
- A/B test targeting strategies.
- Continuously retrain with new campaign data.

