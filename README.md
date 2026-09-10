# Smoov: Relevance & Surprise Scoring Engine

Data-driven recommendation and ranking engine developed during a Business Intelligence internship at **Value Digital Services** for the Smoov travel application. The system processes cultural points of interest (POIs), scoring and categorizing locations based on historical relevance and unique "surprise" metrics.

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white"/>
</p>

---

## Project Artifacts

 **[View Presentation Slides (PDF)](Timeline%20Cycle%20Visual%20Charts%20Presentation%20in%20Blue%20White%20Teal%20Simple%20Style.pdf)**  
 **[View Processed Dataset (Excel)](last.xlsx)**

---

## Objective & Scope

* **Objective:** Identify and rank cultural and historical locations across Tunisia using data-driven Relevance and Surprise scores.
* **Scope:** Perform web scraping, clean multi-source geospatial data, execute review sentiment analysis, and train unsupervised clustering models to categorize POIs.

---

## Workflow & Methodology

1. **Data Understanding & Cleaning:** Standardized POI names, coordinates, and metadata attributes.
2. **Feature Extraction:** Scraped online reviews via APIs, calculated Wikipedia word counts, and extracted sentiment polarity scores.
3. **Clustering Analysis:** Used K-Means and Self-Organizing Maps (SOM) to group POIs with similar traits into clusters (e.g., Highly Relevant, Highly Surprising, Irrelevant).
4. **Relevance Scoring:** Applied a multi-factor weighted equation incorporating structural and sentiment parameters.
5. **Surprise Scoring:** Quantified unexpected location appeal by mining text reviews for historical significance, unique features, and visitor trends.

---

## Relevance Score Formula

The **Relevance Score ($R$)** is calculated using the following weighted mathematical model:

$$R = w_1 \cdot WWC + w_2 \cdot RSS + w_3 \cdot \log(1+NR) + w_4 \cdot UNESCO + w_5 \cdot Heritage + w_6 \cdot Cat + w_7 \cdot Type$$

| Feature Code | Variable Name | Description |
|---|---|---|
| **WWC** | Wikipedia Word Count | Total word count of the location's Wikipedia page |
| **RSS** | Review Sentiment Score | Average sentiment score from collected user reviews |
| **NR** | Number of Reviews | Total review count (log-transformed to manage extreme scale) |
| **UNESCO** | UNESCO Status | Binary indicator (1 if UNESCO site, 0 otherwise) |
| **Heritage** | Heritage Status | Binary indicator (1 if registered heritage site, 0 otherwise) |
| **Cat** | Category | Categorical classification rank (1 to 6) |
| **Type** | Type of Place | Encoded place type (e.g., historical, natural, cultural) |

---

## Team & Credits

Internship Project at **Value Digital Services**.  
