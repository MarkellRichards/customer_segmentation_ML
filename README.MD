# Customer Segmentation Using K-Means Clustering

## Overview

Understanding the diverse needs of a company's clientele is crucial for driving growth and implementing effective business strategies. This project employs machine learning to segment customers into distinct groups, enabling tailored marketing and service approaches. Using the K-means clustering algorithm, we analyze customer data to derive insights into the unique characteristics and differences between customer segments. These insights can help the company enhance customer satisfaction, fidelity, and profitability by crafting personalized strategies for each segment.

## Project Workflow

This project follows a structured approach to ensure robust segmentation and meaningful insights:

1. Data Collection: Assembling a dataset from DataQuest, containing various attributes related to customer demographics and interactions.
2. Data Preprocessing and Feature Engineering: Cleaning the dataset to handle missing values, encoding categorical variables, and standardizing quantitative features for optimal clustering performance.
3. Model Implementation: Applying the K-means algorithm to segment customers into distinct clusters based on shared characteristics.
4. Results Analysis: Interpreting the clusters to provide actionable insights into the different customer groups and their behaviors.

## Dataset Description

The dataset includes the following features:

- `customer_id`: Unique identifier for each customer.
- `age`: Customer age in years.
- `gender`: Customer gender (M or F).
- `dependent_count`: Number of dependents.
- `education_level`: Level of education (e.g., "High School", "Graduate").
- `marital_status`: Marital status (e.g., "Single", "Married").
- `estimated_income`: Projected income estimated by the data science team.
- `months_on_book`: Duration as a customer in months.
- `total_relationship_count`: Number of times the customer contacted the company.
- `months_inactive_12_mon`: Number of inactive months in the past year.
- `credit_limit`: Customer's credit limit.
- `total_trans_amount`: Total expenditure on the card.
- `total_trans_count`: Number of card transactions.
- `avg_utilization_ratio`: Daily average credit utilization.

## Results

Following the application of the K-means algorithm, customers were segmented into six distinct clusters, each characterized by unique attributes:

### Cluster 1

- Characteristics: Predominantly male, highest earners, largest credit limits, lowest transaction counts, credit utilization, and transaction amounts.
- Insight: These individuals are high earners but infrequent credit card users, presenting an opportunity to incentivize increased spending.

### Cluster 2

- Characteristics: Predominantly female, married, lowest earners, smallest credit limits, highest credit utilization in small transaction amounts.
- Insight: Couples often have dependents and make frequent small purchases, suggesting an opportunity to engage them with rewards.

### Cluster 3

- Characteristics: Slight female majority, oldest customers, high credit utilization, long-standing customers, lowest spending.
- Insight: Represents long-time customers with frequent, small transactions, indicating a potential for increased spending via targeted benefits.

### Cluster 4

- Characteristics: Primarily single females, high utilization rates, low limits and transaction amounts.
- Insight: Provides an opportunity to increase credit limits and drive higher utility and income segments.

### Cluster 5

- Characteristics: Balanced gender, unknown marital status, high dependents, moderate utilization and credit limits.
- Insight: Opportunities exist in providing targeted offers to balance the high dependencies against moderate limits.

### Cluster 6

- Characteristics: Highest spenders, most transactions, primarily male, low utilization, moderate limits.
- Insight: High usage and spending capacity, representing a segment to incentivize with bonus rewards.

## Getting Started

To run the analysis or extend the project:

1. Clone the repository:

`bash git clone https://github.com/YourUsername/customer_segmentation_ml.git`

2. Set up the environment:

- Install Docker Desktop.
- Launch a Jupyter Docker stack container:

  `bash docker run -it --rm -p 10000:8888 -v "${PWD}":/home/jovyan/work quay.io/jupyter/datascience-notebook:2024-10-07`

- Documentation: [Jupyter Docker Stacks](https://jupyter-docker-stacks.readthedocs.io/en/latest/)

Alternatively, use a Python virtual environment or Conda with a `requirements.txt` file.

## Contributing

We welcome contributions! Please open an issue or submit a pull request for enhancements or fixes.

## License

This project is licensed under the MIT License.
