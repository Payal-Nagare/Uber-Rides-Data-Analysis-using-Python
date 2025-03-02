Uber Dataset Analysis

Overview

This project analyzes an Uber dataset to derive insights about user behavior, ride purposes, and patterns in ride distances. The dataset contains 1156 entries with columns such as start and end times, ride category, start and stop locations, miles traveled, and purpose of the ride. The goal is to preprocess, clean, visualize, and extract meaningful insights from the data.

Dataset Information

Total Rows: 1156

Total Columns: 7

Columns: START_DATE, END_DATE, CATEGORY, START, STOP, MILES, PURPOSE

Missing Values: Found in END_DATE, CATEGORY, START, STOP, and PURPOSE columns.

Data Preprocessing

Filled missing values in the PURPOSE column with "NOT".

Converted START_DATE and END_DATE to datetime format.

Extracted date and time from START_DATE.

Created a day-night classification based on time (Morning, Afternoon, Evening, Night).

Dropped duplicate rows to maintain data integrity.

Data Visualization & Insights

1. Ride Category and Purpose Distribution

Majority of the rides were for business purposes.

Most common reasons for rides were Meetings and Meal/Entertainment.

2. Time-Based Analysis

Peak hours: Most rides were booked between 10 AM - 5 PM.

Day classification: Rides were categorized into Morning, Afternoon, Evening, and Night for better analysis.

3. One-Hot Encoding of Categorical Data

Encoded CATEGORY and PURPOSE using OneHotEncoder for better numerical analysis.

4. Correlation Analysis (Heatmap)

Business and Personal categories were highly negatively correlated, confirming previous observations.

No strong correlation among other features was found.

5. Monthly Ride Trends

Rides decreased in November, December, and January, likely due to winter months.

Other months had fluctuating ride counts.

6. Day of the Week Analysis

Rides were distributed across the week, but weekdays had more rides than weekends.

7. Miles Distribution Analysis

Most rides were short-distance (4-5 miles).

Majority of rides were within 0-20 miles, with very few long-distance rides (>20 miles).

Key Takeaways

Business-related rides dominate the dataset.

Afternoon hours (10 AM - 5 PM) see the highest ride activity.

Winters (Nov-Jan) have fewer rides compared to other months.

Most rides cover short distances, mainly under 20 miles.

Conclusion

This dataset provides valuable insights into Uber ride patterns, showing how business users, short trips, and specific hours drive ride demand. Future work can explore additional factors like seasonal trends, geographical ride patterns, or fare price analysis for deeper insights.
