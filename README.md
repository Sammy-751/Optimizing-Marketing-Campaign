# 📈 Optimizing Market Campaigns: Predicting Term Deposit Subscriptions
### Boosting Campaign Efficiency Through Data-Driven Marketing

![Banner Image – Optional](images/deposit.avif) <!-- Replace with your banner or thematic image -->

---

## Overview
The bank runs large-scale phone campaigns to promote term deposits — but only a small fraction of customers actually subscribe.  
This project develops a predictive model to help the marketing team:

- Better target potential customers  
- Reduce unnecessary calls  
- Increase campaign efficiency and ROI  

---

## Business & Data Understanding

**Stakeholders:**  
Marketing managers and campaign strategists aiming to improve the return on telemarketing efforts.

**Dataset:**  
Direct marketing campaign data from a Portuguese banking institution. Campaigns were conducted via phone calls.  
Clients were contacted multiple times to determine if they would subscribe to a term deposit.

### 💬 Business Questions

- What customer and campaign characteristics most influence subscriptions?  
- Can we use insights to prioritize and reduce unnecessary outreach?  
- Can we accurately predict who will subscribe and use this to guide planning?

![Banner Image – Optional](images/overall%20subs(y).png)

- The chart shows a major imbalance: most clients say "no", and only a small fraction say "yes". This is typical for cold outreach campaigns.
- This imbalance creates two challenges:

  - Models can be biased toward predicting "no" by default

  - A lot of marketing resources may be wasted contacting unlikely prospects
- We used techniques like SMOTE to ensure the model learned to recognize "yes" cases well despite the imbalance.
- The final model focuses on finding the valuable few who are likely to subscribe — helping us reach more of the right people, faster.
---

## 🔬 Modeling Approach

- Algorithms: **Logistic Regression**, **Decision Tree**
- Preprocessing: Encoding, Scaling
- Imbalanced Classes: Handled using **SMOTE**
- Key Features: `duration`, `month`, `previous`, `poutcome`, and others

![Banner Image – Optional](images/Tableau%20Dashboard.png)

---

## 📈 Model Evaluation

| Metric       | Logistic Regression | Decision Tree |
|--------------|---------------------|----------------|
| Accuracy     | 85%                 | 87%            |
| ROC AUC      | 0.89                | 0.82           |
| Precision    | 42%                 | 46%            |
| Recall       | 78%                 | 57%            |

![Banner Image – Optional](images/ROC%20Curve-Logit.png)

- This curve helps us understand how effective the model is at separating likely subscribers from non-subscribers.
- The Area Under the Curve (AUC) is 0.89, which is excellent — it means the model correctly ranks likely "yes" clients 89% of the time.
- In simple terms, the model does a very good job identifying promising leads, helping us avoid wasting time on uninterested clients.
---

## 💡 Key Insights

- Clients with **past successful outcomes** are **9× more likely** to say "yes"
- **March** and **October** had the highest conversion rates
- **Longer call durations** strongly correlated with positive outcomes

![Banner Image – Optional](images/Top%2010%20Features%20per%20Odss-ration.png)


- These top predictors help us understand who is most likely to convert and why. For instance, clients who had subscribed previously, with a successful history, or in October are prime candidates.
- This gives us a clear profile of “high-value” leads we can prioritize in the campaign.

---

##  Conclusion

Using classification models helped identify **high-potential customers**, enabling:

- 📉 Reduced marketing costs
- 🎯 More effective targeting
- 💰 Higher return on investment

---

## Recommendations

- Focus outreach on clients with:
  - **Past successful contact history**
  - **High predicted subscription probabilities**
  - **Engagement in peak months**

---

## Next Steps

- ✅ Integrate predictions into marketing workflow
- 🔁 A/B test targeting strategies
- 🔄 Continuously retrain the model with new campaign data

---

## 📬 Contacts

- **Author:** Sammy Macharia 

- **Email:** [macharias738@gmail.com](mailto:macharias738@gmail.com)

- **LinkedIn:** [linkedin.com/in/Sammy Macharia](https://linkedin.com/in/sammy-macharia)  
- **GitHub:** [github.com/Sammy-751](https://github.com/Sammy-751)

---

> *This project was developed as part of a data science portfolio to demonstrate predictive modeling and business-driven analysis.*

