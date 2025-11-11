# 🧭 Customer Segmentation & Behavioral Analysis using K-Means

## 📖 Overview
This project applies **unsupervised learning** to perform customer segmentation based on booking and behavioral data.  
By analyzing user activity, cancellations, loyalty, and engagement patterns, the goal is to discover **distinct customer groups** and generate **actionable business insights** for data-driven decision-making.

---

## 🎯 Objectives
- Analyze and preprocess customer booking data  
- Engineer user-level behavioral features  
- Identify natural customer segments using **K-Means clustering**  
- Interpret and visualize clusters for strategic insights  

---

## 🧠 Project Workflow

### **1️⃣ Data Understanding**
- Explored over 100K booking records with multiple attributes  
- Identified key features such as booking frequency, cancellation behavior, lead time, and spending  
- Detected outliers, missing values, and feature correlations  

### **2️⃣ Data Cleaning & Preprocessing**
- Removed invalid or duplicate records  
- Handled missing values in categorical and numerical columns  
- Created additional features such as total nights, total revenue, and promo usage rate  
- Normalized numerical features for consistent scaling  

### **3️⃣ Feature Engineering**
- Aggregated booking-level data into **user-level profiles**  
- Designed hybrid **RFM-like (Recency, Frequency, Monetary)** and behavioral features:  
  - `cancel_rate`, `used_promo_rate`, `booking_changes_mean`, `special_requests_mean`, `engagement_score`, etc.  
- Generated a compact dataset representing user behavior across all bookings  

### **4️⃣ Modelling & Clustering**
- Applied **K-Means** algorithm with `StandardScaler` normalization  
- Determined the optimal number of clusters:  
  - **Elbow Method** → curve flattened after *k = 4*  
  - **Silhouette Score** → peaked at *0.263* (fair separation quality)  
- Trained final model with **4 clusters**, then profiled and visualized cluster characteristics  

---

## 📊 Results & Insights

| Cluster | Segment Name | Behavioral Traits | Strategic Recommendation |
|----------|----------------|------------------|---------------------------|
| **0 – Cancellation-Prone Users** | High cancellation rate (~0.83), low loyalty, long inactivity | Introduce **deposit policy** or **limited-time offers** to reduce cancellations |
| **1 – Regular Users** | Stable behavior, moderate spending, low churn | Maintain retention with **loyalty reminders and periodic discounts** |
| **2 – Active Planners** | High engagement, many booking changes & requests, rare cancellations | Provide **premium options** such as flexible rescheduling or itinerary planning tools |
| **3 – Loyal High-Spenders** | Frequent bookings, high revenue, low cancellation, active recency | Offer **exclusive rewards and membership benefits** to strengthen loyalty |

---

## 📈 Key Visualizations
- **Elbow Curve** → identifies *k = 4* as the optimal cluster count
  <img width="639" height="398" alt="output" src="https://github.com/user-attachments/assets/e78b2ba9-ab7a-4a4b-9020-fb32337324bd" />
- **Silhouette Plot** → confirms good separation between groups
  <img width="626" height="398" alt="output" src="https://github.com/user-attachments/assets/75c989b6-db9b-4ba7-85b9-13dad20926d5" />
- **Cluster Distribution** → shows the majority belong to “Regular Users” segment (~57%)
  <img width="553" height="393" alt="output" src="https://github.com/user-attachments/assets/0eba9eb0-9be9-433f-bb99-529cd4d9afce" />
- **Heatmap Profiling** → highlights behavioral contrasts across clusters
  <img width="785" height="682" alt="output" src="https://github.com/user-attachments/assets/29043e3f-397e-41e9-a1d2-068f28fb39bc" />

---

## 🧩 Tools & Libraries
- **Programming Language:** Python  
- **Core Libraries:** pandas, numpy, scikit-learn, matplotlib, seaborn  
- **Development Environment:** Jupyter Notebook / VS Code  

---

## ✅ Key Takeaways
- Built a complete **unsupervised segmentation pipeline** from data preprocessing to behavioral profiling.  
- Discovered **4 distinct customer personas** with clear business implications.  
- The results can support strategies for:  
  - **Retention and loyalty programs** (for high-value users)  
  - **Reactivation campaigns** (for inactive or high-cancellation users)  
  - **Targeted promotions and personalization**  

---

## 🏁 Future Enhancements
- Deploy interactive **Streamlit dashboard** for dynamic visualization  
- Experiment with advanced clustering algorithms (DBSCAN, GMM, Hierarchical)  
- Integrate transaction history and demographic data for richer segmentation  

---

## 👨‍💻 Author
**Falah Razan Hibrizi**  
Informatics Student @ Telkom University | AI & Data Science Enthusiast  
📍 Bandung, Indonesia  
🔗 [LinkedIn]([https://linkedin.com/in/your-link](https://www.linkedin.com/in/falah-razan-hibrizi-3b36b2280/)) · [GitHub](https://github.com/Frazanhibriz)

---

⭐ **If you find this project insightful, feel free to star or fork it!**
