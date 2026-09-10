# Smoov: Relevance & Surprise Scoring Engine

**Internship Project @ Value Digital Services**

A data-driven recommendation and scoring engine built for the Smoov mobile application. This project analyzes cultural points of interest (POIs) to surface locations that are historically significant and uniquely surprising for users[cite: 2].

##  Project Objective
To identify and rank the most interesting places by establishing data-driven **Relevance** and **Surprise** scores using web scraping, feature engineering, and Machine Learning clustering[cite: 2].

##  Methodology & Tech Stack

*   **Data Collection & Cleaning (Python, Pandas):** Engineered pipelines to scrape and consolidate POI data, extracting metrics like Wikipedia page lengths, Google Maps reviews, and geographic coordinates. 
*   **Feature Engineering:** Processed key variables from raw data, including `UNESCO` status, `heritage` classification, `Average Rating`, and `Total number of ratings` to feed the scoring model.
*   **Relevance Scoring (Math Modeling):** Implemented a custom weighted scoring formula combining historical data and visitor sentiment[cite: 2]:
    $$R = w_{1} \cdot WWC + w_{2} \cdot RSS + w_{3} \cdot \log(1+NR) + w_{4} \cdot UNESCO + w_{5} \cdot Heritage + w_{6} \cdot Cat + w_{7} \cdot Type$$
*   **Surprise Scoring (Unsupervised ML):** Applied K-Means clustering and Self-Organizing Maps to group locations based on hidden characteristics, helping to identify off-the-beaten-path or unexpectedly unique places[cite: 2].

## Business Impact
The resulting algorithms allow the Smoov app to categorize places dynamically, enabling users to sort destinations by both relevance and surprise, significantly improving the app's discovery experience[cite: 2].
