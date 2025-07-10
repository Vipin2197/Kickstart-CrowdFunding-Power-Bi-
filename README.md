# Kickstart-CrowdFunding-Power-Bi-
Power BI Project: Kickstarter Campaign Analysis Dashboard
🧩 Data Model Design
Created a robust star schema model in Power BI with relationships optimized for DAX performance:

Fact Table – Projects
Contains key campaign-level data:
project_id, name, category, subcategory, country, launch_date, deadline, goal_usd, pledged_usd, backers, state

Dimension Tables:

Currency: Static exchange rates for currency normalization

Calendar: Custom date table with fields like:

Year, Month, Quarter, YearMonth (YYYY-MMM)

Weekday, FinancialMonth, FinancialQuarter

Country: For filtering and geographic insights

Used Power Query for transformation and DAX for calculated columns and measures.

🔍 Core Analysis Areas (Using DAX Measures)
💱 Currency Normalization
Converted all goal and pledged values to USD using the Currency table.

📈 Campaign Volume & Distribution

Projects by country, category, and subcategory

Launch trends by Year, Quarter, Month

✅ Success Rate Analysis

Success/failure rate by category and country

Compared goal size vs outcome

🎯 Goal Bucketing Strategy
Segmented projects into ranges:

<$1K, $1K–$10K, $10K–$100K, $100K+

Analyzed success ratio across buckets

🤝 Backer Engagement Metrics

Average pledge per backer

Pledge-to-goal ratio

Impact of early pledges on overall success

🏆 Top Campaign Identification

Sorted by total pledged amount

Sorted by number of backers

📊 Dashboard Features in Power BI
Built an interactive dashboard experience with:

🌍 Geo Map – Country-wise project count and success ratio

🔳 Category Treemap – Funding by main and subcategories

📉 Line Chart – Monthly and quarterly launch & success trends

🟢 Scatter Plot – Visualizing relationship between goal size and outcome

📋 Top Projects Table – Ranked view of most-funded and most-backed campaigns

📅 Drill-Down Filters – Launch year > quarter > month

🎛️ Interactive Slicers – Country, category, state, time period

Applied best practices in Power BI design:

Consistent theme/colors

Minimal visual overload

Tooltip customization

Bookmark navigation (optional)

💡 Business Insights Derived
🏁 Ideal Goal Range: Projects with goals <$10K had 40%+ success rate

⏳ Best Duration: 30-day campaigns performed significantly better

🎮 Top Categories: Creative arts and games had higher pledge rates

📌 Coaching Opportunity: Some countries had high launch volume but low success—flagged for targeted improvement

🚀 Predictive Indicator: Early backer engagement (first 48h) strongly linked to success

🛠 Tools & Techniques Used
Power BI Desktop – Data modeling, DAX, interactive visualizations

Power Query – Data transformation, cleaning

SQL – Source-level filtering and aggregation

Excel – Static tables for currency conversion
