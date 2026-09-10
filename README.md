# Smoov: Relevance & Surprise Scoring Engine

**Internship Project @ Value Digital Services**

A data-driven recommendation engine designed to identify, rank, and categorize points of interest (POIs) for the Smoov mobile application based on cultural relevance and a unique "surprise" factor[cite: 2].

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
</p>

## Project Overview

*   **Data Ingestion & Scraping:** Developed Python web scraping pipelines to collect POI metrics, including Wikipedia page length, Google Maps review sentiment, and user ratings volume[cite: 2]. The resulting datasets structure key variables like `UNESCO` status, `heritage` tags, and `Total number of ratings`.
*   **Relevance Scoring:** Engineered a weighted mathematical model ($R=w_{1}\cdot WWC+w_{2}\cdot RSS+w_{3}\cdot \log(1+NR)+w_{4}\cdot UNESCO+w_{5}\cdot Heritage...$) to rank locations based on historical significance and visitor consensus[cite: 2].
*   **Surprise Scoring (Clustering):** Implemented unsupervised machine learning algorithms (K-Means and Self-Organizing Maps) to group locations by hidden characteristics[cite: 2]. This isolates "surprising" or off-the-beaten-path locations by analyzing unique visitor trends and text-mining cultural significance from reviews[cite: 2]. 
*   **Impact:** Empowers Smoov app users to sort and discover highly relevant or uniquely surprising heritage sites easily[cite: 2].
