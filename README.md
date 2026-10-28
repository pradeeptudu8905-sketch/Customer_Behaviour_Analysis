Customer Shopping Behavior Analysis


An exploratory data analysis (EDA) project investigating customer
purchasing patterns across demographics, product categories, payment
methods, discounts, subscriptions, product sizes, and shipping methods.
Project status: Descriptive EDA completed from the analysis
outputs documented in REPORT.md. The results are observational and
should not be interpreted as proof of causation.

Project Objectives

- Understand how purchase behavior varies across customer age groups.
- Compare purchase activity and review ratings across product
  categories.
- Examine purchase amounts by payment method.
- Evaluate descriptive differences between discounted and
  non-discounted transactions.
- Compare subscription rates across product categories and purchase
  frequencies.
- Explore purchase behavior by product size and shipping method.
- Translate the results into practical, testable business
  recommendations.

Key Findings

The following figures are based on the analysis outputs recorded in the
report.
1. Age groups: The 51--70 age group recorded the highest total
   revenue among age groups, at $88,480. The 18--25 group had the
   highest average purchase amount, at $60.65.
2. Product categories: Clothing had the highest transaction count
   (1,737) and the lowest average review rating (3.72) among
   the four categories. Footwear had the highest average review rating
   (3.79).
3. Payment methods: Credit Card had the highest total purchase
   amount ($40,310), while Debit Card had the highest average
   purchase amount ($60.92).
4. Discounts: Non-discounted transactions had an average purchase
   amount of $60.13, compared with $59.28 for discounted
   transactions. This difference is descriptive and does not establish
   that discounts reduce spending.
5. Subscriptions: Footwear had the highest category subscription
   rate (28.55%). Weekly purchasers had the highest subscription
   rate by purchase frequency (29.13%).
6. Product sizes: Medium had the highest transaction count
   (1,755). Small had the highest average purchase amount
   ($61.04).
7. Shipping: Free Shipping recorded the highest total revenue
   ($40,777) among shipping methods. 2-Day Shipping had the
   highest average purchase amount ($60.73).
See [`REPORT.md`](REPORT.md) for the detailed tables, interpretations,
recommendations, limitations, and next steps.


Tools and Libraries


- Python
- pandas
- Matplotlib
- Jupyter Notebook / Google Colab
- Statistical testing is recommended as a follow-up step; results
  should only be added after the tests are run.


Repository Structure


customer-shopping-behavior-analysis/
├── README.md
├── REPORT.md
├── customer_shopping_behavior.ipynb   # Add your completed notebook
├── data/
│   └── customer_shopping_behavior.csv  # Add the dataset if redistribution is permitted
└── images/
    └──                         # Add exported charts for the report/README
The notebook, dataset, and image files shown above are suggested
locations. Add them to the repository only if you have those files and
permission to share the dataset.


How to Run


1. Clone or download this repository.
2. Install the required libraries:
   pip install pandas matplotlib jupyter
3. Place the dataset in the data/ directory, or update the file path
   in your notebook.
4. Open customer_shopping_behavior.ipynb in Jupyter Notebook or
   Google Colab.
5. Run the notebook cells from top to bottom.
Example data loading code (adjust the path and filename to match your
actual file):
import pandas as pd

df = pd.read_csv("data/customer_shopping_behavior.csv")
df.head()
Analysis Workflow
1. Load and inspect the dataset.
2. Check data types, missing values, duplicates, and category labels.
3. Summarize purchase behavior using groupby(), agg(),
   value_counts(), and crosstab().
4. Visualize patterns with bar charts.
5. Interpret findings in a business context.
6. Validate totals and, where appropriate, perform statistical tests
   before making stronger claims.


Important Notes


- In the analysis screenshots, Customer ID.count() was used for some
  grouped counts. Unless the data model guarantees one row per
  customer, these counts should be described as
  records/transactions, not unique customers.
- Revenue is the sum of the recorded Purchase Amount (USD) values.
  It should not be described as profit because costs and margins were
  not included.
- The discount comparison is observational. A controlled experiment or
  suitable statistical analysis would be needed to estimate the effect
  of discounts.
- Some screenshot outputs did not show every subgroup (for example,
  the female subscriber row in one gender/subscription table).
  Incomplete tables are not used to draw complete gender-level
  conclusions.
- The results and figures should be rechecked against the original
  dataset before final publication.


Future Improvements


- Add data-quality checks and a reproducible notebook.
- Add statistical tests with assumptions, effect sizes, and p-values.
- Build a Power BI dashboard with filters for age group, gender,
  category, payment method, discount, subscription, and shipping.
- Analyze profit/margins if cost data becomes available.
- Explore customer-level behavior only after confirming whether
  Customer ID is unique or repeated.

Author
Pradeep Tudu
B.Tech, Electronics and Communication Engineering
NIT Agartala