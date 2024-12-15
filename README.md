# Iris Dataset Analysis

## Project Overview
This project involves an in-depth analysis of the **Iris Dataset**, a classic dataset in machine learning and statistics. The analysis includes exploratory data analysis (EDA), hypothesis testing, dimensionality reduction, and advanced statistical methods to uncover patterns and insights in the data.

## Steps Performed

### 1. Exploratory Data Analysis (EDA)
- **Univariate Analysis**:
  - Analyzed distributions of individual features using histograms, density plots, and box plots.
  - Key Insights:
    - Petal features (length and width) show greater variance compared to sepal features.
    - Setosa is easily distinguishable from other species based on its petal measurements.

- **Bivariate Analysis**:
  - Explored relationships between feature pairs using scatter plots and correlation heatmaps.
  - Key Insights:
    - Strong positive correlation between petal length and petal width.
    - Sepal features are less correlated with petal features.

- **Multivariate Analysis**:
  - Created 3D scatter plots using Matplotlib and Plotly for enhanced species separation.
  - Key Insights:
    - Matplotlib 3D visualization struggled to separate some species.
    - Plotly provided a clearer distinction between species clusters.

### 2. Hypothesis Testing
- Performed a **t-test** to compare the petal lengths of Iris Versicolor and Iris Virginica.
  - **Results**:
    - T-statistic: -12.60
    - P-value: ~0 (significant difference).
  - Interpretation: There is a statistically significant difference in petal lengths between these two species.
- Calculated **Cohen’s d** to measure effect size, revealing a large effect size for this difference.

### 3. Dimensionality Reduction
- Applied **Principal Component Analysis (PCA)** to reduce dimensionality to 2 components.
  - **Explained Variance**: The first two principal components explain over 95% of the variance in the dataset.
  - Visualized clusters in the reduced 2D space, confirming clear separation of Setosa and overlapping between Versicolor and Virginica.

### 4. Clustering
- Used clustering algorithms to explore natural groupings in the data:
  - **Elbow Method**: Determined optimal cluster count for K-Means.
  - **K-Means Clustering**: Identified distinct clusters, matching species labels.
  - **Hierarchical Clustering**: Explored dendrograms for hierarchical relationships.

### 5. Advanced Statistical Methods
- Calculated confidence intervals for feature means to quantify differences across species.
- Visualized feature distributions by species to highlight patterns.
  - Key Insight: Setosa is easily separable; Versicolor and Virginica show overlapping distributions.

## Key Findings
1. **Feature Importance**:
   - Petal length and width are the most significant features for species differentiation.
2. **Species Separation**:
   - Setosa is clearly separable, while Versicolor and Virginica show some overlap in features.
3. **Statistical Insights**:
   - Hypothesis testing confirmed significant differences in petal lengths between species.
   - PCA effectively reduced dimensions while retaining most of the variance.

## Tools and Libraries Used
- **Python Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Plotly, SciPy
- **Jupyter Notebook**: For seamless integration of code, visuals, and documentation.

## Instructions for Running
1. Clone this repository to your local machine.
2. Install the required dependencies using:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook iris_analysis.ipynb
   ```
4. Run all cells sequentially to reproduce the analysis.

## Future Enhancements
- Apply machine learning models (e.g., logistic regression, SVM) for species classification.
- Explore other dimensionality reduction techniques like t-SNE.
- Extend analysis to other datasets for benchmarking.

## Acknowledgments
- The Iris dataset was introduced by Ronald A. Fisher in 1936 and is widely used in the field of machine learning and statistics.

---

This project is part of a data science portfolio to showcase skills in data analysis, visualization, and statistical modeling.

