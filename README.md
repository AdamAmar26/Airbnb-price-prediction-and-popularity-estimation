# Predicting Prices and Quantifying Popularity for Airbnbs in Barcelona City

## Overview
This project aims to develop a predictive model to optimize rental pricing and estimate property popularity for Airbnb listings in Barcelona. The research focuses on utilizing key features such as room type, neighborhood, accommodation capacity, reviews, and proximity to landmarks to inform pricing strategies and popularity metrics. 

The study applies machine learning techniques like **Linear Regression** and **Random Forest Regression** to analyze data from over 10,000 Airbnb listings, providing insights that can help property owners maximize revenue and adapt to market trends.

---

## Key Features
- **Price Prediction:** 
  - Explores relationships between features like number of rooms, accommodation capacity, and guest reviews to determine optimal rental prices.
  - Achieved an R² of 0.509 using Linear Regression and 0.66 using Random Forest Regression on testing data.
  
- **Popularity Estimation:** 
  - Created a composite popularity index based on metrics such as review frequency, availability, and ratings.
  - Weighted aggregation approach for key features.

- **Derived Metrics:** 
  - Incorporated features like proximity to landmarks, bedroom density, and reviews per person to enhance model accuracy.

---

## Dataset
- **Source:** Airbnb dataset containing 10,441 listings in Barcelona.
- **Key Attributes:**
  - Room Type
  - Neighborhood
  - Reviews and Satisfaction Scores
  - Accommodation Capacity
  - Geographic Coordinates (Latitude and Longitude)

### Data Preprocessing
- Removed irrelevant or incomplete columns such as `Country`, `City`, and `Bathrooms`.
- Logarithmic transformation applied to price data to mitigate outliers.

---

## Methods
1. **Data Cleaning:** Focused on retaining relevant columns and ensuring a balanced dataset.
2. **Feature Engineering:** Derived features like proximity to landmarks, satisfaction per person, and bedroom density for richer insights.
3. **Modeling Techniques:**
   - Linear Regression (Baseline)
   - Random Forest Regression
   - Linear Regression with Top Features
4. **Popularity Index:** Weighted score combining review-based metrics and listing availability.

---

## Results
- **Linear Regression:**
  - R² of 0.503 on training data and 0.509 on test data.
  - RMSE of 0.28 (training) and 0.27 (test).
- **Random Forest Regression:**
  - R² of 0.95 on training data but 0.66 on test data (indicating overfitting).
  - Accommodates emerged as the most significant predictor.
- **Popularity Index:** Scores ranged from 0.40 to 0.70, with the number of reviews having the most consistent positive influence.

---

## Limitations
- Limited dataset features may overlook influential factors like seasonal trends or host experience.
- Linear regression oversimplifies non-linear relationships.
- Overfitting observed in ensemble models.

---

## Future Work
- Incorporate advanced modeling techniques like neural networks for non-linear relationships.
- Expand dataset with temporal and sentiment analysis data.
- Scale the framework to other cities and markets.

---

## Contributors
- **Adam Amar**
- **Oore Fasawe**

---
