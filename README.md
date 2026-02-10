![Dashboard Preview](dashboard_preview.png)

**Pizza-Sales-Analysis**

📄 **Executive Summary**

The Quick Service Restaurant (QSR) industry is defined by tight margins and high operational velocity. This project involved a deep-dive analysis of 12 months of transactional data for a pizza restaurant. By analyzing 48,620 individual line items across 21,350 orders, I sought to identify inefficiencies in inventory management, staffing schedules, and menu pricing.

The analysis revealed that while the business generated $817,860 in revenue, there are significant opportunities to optimize the menu (removing underperforming SKUs) and restructure staffing during peak operational windows.

❓ **The Business Problem**

The restaurant management team faced a common scalability challenge: "We are busy, but are we efficient?" They lacked a centralized view of their performance and needed data-backed answers to the following strategic questions:

Operational Bottlenecks: When are the absolute busiest periods (Day/Time) requiring maximum staff on the floor?

Inventory Complexity: Are we stocking ingredients for menu items that no longer drive value? (e.g., specific pizza sizes or niche flavors).

Revenue Drivers: Which specific pizza categories and types are the "Cash Cows" vs. the "Question Marks"?

Seasonal Dips: Are there predictable revenue slumps during the year that require proactive marketing interventions?


🛠️ **The Analysis Methodology**

To derive these insights, I engaged in a multi-step data engineering and analysis process:

**1. Data Modeling & Merging**

The raw data was fragmented across four separate CSV files. I utilized Power Query in MS Excel to perform left-joins and create a unified "Master Dataset":

Orders.csv (Date, Time) joined with Order_Details.csv (Pizzas, Quantity).

Pizzas.csv (Price, Size) joined to calculate transactional revenue.

Pizza_Types.csv (Category, Ingredients) joined to allow for categorical segmentation.

**2. Feature Engineering**

Extracted Hour from timestamps to create trends for peak operational times.

Grouped Month to visualize seasonality trends.

**3. Visualization**

Designed an interactive Excel Dashboard to allow stakeholders to filter by Month, Category, and Size.

**📊 Deep-Dive Insights**

**1. Temporal Trends (The "When")**

Peak Season: July was the highest-performing month with **$72,557** in revenue.

The **"Fall Slump"**: Revenue consistently dips in September ($64k) and October ($64k).

The **"Lunch & Dinner Rush"**: The store exhibits a bi-modal peak.

Lunch: **12:00 PM – 1:00 PM** (Corporate/Office crowd).

Dinner: **5:00 PM – 7:00 PM** (Family/Home crowd).

**2. Product Performance (The "What")**

Category Leaders: The **"Classic"** category (e.g., Pepperoni, Hawaiian) is the volume leader, driving the most total orders. However, the **"Chicken"** category (e.g., Thai Chicken, BBQ Chicken) has a higher average price point, making it a critical revenue driver.

Top Sellers: The **Thai Chicken Pizza** and **Barbecue Chicken Pizza** are the top individual contributors to revenue.

Underperformers: The **"XXL"** size option accounts for a negligible fraction of sales (**<2%**).

**3. Customer Preference**

Size Matters: Large pizzas are the overwhelming favorite, followed by Medium. Small pizzas sell moderately, but XL and XXL have very low adoption rates.

**🚀 Strategic Recommendations**

Based on the data, I have developed the following recommendations to improve operations and profitability.

**Recommendation 1:** Optimize Staffing for "Rush Windows"

Why did it happen? 

The data proves that order volume doubles during the 12 PM–1 PM and 5 PM–7 PM windows.

What should we do next? 

Implement "Split Shift" scheduling. Instead of flat staffing all day, bring in part-time support specifically for these 3-hour windows to reduce wait times and increase table turnover.

**Recommendation 2:** Menu Rationalization (Kill the XXL)

Why did it happen? 

The XXL size drives less than 2% of revenue but likely requires specific inventory (larger boxes, larger dough balls).

What should we do next? 

Remove the XXL size from the menu. This will simplify the supply chain, reduce storage needs for unique boxes, and streamline kitchen operations without impacting significant revenue.

**Recommendation 3:** "Fall Special" Marketing Campaign

Why did it happen? 

The data shows a consistent $8k revenue drop-off in September and October compared to July.

What should we do next? 

Launch a promotional campaign in late August (e.g., "Back to School Bundle" or "Oktoberfest Feast") to artificially stimulate demand during this predictable slow period.

**Recommendation 4:** The Upsell Protocol

Why did it happen?

Large pizzas are the most popular, indicating customers perceive value there.

What should we do next? 

Train staff to aggressively upsell Medium orders to Large. With a small marginal cost difference for the restaurant but a higher price point, this will immediately increase the profit margin per order.

**💻 Technical Stack & Skills Demonstrated**

Analysis: Pivot Tables, Power Query.

Visualization: Interactive Dashboard design, Conditional Formatting.

Business Intelligence: Translating raw metrics into actionable operational strategy.

