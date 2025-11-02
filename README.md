---

# 🧠 ChatGPT Reviews Analysis with Python

## 📘 **Project Overview**

This project focuses on performing **sentiment analysis and review analytics** on user feedback about **ChatGPT**.
By exploring real user reviews, the goal is to uncover how users perceive ChatGPT — what they love, what frustrates them, and how these opinions have changed over time.

Through a combination of **Natural Language Processing (NLP)** and **data visualization**, this project provides valuable insights into user sentiment, recurring themes, and overall satisfaction metrics such as the **Net Promoter Score (NPS)**.

---

## 💡 **Problem Statement**

As ChatGPT’s user base continues to grow, understanding public perception becomes increasingly important for improving user experience and feature development.
However, raw reviews are unstructured and vast — making it difficult to manually extract meaningful insights.

This project addresses the challenge of:

* Automatically classifying reviews by sentiment (positive, neutral, negative),
* Identifying key phrases that users associate with satisfaction or dissatisfaction,
* Tracking how user sentiment evolves over time,
* Quantifying customer loyalty through the NPS metric.

---

## 🎯 **Project Objective**

The main objectives of this project are to:

1. **Perform sentiment analysis** on ChatGPT user reviews using NLP techniques.
2. **Identify and visualize** what users like and dislike most about ChatGPT.
3. **Categorize common problems** and areas needing improvement.
4. **Track sentiment trends** over time to monitor changes in user perception.
5. **Calculate the Net Promoter Score (NPS)** to measure user satisfaction and loyalty.

---

## 🧰 **Tech Stack**

| Category             | Tools/Libraries                          |
| -------------------- | ---------------------------------------- |
| Programming Language | Python                                   |
| Data Manipulation    | Pandas                                   |
| NLP                  | TextBlob, CountVectorizer (Scikit-learn) |
| Visualization        | Plotly (Express & Graph Objects)         |
| Others               | Collections, NumPy                       |

---

## 🗂️ **Dataset Description**

**File:** `chatgpt_reviews.csv`
**Columns:**

* `Review Id` – Unique identifier for each review
* `Review` – Text content of the user review
* `Ratings` – Numerical rating (1–5)
* `Review Date` – Date and time of the review submission

**Data Cleaning:**

* Missing values in the `Review` column were replaced with empty strings.
* `Review Date` was converted to datetime format for trend analysis.

---

## ⚙️ **Project Workflow**

### **1. Data Preprocessing**

* Handled missing values.
* Converted textual and date columns into usable formats.

### **2. Sentiment Analysis**

Used **TextBlob** to assign sentiment polarity:

* Positive (`>0`)
* Neutral (`=0`)
* Negative (`<0`)

Visualized sentiment distribution using a Plotly bar chart.

### **3. Positive Reviews Analysis**

* Extracted most common bi-grams and tri-grams using `CountVectorizer`.
* Identified phrases such as *“great app”*, *“amazing app”*, and *“useful tool”*.

### **4. Negative Reviews Analysis**

* Extracted n-grams from negative reviews to uncover pain points.
* Frequent phrases included *“bad app”*, *“doesn’t work”*, and *“network error”*.

### **5. Problem Categorization**

Grouped negative phrases into broader categories like:

* Incorrect Answers
* App Performance
* User Interface
* Features Missing
* Quality of Responses

### **6. Sentiment Trend Over Time**

* Aggregated monthly sentiment data to track changes in user perception.
* Positive reviews increased sharply around **March–May 2024**, showing growth in satisfaction.

### **7. Net Promoter Score (NPS)**

Calculated NPS using ratings:

* **Promoters:** 5 stars
* **Passives:** 4 stars
* **Detractors:** 1–3 stars

📈 **NPS Score:** `64.35` — indicating strong loyalty and positive user experience.

---

## 📊 **Summary of Insights**

| **Aspect**            | **Insights**                                                                                |
| --------------------- | ------------------------------------------------------------------------------------------- |
| **Overall Sentiment** | Majority of reviews are positive, showing strong user satisfaction.                         |
| **Positive Feedback** | Users appreciate ChatGPT’s usability, educational benefits, and AI capabilities.            |
| **Negative Feedback** | Complaints mainly concern incorrect answers, technical errors, and occasional bugs.         |
| **Common Problems**   | Top issue is *Incorrect Answers*, followed by *App Performance* and *Quality of Responses*. |
| **Trends Over Time**  | Positive sentiment has risen consistently throughout 2024.                                  |
| **NPS Score**         | 64.35 — an excellent indicator of user loyalty.                                             |

---

## 🧩 **Key Visualizations**

* Sentiment Distribution (Positive, Neutral, Negative)
* Top Common Phrases in Positive Reviews
* Top Common Phrases in Negative Reviews
* Common Problems Faced by Users
* Sentiment Trends Over Time

*(All visualizations were created using interactive Plotly charts.)*

---

## 🧠 **Insights and Interpretation**

* ChatGPT enjoys **strong user advocacy** with consistent positive feedback.
* Users love the **AI accuracy**, **educational usefulness**, and **ease of use**.
* However, improvements are needed in **response reliability** and **technical stability**.
* The steady rise in positive reviews suggests **improving user trust and adoption**.

---

## 🏁 **Conclusion**

This analysis demonstrates the power of **data-driven product evaluation**.
By applying sentiment analysis and trend tracking, we gain actionable insights into how users perceive ChatGPT — both its strengths and weaknesses.

A high **Net Promoter Score of 64.35** indicates that ChatGPT not only satisfies most users but also inspires strong recommendations — a sign of excellent product reception.

---

## 🚀 **Future Work**

To enhance this project:

1. Implement **advanced transformer-based sentiment models** (e.g., RoBERTa, BERT).
2. Integrate **topic modeling (LDA)** for deeper theme discovery.
3. Build an **interactive Streamlit dashboard** for real-time review insights.
4. Incorporate **data from multiple platforms** (Play Store, Reddit, etc.).

---
