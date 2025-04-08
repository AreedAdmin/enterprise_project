# Enterprise Project Code

Welcome to the Enterprise Project Code repository! This project was developed as part of an enterprise initiative to collect and analyze consumer behavior data. Over the course of the project, we gathered survey responses from 350 participants to better understand consumer preferences and behaviors—focusing on aspects like online grocery usage, delivery expectations, and feature prioritization. While the raw survey data has been omitted from the repository to protect privacy, all the code detailing the data preprocessing, exploratory data analysis (EDA), and feature engineering for predictive modeling is included for you to review and learn from.

⸻

## Table of Contents
- [Project Overview](#project-overview)
- [Project Structure](#project-structure)
- [Code Walkthrough](#code-walkthrough)
- [Usage Instructions](#usage-instructions)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [License](#license)

⸻

## Project Overview

This project is an end-to-end demonstration of working with survey data to uncover insights about consumer behavior in the online grocery sector. The key objectives included:
- **Data Collection & Privacy**: Collecting responses from 350 surveys while ensuring respondent data privacy. (The dataset itself has been excluded from the repository.)
- **Exploratory Data Analysis (EDA)**: Conducting comprehensive EDA to summarize statistics, visualize relationships, and understand the distribution of key variables such as Age, Salary, Weekly Spending, and more.
- **Feature Engineering for Predictive Modeling**: Engineering features that might predict consumer behavior, such as preferences for free delivery, prioritization of price vs. convenience, and delivery speed expectations.
- **Hypothesis Testing**: Running statistical tests (e.g., one-sample and two-sample t-tests, and proportion tests) to validate various hypotheses:
  - Whether non–online-grocery users are likely to try if free delivery is offered.
  - Differences in feature ranking preferences between bachelors and families.
  - Analysis of consumer expectations regarding fast delivery times.

⸻

## Project Structure

```
enterprise_project_code/
├── visualisations/
│   ├── regression/
│   │   ├── categorical_analysis.png
│   │   ├── correlation_heatmap.png
│   │   ├── feature_scatter_plots.png
│   │   ├── target_correlations.png
│   │   ├── top_features_heatmap.png
│   │   └── top_features_pairplot.png
│   ├── Age Distribution.png
│   ├── age_distribution_by_segment.png
│   ├── correlation_matrix_with_segment.png
│   ├── correlation_matrix.png
│   ├── Delivery Speed Expectations.png
│   ├── delivery_expectations_by_segment.png
│   ├── FDO by Age.png
│   ├── FDO by gender.png
│   ├── FDO by segment.png
│   ├── feature_ranking_by_segment.png
│   ├── feature_ranks_by_segments_model_output.png
│   ├── features_corr_with_family_vs_bachelor.png
│   ├── Lean Canvas.png
│   ├── linear relationships of top features to free delivery gambit.png
│   ├── online_grocery_usage_by_segment.png
│   ├── Pain:Solution.png
│   ├── pairplot_5_col_features.png
│   ├── salary_by_segment.png
│   ├── salary_dis_by_cust_segment_excl_outliers.png
│   ├── segment_correlations.png
│   ├── spending_ratio_by_segment.png
│   ├── value proposition rankings.png
│   ├── Weekly Spending by Customer Segment.png
│   ├── Weekly Spending to income ratio.png
│   └── weekly_spending_by_segment.png
├── .gitignore
├── main.ipynb
└── preprocessing.ipynb
```

- **visualisations/**: Contains various PNG images generated during the analysis, including plots for regression diagnostics, EDA visuals, and hypothesis testing outcomes.
- **main.ipynb**: This Jupyter Notebook is the core of the project. It demonstrates:
  - Data loading and initial descriptive statistics.
  - Exploratory data analysis including consumer spending and feature ranking statistics.
  - Statistical tests that help answer key research hypotheses regarding consumer behavior.
- **preprocessing.ipynb**: This notebook covers the initial data cleaning, transformation, and preparation steps. It outlines the feature engineering process that feeds into the predictive modeling tasks.
- **.gitignore**: Ensures that sensitive data files (e.g., raw survey data) are not included in the repository.

⸻

## Code Walkthrough

### Data Preprocessing

The preprocessing.ipynb notebook is dedicated to cleaning and preparing the raw survey data. Key steps include:
- Handling missing data while preserving data privacy.
- Converting data types (e.g., numerical conversion of binary categorical variables).
- Engineering new features to better capture consumer behavior nuances for subsequent analysis.

### Exploratory Data Analysis (EDA)

The main.ipynb notebook starts with a detailed exploratory analysis, which includes:
- **Descriptive Statistics**: Generating summaries (mean, standard deviation, min/max values) to get an initial sense of the dataset.
- **Visualizations**: Creating insightful plots such as correlation matrices, distribution plots (e.g., age distribution, weekly spending) and segment-wise comparisons.

### Hypothesis Testing & Feature Engineering

Several hypotheses were tested using statistical methods:
- **Hypothesis 1**: Testing if non–online grocery users are significantly more likely to try the service if free delivery is offered using a one-sample proportion test.
- **Hypothesis 2**: Comparing feature ranking preferences between consumer segments (e.g., bachelors vs. families) using t-tests to check if price is prioritized differently.
- **Hypothesis 3 & 4**: Evaluating delivery expectations by comparing overall averages and splitting the sample between online and non-online grocery users.
- **Hypothesis 5**: Examining differences in consumer expectations regarding standard delivery times.

Each hypothesis is thoroughly analyzed through code examples and detailed statistical reporting directly in the notebooks.

⸻

## Usage Instructions

To get started with this repository:

1. **Clone the Repository**:
```bash
git clone https://github.com/AreedAdmin/enterprise_project.git
cd enterprise_project
```

2. **Install Required Dependencies**:
It is recommended to use a virtual environment. From the project directory, run:
```bash
pip install -r requirements.txt
```

Dependencies include libraries such as pandas, numpy, scipy, statsmodels, and matplotlib.

3. **Launch Jupyter Notebook**:
You can explore and run the notebooks using:
```bash
jupyter notebook
```

Open and run main.ipynb and preprocessing.ipynb to see how the data is processed and analyzed.

4. **Data Privacy Notice**:
Note that the raw survey data has been excluded from the repository to ensure participant privacy. The notebooks contain all necessary code to reproduce the analysis with your own dataset if desired.

⸻

## Dependencies
- Python 3.9+
- pandas
- numpy
- scipy
- statsmodels
- matplotlib
- Jupyter Notebook

Refer to the requirements.txt file for a full list of dependencies and their versions.

⸻

## Contributing

Contributions to enhance the analysis, add further visualizations, or improve the code structure are welcome! Please fork the repository, make your changes, and submit a pull request. For major changes, please open an issue first to discuss what you would like to modify.

⸻

## License

This project is licensed under the MIT License. See the LICENSE file for details.

⸻

Thank you for visiting our repository! We hope you find the code insightful and useful for understanding the process of data collection, feature engineering, and predictive modeling in an enterprise context.

Happy coding! 