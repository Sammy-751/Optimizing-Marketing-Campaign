# 📈 Optimizing Market Campaigns: Predicting Term Deposit Subscriptions

## 📌 Overview
The bank runs large-scale phone campaigns to promote term deposits — but only a small fraction of customers actually subscribe.  
This project develops a predictive model to help the marketing team:

- Better target potential customers  
- Reduce unnecessary calls  
- Increase campaign efficiency and ROI  

---

## 🧠 Business & Data Understanding

**Stakeholders:**  
Marketing managers and campaign strategists aiming to improve the return on telemarketing efforts.

**Dataset:**  
Direct marketing campaign data from a Portuguese banking institution. Campaigns were conducted via phone calls.  
Clients were contacted multiple times to determine if they would subscribe to a term deposit.

### 💬 Business Questions

- What customer and campaign characteristics most influence subscriptions?  
- Can we use insights to prioritize and reduce unnecessary outreach?  
- Can we accurately predict who will subscribe and use this to guide planning?

📊 *[Visualization: Class imbalance bar chart (yes vs no), feature overview]*

---

## 🔬 Modeling Approach

- Algorithms: **Logistic Regression**, **Decision Tree**
- Preprocessing: Encoding, Scaling
- Imbalanced Classes: Handled using **SMOTE**
- Key Features: `duration`, `month`, `previous`, `poutcome`, and others

📊 *[Visualization: Preprocessing pipeline, correlation heatmap, decision tree diagram]*

---

## 📈 Model Evaluation

| Metric       | Logistic Regression | Decision Tree |
|--------------|---------------------|----------------|
| Accuracy     | 85%                 | 87%            |
| ROC AUC      | 0.89                | 0.82           |
| Precision    | 42%                 | 46%            |
| Recall       | 78%                 | 57%            |

📊 *[Visualization: ROC curves, Precision-Recall curve, Confusion matrix]*

---

## 💡 Key Insights

- Clients with **past successful outcomes** are **9× more likely** to say "yes"
- **March** and **October** had the highest conversion rates
- **Longer call durations** strongly correlated with positive outcomes

📊 *[Visualization: Odds ratios bar plot, success rate by month and duration]*

---

## ✅ Conclusion

Using classification models helped identify **high-potential customers**, enabling:

- 📉 Reduced marketing costs
- 🎯 More effective targeting
- 💰 Higher return on investment

---

## 📌 Recommendations

- Focus outreach on clients with:
  - **Past successful contact history**
  - **High predicted subscription probabilities**
  - **Engagement in peak months**

- Use **probability thresholds** and **lift/gain charts** for smarter segmentation.

📊 *[Visualization: Lift chart, Gain chart, customer ranking]*

---

## 🚀 Next Steps

- ✅ Integrate predictions into marketing workflow
- 🔁 A/B test targeting strategies
- 🔄 Continuously retrain model with new campaign data

---

## 📬 Contacts

**Author:** Your Name  
**Email:** your.email@example.com  
**LinkedIn:** [linkedin.com/in/your-profile](https://linkedin.com/in/your-profile)  
**GitHub:** [github.com/yourusername](https://github.com/yourusername)

---

> *This project was developed as part of a data science portfolio to demonstrate predictive modeling and business-driven analysis.*

