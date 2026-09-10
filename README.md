# Smoov: Relevance & Surprise Scoring Engine

Data-driven recommendation and ranking engine developed during a Business Intelligence internship at **Value Digital Services** for the Smoov travel application[cite: 2]. The system processes cultural points of interest (POIs), scoring and categorizing locations based on historical relevance and unique "surprise" metrics[cite: 2].

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white"/>
</p>

---

## Project Artifacts

 **[View Presentation Slides (PDF)](Timeline%20Cycle%20Visual%20Charts%20Presentation%20in%20Blue%20White%20Teal%20Simple%20Style.pdf)**[cite: 2]  
 **[View Processed Dataset (Excel)](last.xlsx)**

---

## Objective & Scope

* **Objective:** Identify and rank cultural and historical locations across Tunisia using data-driven Relevance and Surprise scores[cite: 2].
* **Scope:** Perform web scraping, clean multi-source geospatial data, execute review sentiment analysis, and train unsupervised clustering models to categorize POIs[cite: 2].

---

## Workflow & Methodology

1. **Data Understanding & Cleaning:** Standardized POI names, coordinates, and metadata attributes[cite: 2].
2. **Feature Extraction:** Scraped online reviews via APIs, calculated Wikipedia word counts, and extracted sentiment polarity scores[cite: 2].
3. **Clustering Analysis:** Used K-Means and Self-Organizing Maps (SOM) to group POIs with similar traits into clusters (e.g., Highly Relevant, Highly Surprising, Irrelevant)[cite: 2].
4. **Relevance Scoring:** Applied a multi-factor weighted equation incorporating structural and sentiment parameters[cite: 2].
5. **Surprise Scoring:** Quantified unexpected location appeal by mining text reviews for historical significance, unique features, and visitor trends[cite: 2].

---

## Relevance Score Formula

The **Relevance Score ($R$)** is calculated using the following weighted mathematical model[cite: 2]:

$$R = w_1 \cdot WWC + w_2 \cdot RSS + w_3 \cdot \log(1+NR) + w_4 \cdot UNESCO + w_5 \cdot Heritage + w_6 \cdot Cat + w_7 \cdot Type$$

| Feature Code | Variable Name | Description |
|---|---|---|
| **WWC** | Wikipedia Word Count | Total word count of the location's Wikipedia page[cite: 2] |
| **RSS** | Review Sentiment Score | Average sentiment score from collected user reviews[cite: 2] |
| **NR** | Number of Reviews | Total review count (log-transformed to manage extreme scale)[cite: 2] |
| **UNESCO** | UNESCO Status | Binary indicator (1 if UNESCO site, 0 otherwise)[cite: 2] |
| **Heritage** | Heritage Status | Binary indicator (1 if registered heritage site, 0 otherwise)[cite: 2] |
| **Cat** | Category | Categorical classification rank (1 to 6)[cite: 2] |
| **Type** | Type of Place | Encoded place type (e.g., historical, natural, cultural)[cite: 2] |

---

## Team & Credits

Internship Project at **Value Digital Services**[cite: 2].  
**Contributors:** Raed Meddeb, Sara Madden, Youssef Hachicha[cite: 2]
