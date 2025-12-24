# 🚗 Automotive Market Segmentation and Consumer Insights (Dangchedi Platform)  

---

## 📌 Project Background

This project analyzes consumer attention and market segmentation in China’s automotive industry using data from the **Dangchedi platform**. By applying clustering and decision tree models, the study aims to break the deadlock of ambiguous segmentation and uncover the drivers behind high-potential vehicle models.  

---

## 💡 Business Goals

- Clarify blurred market segment boundaries
- Identify high-potential models and their drivers
- Provide actionable insights for automakers and platforms  

---

## 🛠 Tech Stack

- **Language**: Python  
- **Libraries**: pandas, numpy, scikit-learn, matplotlib, seaborn, requests  
- **Methods**: Web scraping, Data cleaning, Clustering (K-means + PCA), Decision Tree  

---

## 📊 Data

- **Source**: Dangchedi web interface `/motor/pc/car/rank_data`  
- **Dataset**: 743 valid vehicle entries (`dongchedi_rank_data.csv`)  
- **Features**: Vehicle series, brand, min/max price, user engagement count, score, rank  
- **Usage**: Cleaning → Clustering → Decision Tree  

---

## 📈 Visualization

- Correlation Matrix: Price range vs. popularity  
- Quadrant Analysis: Price distribution, popularity distribution, rank histogram, brand coverage  
- Key Insight: Most popular models are **new energy vehicles**, showing rising consumer interest in EVs  

---

## 🔍 Cluster Analysis

- Optimal K = 3 (tested with silhouette coefficient)  
- **Group 1 (56%)**: Low price, low attention (Honda, Wuling)  
- **Group 2 (23%)**: Low price, high attention (BYD, Toyota)  
- **Group 3 (20%)**: Mid-to-high price, high attention (Audi, Denza)  

---

## 🧭 Business Suggestion

- Platforms: Stratified user operations, targeted promotion  
- Automakers: Focus resources on high-potential segments  
- Brands: Clarify positioning and optimize competitive strategies  

---

## 🌳 Decision Tree
- **Core Features**: Brand type (mainstream vs. others), Minimum price  
- **Key Rules**:  
  1. Min price ≤ 139k + mainstream brand → High Attention (Coverage 68.9%)  
  2. Min price ≤ 139k + other brand → Low Attention (Coverage 53.5%)  
  3. Min price > 452k → Low Attention (Coverage 100%)  
- **Business Value**:
  - Quickly screen promotional models  
  - Eliminate low-potential high-priced models  
  - Balance brand and price dimensions for strategic layout  

---

## ✅ Conclusion

- Market can be divided into **three clear segments**: affordable daily-use vehicles, mid-to-high-end new energy vehicles, and premium models.  
- Price ≤ 250,000 yuan is the **core threshold** for distinguishing user attention.  
- Leading brands succeed with **multi-model coverage + targeted pricing** strategies.  
- Data-driven segmentation enables automakers to **reduce marketing costs and optimize positioning**.  

---

## 📘 Project Files

- Data: `dongchedi_rank_data_clean.csv`
- Notebook: [Dangchedi Platform.ipynb](https://github.com/25422138/Automotive-Market-Segmentation-and-Consumer-Insights-Dangchedi-Platform-/blob/main/Automotive%20Market%20Segmentation%20and%20Consumer%20Insights%20(Dangchedi%20Platform)/Dangchedi%20Platform.ipynb)
- Presentation: `Automotive Market Segmentation and Consumer Insights (Dongchedi Platform).pptx`
