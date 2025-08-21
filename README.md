Got it. Here’s a simplified, medium-length README without any src folder references.

pandemic-insights-py
A straightforward, end-to-end analytics project that turns raw pandemic data into clean insights. It uses Python (Pandas, NumPy) for cleaning and analysis, exports ready-to-use CSVs, and includes an interactive Power BI dashboard.

What’s Included
  data/raw: original CSVs

  data/cleaned: cleaned, analysis-ready CSVs

  data/analyzed: aggregated/feature-enriched CSVs

  notebooks: cleaning, EDA, feature engineering, and export steps

  dashboards/pandemic_insights.pbix: Power BI dashboard

Tech Stack
  Python: Pandas, NumPy

  Visualization: Power BI

  Files: CSV

How to Run
  Setup

   Create a virtual environment and install requirements from requirements.txt.

   Place raw CSVs in data/raw/.

   Clean and Analyze (via notebooks)

   Standardize column names and data types

   Handle missing values and duplicates

   Create rolling averages (7d/14d), growth rates, and per-capita metrics

   Export cleaned CSVs to data/cleaned and analyzed CSVs to data/analyzed

Explore in Power BI

   Open dashboards/pandemic_insights.pbix

   Refresh data connections pointing to data/cleaned and data/analyzed

   Use slicers (date, region, metric) to explore trends and drilldowns

Methods Used
   Validation: schema checks, type casting, date range sanity, duplicate detection

   Cleaning: date parsing, fixing negatives, consistent region naming/ISO codes

   Features: 7-day averages, week-over-week deltas, per-100k rates, CFR, positivity (if fields available)

   Aggregations: region/day rollups and latest snapshots for reporting

Project Structure
   data/

   raw/

   cleaned/

   analyzed/

   notebooks/

00_data_quality.ipynb

01_cleaning_transform.ipynb

02_eda.ipynb

03_feature_engineering.ipynb

04_analysis_exports.ipynb

dashboards/

   pandemic_insights.pbix

   requirements.txt

   README.md

   Filenames are examples—adjust to match the repository.

Outputs
   Cleaned CSVs: standardized, analysis-ready tables

   Analyzed CSVs: aggregated and feature-enriched datasets

   Power BI dashboard: interactive KPIs and trend pages

Notes and Limitations
   Results depend on source data quality and completeness.

   Some metrics (e.g., positivity) require consistent testing data coverage.

   If raw schemas differ, update the notebooks’ mapping cells accordingly.

Getting Help
   When reporting an issue, include:

   Which notebook and steps were run

   A small data sample (5–10 rows) with column names

   Error message and expected behavior

   This repo is designed to be easy to follow, reproducible, and useful for analysts and stakeholders.
