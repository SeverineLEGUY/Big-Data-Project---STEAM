# Big-Data-Project---STEAM

 *LINK TO THE DATABRICKS NOTEBOOK* :<br>
 --> https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/1461761622814092/1302668415778982/7316918205960528/latest.html

## 🏢 About the Company: Steam

**Steam** is a digital distribution platform developed by Valve, launched in 2003. It offers:
- Game distribution and automatic updates,
- Digital Rights Management (DRM),
- Matchmaking and anti-cheat features through Valve Anti-Cheat,
- Social features (chat, in-game overlay, item marketplace, cloud saving, etc.).

Steam is now a major player in the video game industry.

---

## 🚧 Project Context

You're working for **Ubisoft**, a major French video game publisher. The company is planning to release a **revolutionary new video game** and has asked you to analyze **all available games on Steam** to:
- Better understand the video game ecosystem,
- Identify current trends,
- Explore factors that influence a game's popularity or sales.

---

## 🎯 Objectives

This project has two main goals:

- ✅ Identify the **key success factors** behind popular or high-selling games  
- ✅ Perform a **comprehensive market analysis**, both global and segmented

---

## 🖼️ Project Scope

- Use **PySpark** and **Databricks** for data exploration and analysis
- Create interactive visualizations using **Databricks' dashboard tool**
- Work with a **semi-structured JSON dataset**, hosted on an S3 bucket: s3://full-stack-bigdata-datasets/Big_Data/Project_Steam/steam_game_output.json
  
---

## 🔍 Summary of the Approach

The project was carried out in the following steps:

1. **Data Loading**
   - Connection to the S3 bucket and reading of the JSON file using PySpark.
   - Analysis of the semi-structured schema, including nested fields.

2. **Cleaning & Preparation**
   - Use of `explode()` to flatten complex, nested columns.
   - Selection and transformation of relevant columns (dates, text, prices, reviews, etc.).
   - Handling of null values and duplicates.

3. **Creation of Specific DataFrames**
   - Splitting the main dataset into logical subgroups:
     - Publisher data  
     - Genre data  
     - Platform data  
     - Pricing and review data  

4. **Exploratory Data Analysis (EDA)**
   - Use of Spark functions such as `groupBy`, `agg`, `withColumn`, etc.
   - Visualizations created in Databricks to:
     - Explore trends (by year, price, genre, etc.)
     - Identify popular games or dominant genres
     - Highlight key publishers and major platforms

5. **Insights & Recommendations**
   - Identification of factors impacting popularity (ratings, pricing, genres, etc.)
   - Key recommendations formulated for Ubisoft based on data findings


