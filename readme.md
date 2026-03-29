✈️ British Airways Review Dashboard
An interactive Tableau dashboard that analyses customer reviews of British Airways, allowing users to explore ratings across key service dimensions, aircraft types, routes, and time periods.

📊 Dashboard Overview
The dashboard provides a multi-view analysis of British Airways passenger reviews, built around a dynamic metric selector that lets users drill into any of seven service categories at once.
Live Views:
SheetDescriptionSummaryHigh-level KPI cards showing average scores across all service dimensionsMapGeographic view of reviews by passenger country of originAircraftAverage ratings broken down by aircraft typeMonthTrend line of ratings over time (by month flown)

🔢 Metrics Tracked
Users can switch between the following metrics using the "Pick a metric" parameter control:

Overall Rating
Cabin Staff Service
Entertainment
Food & Beverages
Ground Services
Seat Comfort
Value for Money


🗂️ Data Sources
FileDescriptionba_reviews.csvRaw British Airways customer reviews scraped from Airline Quality review sitesCountries.csvCountry lookup table with continent and region mappings
ba_reviews.csv — Key Fields
FieldTypeDescriptiondateDateDate the review was posteddate_flownDateDate of the actual flightaircraftStringAircraft type (e.g., Boeing 777, A380)traveller_typeStringSolo, couple, family, businessseat_typeStringEconomy, Business, First, Premium EconomyrouteStringOrigin → DestinationratingIntegerOverall rating (1–10)seat_comfortIntegerSeat comfort scorecabin_staff_serviceIntegerCabin crew ratingfood_beveragesIntegerFood & drink ratingground_serviceIntegerGround service ratingvalue_for_moneyIntegerValue for money ratingentertainmentIntegerIn-flight entertainment ratingrecommendedStringWhether the reviewer recommends BA

🎛️ Filters & Interactivity
The dashboard supports the following interactive filters:

Aircraft — Filter reviews by aircraft type
Month/Date — Narrow the analysis to a specific time window
Place — Filter by the reviewer's country or region

All filters are cross-sheet actions, meaning selecting a mark on one chart filters the rest of the dashboard.

🛠️ Built With

Tableau Desktop 2025.3
Data joined across two CSV sources using Tableau's built-in data modelling


🚀 Getting Started

Clone this repository:

bash   git clone https://github.com/your-username/british-airways-review-dashboard.git

Open British_Airways_review_Dashboard.twbx in Tableau Desktop (2020.4 or later recommended).
The .twbx is a packaged workbook — all data is bundled inside, so no separate data connection setup is needed.


📁 Repository Structure
├── British_Airways_review_Dashboard.twbx   # Tableau packaged workbook (includes data)
├── ba_reviews.csv                          # Raw review data (optional, already embedded)
├── Countries.csv                           # Country reference table (optional, already embedded)
└── README.md

💡 Key Insights You Can Explore

Which aircraft types receive the highest and lowest ratings?
How have British Airways ratings trended over the years?
Which traveller types (business vs leisure) rate the airline differently?
Which routes or regions generate the most dissatisfied customers?
Is there a gap between overall satisfaction and value for money?

