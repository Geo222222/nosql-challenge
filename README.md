# 🥘 Eat Safe, Love – UK Food Hygiene Ratings (NoSQL Challenge)

## 🧾 Overview

This project analyzes food hygiene ratings from the UK Food Standards Agency using **MongoDB**. The dataset includes information on restaurants, cafes, takeaways, and other food-related establishments across the UK. The objective is to store, query, and analyze data efficiently using a NoSQL model.

This challenge demonstrates how to:
- Convert raw CSV data into a JSON format suitable for MongoDB
- Design and insert structured NoSQL documents
- Query and analyze data using Mongo shell and aggregation pipelines

---

## 🧰 Technologies Used

- MongoDB
- NoSQL (JSON)
- Python
- Jupyter Notebook / VS Code
- Pandas

---

## 📁 Project Structure

```
nosql-challenge/
├── uk_food.json                 # Transformed JSON-ready food rating data
├── NoSQL_setup.ipynb           # Script for ETL and conversion
├── NoSQL_analysis.ipynb        # MongoDB queries and aggregation pipelines
└── README.md                   # Project documentation
```

---

## 🔄 ETL Process

1. **Extract**
   - Started with CSV data from the UK Food Standards Agency

2. **Transform**
   - Converted fields into a nested JSON format
   - Handled missing values and normalized keys

3. **Load**
   - Inserted documents into MongoDB using `pymongo`

---

## 🔍 Analysis Goals

- Count establishments by local authority
- Find highest-rated establishments per region
- Identify trends by business type (e.g., restaurants, pubs, schools)
- Aggregate results using `$group`, `$sort`, and `$match` operators

---

## 📊 Example Queries

- Total number of takeaways in London
- Establishments with a hygiene score of 5 in Liverpool
- All establishments that contain the word "Pizza" in their name

---

## 🚀 How to Run

1. Install MongoDB locally or use MongoDB Atlas
2. Load `uk_food.json` into a collection:
```bash
mongoimport --db uk_food --collection establishments --file uk_food.json --jsonArray
```
3. Open `NoSQL_analysis.ipynb` or run queries in Mongo shell

---

## 📌 Future Enhancements

- Build a dashboard with real-time filtering by hygiene score and location
- Integrate with map APIs (e.g., Leaflet or Google Maps)
- Schedule regular scraping or API updates from the UK Food Standards Agency

---

**Author:** [Geo222222](https://github.com/Geo222222)  
**Focus:** NoSQL • Data Analysis • Public Health Data

