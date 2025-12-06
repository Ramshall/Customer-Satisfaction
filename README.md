# Customer Satisfaction & Sentiment Analysis Dashboard

## Project Overview
This project analyzes customer feedback from 1,462 users across various ticketing systems (e.g., Zendesk, Zoho Desk, Freshdesk). The goal is to evaluate product performance using standard CX metrics (CSAT, NPS, CES) and enrich the analysis using Natural Language Processing (NLP) to classify unstructured review texts into sentiment categories.

The analysis highlights a significant contrast between high product satisfaction and lower service satisfaction, identifying specific areas for operational improvement.

## Dashboard Preview

### 1. Overview: CX Metrics
![Overview Dashboard](https://github.com/user-attachments/assets/73202ca6-46ea-4547-b02b-c5a4e39651a9)
*Displays Overall CSAT, NPS, and granular scores for Customer Service, Features, and Ease of Use.*

### 2. Customer Sentiment Analysis
![Sentiment Dashboard](https://github.com/user-attachments/assets/765b47e1-2a1b-47d0-a3cb-fc4375408932)
*Displays sentiment trends over time and the distribution of sentiment categories derived from the NLP model.*

---

## Tech Stack & Methodology

* **Python:** Used for data cleaning, preprocessing, and advanced calculation.
    * **Libraries:** Pandas, NumPy.
    * **NLP Model:** Integrated `tabularisai/multilingual-sentiment-analysis` (Pre-trained BERT model from Hugging Face) to classify text reviews into 5 sentiment levels (Very Positive to Very Negative).
* **Power BI:** Used for data visualization and interactive dashboard creation.

---

## Key Insights

Based on the analysis of survey responses and text reviews:

### 1. The "Service Gap" Anomaly
While the **Overall CSAT** is exceptionally high at **91.18%**, a deeper dive reveals a performance gap in **Customer Service**, which scored significantly lower at **67.45%**. In contrast, product-centric attributes like **Ease of Use (89.48%)** and **Features (88.34%)** received high praise. This indicates that users are happy with the tool but frustrated with the human support.

### 2. The "Passive" Trap in NPS
The **Net Promoter Score (NPS)** is relatively low at **11.94%**. This is driven by a dominant **"Passive"** segment (**48%** of users), compared to 32% Promoters and 20% Detractors. This suggests that while customers are not actively dissatisfied, they lack the enthusiasm to advocate for the brand, likely due to the average support experience mentioned above.

### 3. Sentiment Correlation
The NLP analysis validates the numerical scores. Positive and Very Positive sentiments are strongly correlated with product features reviews, whereas Neutral and Negative sentiments frequently appear in contexts related to support responsiveness and ticket handling.

---

## Business Recommendations

To improve customer loyalty and the NPS score, the following actions are recommended:

1.  **Prioritize Support Training:**
    Since Product Features and Ease of Use are already performing well, resources should be shifted to improve the **Customer Service** score (currently 67.45%). Reducing response times and improving ticket resolution quality are critical.

2.  **Activate the "Passive" Segment:**
    With 48% of users sitting in the "Passive" category, there is a massive opportunity for growth. Targeted campaigns that reward loyalty and proactive success management can convert these satisfied-but-quiet users into active Promoters.

3.  **Sentiment-Based Alerting:**
    Implement the NLP model into the live pipeline to flag "Negative" sentiment reviews immediately for the support team, allowing for damage control before a customer churns.
