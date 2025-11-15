<h1 align="center">🧭 Customer Segmentation & Behavioral Analysis using K-Means</h1>

<p align="center">
  <b>Unsupervised Learning Project · Python · Data Science</b><br>
  Discover behavioral clusters from hotel booking patterns using K-Means
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Machine%20Learning-KMeans-blue?style=flat-square&logo=scikit-learn" />
  <img src="https://img.shields.io/badge/Python-3.10%2B-yellow?style=flat-square&logo=python" />
  <img src="https://img.shields.io/badge/VSCode-Editor-blueviolet?style=flat-square&logo=visualstudiocode" />
  <img src="https://img.shields.io/badge/Status-Completed-success?style=flat-square" />
</p>

---

## 📖 Overview
This project applies **unsupervised learning** to perform customer segmentation based on hotel booking and behavioral data.  
By analyzing patterns such as cancellations, loyalty, and engagement, it identifies **distinct customer groups** and generates **data-driven business insights** to support marketing and retention strategies.

---

## 🎯 Objectives
- Analyze and preprocess customer booking data  
- Engineer user-level behavioral features  
- Identify natural customer segments using **K-Means clustering**  
- Interpret and visualize clusters for **strategic decision-making**

---

## 🧠 Project Workflow

### **1️⃣ Data Understanding**
- Explored **100K+ booking records**
- Identified key features: booking frequency, cancellations, lead time, spending
- Detected missing values, outliers, and feature correlations  

### **2️⃣ Data Cleaning & Preprocessing**
- Removed invalid or duplicate records  
- Imputed missing values (categorical & numerical)  
- Created new features (`total_revenue`, `promo_rate`, `avg_stay_nights`)  
- Normalized data using **StandardScaler**

### **3️⃣ Feature Engineering**
- Aggregated booking-level data → **user-level profiles**  
- Built hybrid **RFM-style (Recency, Frequency, Monetary)** metrics and behavioral scores  
- Key features:  
  - `cancel_rate`, `booking_changes_mean`, `special_requests_mean`, `loyalty_index`, `engagement_score`

### **4️⃣ Modeling & Clustering**
- Algorithm: **K-Means (k=4)**  
- Evaluation:  
  - **Elbow Method:** curve stabilized after *k=4*  
  - **Silhouette Score:** *0.263 → fair separation quality*  
- Profiling and visualization conducted for each cluster

---

## 📊 Results & Insights

| Cluster | Segment Name | Behavioral Traits | Strategic Recommendation |
|:--------|:--------------|:------------------|:--------------------------|
| **0 – Cancellation-Prone Users** | High cancellation rate (~0.83), low loyalty, long inactivity | Introduce **deposit policy** or **limited-time offers** to reduce cancellations | Encourage **re-activation** through special incentives or stricter booking commitments |
| **1 – Regular Users** | Stable behavior, moderate spending, low churn | Maintain retention with **loyalty reminders** and **periodic discounts** | Strengthen loyalty with **tiered point programs** and **personalized deals** |
| **2 – Active Planners** | High engagement, many booking changes & requests, rare cancellations | Provide **premium options** such as flexible rescheduling or itinerary planning tools | Upsell **priority support** and **exclusive travel perks** |
| **3 – Loyal High-Spenders** | Frequent bookings, high revenue, low cancellation, active recency | Offer **exclusive rewards** and **membership benefits** to strengthen loyalty | Focus on **retention & cross-sell campaigns** (e.g., bundles, upgrades) |

---

## 📈 Key Visualizations

| Visualization | Description |
|:--------------|:-------------|
| 🧩 **Elbow Curve** | Optimal number of clusters (k=4) |
| 🎭 **Silhouette Score Plot** | Shows inter-cluster separation quality |
| 👥 **Cluster Distribution** | Majority are “Regular Users” (~57%) |
| 🔥 **Heatmap Profiling** | Visual contrast between engagement, loyalty, and cancellations |

<p align="center">
  <img width="600" src="https://github.com/user-attachments/assets/e78b2ba9-ab7a-4a4b-9020-fb32337324bd" alt="Elbow Curve" />
  <img width="600" src="https://github.com/user-attachments/assets/75c989b6-db9b-4ba7-85b9-13dad20926d5" alt="Silhouette Plot" />
  <img width="600" src="https://github.com/user-attachments/assets/0eba9eb0-9be9-433f-bb99-529cd4d9afce" alt="Cluster Distribution" />
  <img width="700" src="https://github.com/user-attachments/assets/29043e3f-397e-41e9-a1d2-068f28fb39bc" alt="Heatmap Profiling" />
</p>

---

## 🧩 Tech Stack
| Category | Tools |
|:----------|:------|
| 💻 Language | Python (v3.10+) |
| 📦 Libraries | pandas, numpy, scikit-learn, matplotlib, seaborn |
| 🧠 ML Technique | K-Means Clustering |
| 🧰 Environment | Jupyter Notebook, VS Code |

---

## ✅ Key Takeaways
- Built a complete **unsupervised segmentation pipeline**  
- Identified **4 clear customer personas** with distinct engagement patterns  
- Derived actionable insights for:  
  - 🌀 Reactivation campaigns  
  - 🎯 Loyalty enhancement  
  - 💡 Cross-sell & personalization strategies  

---

## 🚀 Future Enhancements
- Deploy **Streamlit dashboard** for interactive analysis  
- Explore advanced clustering (DBSCAN, GMM, Hierarchical)  
- Integrate demographic or transactional data for deeper insights  

---

## 👨‍💻 Author
**Falah Razan Hibrizi**  
Informatics Student @ Telkom University · AI & Data Science Enthusiast  
📍 Bandung, Indonesia  
🌐 [LinkedIn](https://www.linkedin.com/in/falah-razan-hibrizi-3b36b2280/) · [GitHub](https://github.com/Frazanhibrizi)

---

## 🔗 Related Project

This repository contains the complete data preprocessing, feature engineering, and customer segmentation workflow.

For the interactive Streamlit dashboard version of this project, visit:  
👉 **Customer Segmentation Dashboard**  
https://github.com/Frazanhibriz/customer_segmentation_dashboard/tree/main

---

<p align="center">
  ⭐ <b>If you find this project insightful, feel free to star or fork it!</b> ⭐  
</p>
