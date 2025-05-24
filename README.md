# S2.04 - MongoDB Queries Practice

---

# 🎯 Objectives

- Learn to query a NoSQL database effectively
- Practice writing various types of MongoDB queries
- Understand document-based filtering, projection, and operators
- Master advanced querying using arrays and conditions

---

## 🔹 Restaurant Collection Exercises

### 📌 Collection Description
We are working with a collection of **Restaurant** documents located in **New York City**. The structure contains fields like:
- `restaurant_id`
- `name`
- `borough`
- `cuisine`
- `address` (including coordinates)
- `grades` (with score, grade, and date)

---

### 📘 Basic Queries (01-10)
01. Show all documents in the Restaurants collection  
02. Show `restaurant_id`, `name`, `borough`, and `cuisine` for all documents  
03. Show `restaurant_id`, `name`, `borough`, and `cuisine`, excluding `_id`  
04. Show `restaurant_id`, `name`, `borough`, and `zipcode`, excluding `_id`  
05. Show all restaurants located in the Bronx  
06. Show the first 5 restaurants in the Bronx  
07. Show the next 5 restaurants after skipping the first 5 in the Bronx  
08. Find restaurants with a score greater than 90  
09. Find restaurants with a score greater than 80 but less than 100  
10. Find restaurants with latitude less than -95.754168  

---

### 📘 Intermediate Queries (11-25)
11. Find restaurants that do not serve 'American' cuisine, have a score > 70, and longitude < -65.754168  
12. Same as #11, but without using the `$and` operator  
13. Find restaurants not serving 'American', got a grade "A", and are not in Brooklyn; sort by cuisine descending  
14. Find `restaurant_id`, `name`, `borough`, and `cuisine` for names starting with 'Wil'  
15. Find `restaurant_id`, `name`, `borough`, and `cuisine` for names ending with 'ces'  
16. Find `restaurant_id`, `name`, `borough`, and `cuisine` for names containing 'Reg'  
17. Find restaurants in the Bronx that serve either 'American' or 'Chinese' cuisine  
18. Find `restaurant_id`, `name`, `borough`, and `cuisine` in Staten Island, Queens, Bronx, or Brooklyn  
19. Find `restaurant_id`, `name`, `borough`, and `cuisine` **not** in Staten Island, Queens, Bronx, or Brooklyn  
20. Find `restaurant_id`, `name`, `borough`, and `cuisine` where score is not more than 10  
21. Find `restaurant_id`, `name`, `borough`, and `cuisine` where cuisine is not 'American' or 'Chinees' or name starts with 'Wil'  
22. Find `restaurant_id`, `name`, and `grades` where grade is "A", score is 11, and date is ISODate "2014-08-11T00:00:00Z"  
23. Find `restaurant_id`, `name`, and `grades` where the second element has grade "A", score 9, and date ISODate "2014-08-11T00:00:00Z"  
24. Find `restaurant_id`, `name`, `address`, and `coord` where the second coordinate value is between 42 and 52  
25. Sort restaurant names in ascending order with all columns  

---

### 📘 Advanced Queries (26-33)
26. Sort restaurant names in descending order with all columns  
27. Sort cuisine ascending and for same cuisine, borough descending  
28. Find all addresses that do not contain the street field  
29. Select documents where `coord` value is of type Double  
30. Select `restaurant_id`, `name`, and `grade` where score modulo 7 is 0  
31. Find `name`, `borough`, `longitude`, `latitude`, and `cuisine` for names containing 'mon'  
32. Find `name`, `borough`, `longitude`, `latitude`, and `cuisine` for names starting with 'Mad'  

---

## 🏆 Achievement Levels

### 🥉 Level 1 (Basic)
- ✅ At least 17 correct queries completed  
- 📌 Covers fundamental projections, filters, and conditionals

### 🥈 Level 2 (Intermediate)  
- ✅ 17–25 queries completed  
- 📌 Combines filters, range conditions, sorting, and logic

### 🥇 Level 3 (Advanced)
- ✅ More than 25 correct queries completed  
- 📌 Complex array access, date-based conditions, type matching, and custom logic

📝 *All levels require valid MongoDB syntax and correct result sets*

---

# 🛠️ Technologies Used

- MongoDB
- Studio 3T for MongoDB
- https://todiagram.com/editor

---

## ⚙️ Installation & Execution

### 📋 Requirements
- MongoDB Community Server
- MongoDB Compass or any other client tool
- Sample database with NYC Restaurants collection

---

### 🛠️ Setup

1. Download the dataset (e.g., `restaurants.json`)
2. Use Studio 3T for testing.

---

### ▶️ Execution

1. Run queries using the Mongo Shell or MongoDB Compass:
```js
// Example:
db.restaurants.find({ borough: "Bronx" }).limit(5);
```
2. Use Studio 3T for testing.

---

# 🌐 Deployment

This query set is designed for learning and testing in any local or cloud-based MongoDB environment.

---

## 📦 Repository

You can store your query files and database import scripts in a Git repository for collaboration and version control.

---

## ✅ Author Notes

These exercises are created to help you gain hands-on experience with MongoDB querying across various real-world scenarios.

After importing the dataset, experiment freely with queries to explore filtering, sorting, and aggregating data.

Happy querying! 🚀
