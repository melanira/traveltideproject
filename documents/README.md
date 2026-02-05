# TravelTide Customer Segmentation Project

## Project Overview
This project analyzes customer behavior data from TravelTide to evaluate and refine proposed reward perks.
The objective is to identify meaningful customer segments and recommend targeted, cost-effective incentives
based on data-driven insights.

The project follows a full analytics workflow including data preprocessing, feature engineering,
customer segmentation, and business-oriented recommendations.

---

## Folder Structure
data/
session_base.csv
traveltide_preprocessed.csv
user_segments.csv
user_perks.csv

documents/
query.sql
README.md
TravelTideFolien.pdf

ipynb/
preprocessing.ipynb
segmentation.ipynb


---

## Notebooks

### preprocessing.ipynb
- Loads raw session-level data
- Cleans and validates data
- Handles missing values and data types
- Identifies data quality signals (e.g. negative nights, extreme clicks)
- Creates behavioral features
- Outputs: `traveltide_preprocessed.csv`

### segmentation.ipynb
- Aggregates data to the user level
- Scales behavioral features
- Evaluates the number of clusters
- Applies KMeans clustering
- Interprets clusters as customer personas
- Provides visual evidence for perk validation
- Outputs: `user_segments.csv`, `user_perks.csv`

---

## Reward Perks Evaluated
1. Free hotel meal
2. Free checked bag
3. No cancellation fees
4. Exclusive discounts
5. One free hotel night with flight

---

## Key Concepts
- **Customer Segmentation:** Customers are grouped based on behavioral similarity.
- **Targeted Perks:** Perks are assigned selectively to customer segments.
- **Simple Visualizations:** Only basic charts and tables are used to support business understanding.

---

## How to Run
1. Install dependencies
2. Run notebooks in order:
   - `preprocessing.ipynb`
   - `segmentation.ipynb`
3. Use the generated CSV files for analysis and presentation

---

## Notes
- Cluster names are interpretative and based on observed behavior.
- Data quality signals should be reviewed before automating perk assignment.
- All recommendations should be validated through A/B testing.

