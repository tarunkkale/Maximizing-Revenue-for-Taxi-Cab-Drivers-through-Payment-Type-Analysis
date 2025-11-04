# Maximizing-Revenue-for-Taxi-Cab-Drivers-through-Payment-Type-Analysis

Maximizing Revenue for Taxi Cab Drivers through Payment Type Analysis

by Tarun Kale

🎯 Project Objective

To understand how different payment methods (Card vs Cash) influence total fare revenue, and help taxi drivers identify the most profitable payment trends using real-world NYC Taxi Trip data.

🗂️ Agenda

Problem Statement – Identify key challenges affecting taxi drivers’ revenue.

Research Question – Does payment type impact fare amount?

Data Overview – Explore dataset, structure, and relevant variables.

Methodology – Steps for data cleaning, analysis, and testing.

Analysis & Findings – Insights from visual and statistical exploration.

Hypothesis Testing – Validate assumptions using statistical models.

Recommendations – Suggest strategies to increase driver revenue.

🧩 Problem Statement

In the competitive taxi industry, maximizing driver income is essential.
This project uses data-driven analysis to determine whether payment method (cash or card) influences total fare and helps drivers identify high-revenue opportunities.

🎯 Objective

Perform A/B Hypothesis Testing to analyze whether fare amount significantly differs between card-paying and cash-paying customers.

❓Research Question

“Is there a significant relationship between total fare and payment type?”
“Can drivers promote specific payment methods to increase revenue?”

📘 Dataset Overview

Source: NYC Taxi Trip Records Dataset
Size: 500,000+ rows, 18 columns
Final Cleaned Dataset: 406,511 rows, 5 columns

Feature	Description
passenger_count	Number of passengers in a trip
payment_type	Mode of payment (Card or Cash)
fare_amount	Total fare charged
trip_distance	Distance (miles)
duration	Trip duration (minutes)

🧹 After Cleaning:

Removed duplicates & irrelevant columns

Verified 0% missing values

Removed outliers in fare and duration

Added new feature duration (dropoff - pickup time)

🧮 Methodology
Step	Description
Descriptive Analysis	Statistical summary of fare, distance, and duration.
Hypothesis Testing	T-Test comparing fare amounts by payment type.
Correlation Analysis	Examined relationship between duration and fare.

📈 Formula:

duration = tpep_dropoff_datetime - tpep_pickup_datetime

📊 Key Insights
1️⃣ Journey Metrics by Payment Type
Metric	Card (Mean ± SD)	Cash (Mean ± SD)	Observation
Fare Amount ($)	10.14 ± 4.43	9.82 ± 4.49	Card users pay slightly higher fares.
Trip Distance (miles)	2.19 ± 1.42	2.06 ± 1.46	Card payments linked to longer trips.
Trip Duration (minutes)	11.28 ± 5.92	10.96 ± 6.01	Card users prefer longer rides.

💡 Interpretation:
Card-paying customers take longer, higher-value trips → higher average revenue per ride.

🧠 Preference of Payment Types
Payment Type	Share
Card	63.3%
Cash	36.7%

✅ Insight:
Majority of customers prefer digital/card payments, showing the shift toward cashless transactions.

🚗 Passenger Count Analysis

Most rides (65%) are solo passengers, and card usage is highest among them.
→ Indicates single riders prefer digital payments for convenience.

Observation:

1–3 passenger trips form ~90% of rides.

Group rides (4–5) are rare and have minimal revenue contribution.

🧪 Hypothesis Testing
Test 1 — Fare Amount vs Payment Type

Test Used: Independent T-Test
H₀: No difference in fare between card and cash.
H₁: Fare amount differs between card and cash users.

Metric	Value
T-statistic	19.53
p-value	7.00 × 10⁻⁸⁵

✅ Decision: Reject H₀
📈 Conclusion: Card users generate significantly higher fares.

Test 2 — Fare Amount vs Trip Duration

Correlation Coefficient: 0.906
🔹 Strong positive correlation → Fare increases with trip duration.

“The longer the trip, the higher the fare.”

💡 Recommendations
💳 Payment Type Impact

Encouraging card payments leads to higher average fare revenue.
Digital payments are associated with longer and more valuable trips.

⏱️ Trip Duration Impact

Strong correlation (r = 0.906) shows fare growth is duration-dependent — use it for dynamic pricing.

🚖 Final Takeaway

“Promote digital payments + Optimize pricing for longer trips = Maximum driver revenue.”

📈 Tools & Libraries Used

Python (Pandas, NumPy, Matplotlib, Seaborn, SciPy)

Excel for initial exploration

Jupyter Notebook for analysis

PowerPoint / Gamma for visualization

🏁 Conclusion

Card-based payments and longer trip durations both directly impact taxi driver earnings.
Using data analysis and hypothesis testing, we can predict revenue drivers and recommend strategies for higher income optimization.



Created by: Tarun Kale
📍 Data Analyst | Microsoft & IBM Certified
📊 Python | SQL | Excel | Power BI | Data Visualization
