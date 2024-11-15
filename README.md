# MOVIES ANALYSIS
## 1.0	Overview

Analysis and Methods
The analysis includes several statistical and visualization techniques to uncover insights:

Data Cleaning: Filtering missing values and removing outliers to ensure data quality.
Univariate Analysis: Examining the distribution of single variables, such as production budgets and gross revenue, through histograms and summary statistics.
Correlation Analysis: Exploring relationships between financial variables to understand associations (e.g., production budget vs. worldwide gross).
Regression Analysis: Modeling the relationship between production budgets and worldwide gross to predict potential revenue.
Genre and Studio Analysis: Identifying top-performing genres and studios and examining their financial impact.
Multivariate Analysis: Combining multiple factors (budget, genre, year) to analyze financial outcomes using heatmaps, scatter plots, and regression models.
Visualizations
The following visualizations are included in this analysis:

Bar Charts: Showing movie count by genre and studio to highlight popularity and distribution.
Line Plots: Illustrating trends over time in production budgets and gross revenue.
Correlation Heatmap: Displaying relationships between key financial metrics.
Box Plots: Highlighting the spread and outliers in production budgets across genres.
Tree Maps: Visualizing the contribution of various genres or studios to overall revenue.
Histograms: Showing the distribution of average votes to understand movie ratings.
Key Findings
Some insights uncovered during the analysis:

Genres like Action and Adventure are often associated with higher budgets and revenue.
Production budget has a positive correlation with worldwide gross, though other factors also play a significant role in profitability.
Studios with high output (e.g., Warner Bros, Universal Pictures) tend to dominate in revenue, but not always in ROI, indicating varied profitability.
How to Use This Project
Prerequisites
Python libraries: pandas, matplotlib, seaborn, statsmodels
Tableau Public for interactive visualizations
Instructions
Clone this repository:
bash
Copy code
git clone <repository-url>
Run financial_analysis.ipynb in Jupyter Notebook or any other compatible IDE.
Use Tableau Public to create additional visualizations by importing movies.csv.
