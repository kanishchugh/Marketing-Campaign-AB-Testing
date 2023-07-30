# A/B Test Project - Marketing Campaign Effectiveness

## Overview

This repository contains the code and analysis for an A/B test conducted to evaluate the effectiveness of different marketing promotions. The goal of the project is to determine if there is a significant difference in sales between three different promotional strategies (Promotion 1, Promotion 2, and Promotion 3) and identify which promotions lead to higher sales.

## Dataset

The data used for this analysis is in the CSV format and contains the following columns:

- `MarketID`: ID of the market where the promotion was carried out.
- `MarketSize`: Categorical variable indicating the size of the market (Small, Medium, Large).
- `LocationID`: ID of the store's location.
- `AgeOfStore`: Age of the store in years.
- `Promotion`: Categorical variable indicating the promotion type (Promotion 1, Promotion 2, Promotion 3).
- `Week`: Week number when the promotion was run.
- `SalesInThousands`: Sales amount in thousands for the corresponding week and promotion.

## Project Structure

The project is structured as follows:

- `datasets/`: Folder containing the dataset used for the analysis.
- `plots/`: Folder containing visualizations and images generated during the analysis.
- `requirements.txt`: List of required Python packages and their versions.

## Analysis

The analysis includes the following steps:

1. Data Exploration: Visualize and summarize the dataset to gain insights into the variables and distributions.

2. ANOVA Model: Build an ANOVA model to test if there is a significant difference in sales between the three promotions.

3. Post-Hoc Testing: Conduct Tukey's HSD post-hoc test to compare the means of each promotion and identify significant differences.

## Results

The results of the analysis are as follows:

- The ANOVA model indicates that there is a significant difference in sales between the three promotions (p < 0.05).
- The post-hoc test reveals that Promotion 1 and Promotion 2 have significantly different sales, as do Promotion 2 and Promotion 3. However, there is no significant difference between Promotion 1 and Promotion 3.
- The mean sales for Promotion 1 and Promotion 3 are comparable, while Promotion 2 shows the lowest sales among the three.

## Conclusion

Based on the A/B test results, it is recommended that the marketing team focus on Promotion 1 and Promotion 3 as they have shown higher sales compared to Promotion 2. Promotion 2 could be further investigated to identify areas for improvement.

## Getting Started

To run the analysis, follow these steps:

1. Clone the repository to your local machine.
2. Install the required Python packages listed in `requirements.txt`.
3. Open the Jupyter Notebooks in the `notebooks/` directory to explore the analysis.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
