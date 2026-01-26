
<img width="1024" height="576" alt="image" src="https://github.com/user-attachments/assets/9d5f8d9c-6ef0-4088-acd3-7d76f8ba615e" />



```markdown
# Airbnb Data Analysis & Insights

## 🏠 Project Overview
This project performs a **comprehensive analysis of Airbnb listings** to understand pricing, demand, guest satisfaction, host behavior, and location-based trends. It demonstrates end-to-end data analytics, starting from **data cleaning and preprocessing** to **feature engineering, exploratory data analysis (EDA), visualization, and business insights**.

The goal is to provide **actionable insights** that can help Airbnb and hosts optimize pricing, improve guest experience, and make data-driven strategic decisions.

---

## 🎯 Objectives
- Clean and preprocess the Airbnb dataset for accurate analysis.
- Understand the distribution and patterns of key variables (price, reviews, room types, etc.).
- Perform feature engineering to extract meaningful information (e.g., property age, price tiers).
- Explore relationships between price, reviews, room types, neighborhoods, and host behavior.
- Generate insights and business recommendations for Airbnb.

---

## 🧹 Data Cleaning & Preprocessing
Key steps taken:
- Removed **duplicates** and rows with missing critical values (`name`, `neighbourhood_group`, `price`, etc.).
- Standardized column names (lowercase, underscores instead of spaces).
- Filled missing values in features like `reviews_per_month`, `host_name`, `host_identity_verified`, etc.
- Cleaned numeric fields (`price`, `service_fee`, `minimum_nights`) to remove symbols and ensure correct data types.
- Stripped strings of extra spaces and special characters.

---

## 🔧 Feature Engineering
- **`year`**: Extracted from `construction_year` for time-based analysis.
- **`property_age`**: Calculated as difference between current year and construction year.
- **`price_label`**: Price bins (Low, Medium, High, Very High) for categorical comparisons.
- Imputed `minimum_nights` using the **mode per neighborhood_group and room_type**.
- Cleaned and normalized numeric and string features for reliable analysis.

---

## 📊 Exploratory Data Analysis (EDA) & Insights

### Distribution & Skewness
- Checked numeric variables for **skewness** and distribution.
- `price` and `calculated_host_listings_count` are **right-skewed**, indicating extreme values.
- `review_rate_number` is approximately symmetric (skew ~ -0.13).

### Pricing Insights
- Location and room type are **key drivers of price**.
- Newer properties charge slightly higher prices.
- Extreme prices are influenced by a small number of luxury listings.

### Guest Behavior
- Higher price does **not guarantee higher reviews**.
- Cheaper listings tend to be booked more frequently.
- Entire home/apartment listings have the highest number of reviews.

### Location-Based Insights
- Micro-markets exist even within the same neighborhood group.
- Top 5 cheapest and most expensive neighborhoods identified for investment/pricing strategies.

### Host Insights
- Most hosts manage only a few listings; a small number own multiple listings, influencing the market.

### Time-Based & Market Trends
- Newer constructions are increasingly common, indicating growth in Airbnb supply.
- Most listings prefer short-term stays (<365 nights).

---

## 💡 Business Suggestions for Airbnb
1. Implement **dynamic pricing** based on neighborhood, room type, and property age.
2. Focus on **quality of stay and amenities** rather than price alone.
3. Promote **affordable listings** to increase booking frequency.
4. Encourage **short-term stays** to maximize occupancy.
5. Use **neighborhood-level insights** for pricing and investment strategies.
6. Support **professional hosts** with analytics tools.
7. Encourage **investment in newer properties** for premium pricing.
8. Monitor and guide **extreme price listings** to maintain market stability.
9. Expand in neighborhoods with **high growth potential**.
10. Provide hosts with insights on **demand trends and competitive pricing**.


---

## 🛠️ Technologies & Libraries Used
- Python 3.x  
- Pandas, NumPy (data manipulation)  
- Matplotlib, Seaborn (visualization)  
- Regular Expressions (`re`) for string cleaning  

---



## 📌 Conclusion

This project provides **actionable insights into Airbnb listings**, helping hosts and Airbnb make data-driven decisions regarding pricing, guest satisfaction, market trends, and investment opportunities. Proper data cleaning, feature engineering, and EDA enabled a **comprehensive understanding of the Airbnb market**, highlighting key patterns and micro-market opportunities.

---

## 📂 Optional Improvements

* Predictive modeling for **price or review rating prediction**.
* Time-series analysis for **booking trends**.
* Incorporate **geospatial mapping** of neighborhoods.
* Compare Airbnb trends across multiple cities.
