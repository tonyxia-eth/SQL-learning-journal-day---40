# SQL-learning-journal-day---40

# Day 40: CS50 SQL Airbnb Assignment – Views, Joins & Data Analysis

Over the past two days, I dove deeper into Lesson 4 of CS50's Introduction to Databases with SQL, working on the Boston Airbnb dataset. I focused on SQL views, JOINs, filters, and aggregate functions.

## ✅ Key Views Created

### `available`
Lists all available Airbnb listings (from the `availabilities` table).
```sql
CREATE VIEW available AS
SELECT l.id, property_type, host_name, date
FROM listings l
JOIN availabilities a ON l.id = a.listing_id
WHERE available = 'TRUE';


🧠 Extra Practice: SQL Quizzes
I created and answered several practice queries:

Counted listings per host.

Found listings with zero or minimal reviews.

Practiced using LEFT JOIN to find unmatched entries.

🔁 Next Steps
Move on to Lesson 5

Complete final project using Airbnb and/or Moneyball datasets

Refactor and publish visualizations to Tableau

