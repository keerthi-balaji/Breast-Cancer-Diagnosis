# Breast-Cancer-Diagnosis
Comparative study using Classification Tree and Logistic Regression to predict malignant and benign tumors. Project completed as part of the MBA course **"Discovery with Data Mining"** at PFW. It combined statistical analysis and machine learning with business-oriented decision-making, focusing on the real-world problem of breast cancer diagnosis.
## Executive Summary
This project aims to build a predictive model to classify breast tumors as malignant (M) or benign (B) using data mining and statistical techniques. The study evaluates two classification models—Classification Tree and Logistic Regression—based on key performance metrics including accuracy, sensitivity, precision, and F1-score.

> Recommendation: Logistic Regression was chosen as the optimal model due to its superior sensitivity and F1-score—critical for minimizing false negatives in medical diagnosis.

## Objective
- Develop a predictive model for breast cancer diagnosis.
- Enhance interpretability to support healthcare decision-making.
- Prioritize minimizing false negatives (i.e., undetected malignant cases).

## Dataset Description
The dataset includes:
  - Target: Diagnosis (M = Malignant, B = Benign)
  - Features: 10 core variables describing tumor characteristics:
    - Radius, Texture, Perimeter, Area, Smoothness, Compactness, Concavity, Concave Points, Symmetry, Fractal Dimension
    - Each variable has 3 versions:
      - Mean, Standard Error (SE), and Worst

## Data Preprocessing
- Handled missing values and created dummy variables.
- Removed redundant features using correlation and scatter plot analysis.
- Normalized features (0–1 range) to ensure comparability.
- Split into training, validation, and test sets.
**Tools used: Excel Analytic Solver and manual data transformations.**

## Methodology
### Models Trained
#### Classification Tree
- Tuned using tree depth and minimum terminal node records.
- Optimal configuration: Depth = 7, Min records = 12.
- Final validation accuracy: 93.86%
- Final sensitivity (recall): 89.41%

#### Logistic Regression
- Feature selection based on correlation and redundancy removal.
- Final model removed overfitting and improved generalization.
- Final validation accuracy: 92.54%
- Final sensitivity (recall): 93.00%

## Evaluation Metrics
|Metric	|Classification Tree|	Logistic Regression|
|Accuracy|	93.86%	|92.54%|
|Sensitivity|	89.41%	|93.00%|
|Specificity	|96.50%	|91.76%|
|Precision|	93.83%	|95.00%|
|F1 Score|	91.57	|93.99|
**Insight: While the classification tree had slightly higher accuracy and specificity, the logistic regression model was superior in detecting malignant tumors—crucial for reducing false negatives.**

## Key Insights
- Tumor size features like radius, perimeter, and area were the most predictive.
- Shape features (compactness, concavity) had moderate correlation.
- Structure features (smoothness, texture) had limited predictive value.
- Logistic regression provided better generalization with high interpretability.

## Technologies Used
- Excel (Analytic Solver Add-on)
- Manual statistical exploration (Descriptive Stats, Correlation, Scatter Plots)
