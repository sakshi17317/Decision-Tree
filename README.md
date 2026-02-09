#  Tree-Based Regression Models Comparison

This repository presents a comparative study of three tree-based regression models using a real-world housing price dataset. The goal is to evaluate model performance, generalization ability, and behavioral differences between single-tree and ensemble methods.

---

##  Dataset

**Dataset:** California Housing Prices  
**Source:** California Census Housing Data (1990)

**Target Variable:**  
- `median_house_value` (continuous)

**Features include:**  
- Median income  
- Housing median age  
- Average number of rooms  
- Population  
- Latitude & longitude  
- Proximity to ocean (categorical)

The dataset contains **20,640 records** and is well-suited for regression tasks.

---

##  Models Implemented

The following tree-based regression models from `scikit-learn` are trained and evaluated:

1. **DecisionTreeRegressor**
   - Single decision tree
   - Easy to interpret
   - Prone to overfitting

2. **RandomForestRegressor**
   - Ensemble of decision trees using bagging
   - Reduces variance and improves generalization

3. **ExtraTreesRegressor (Extremely Randomized Trees)**
   - Highly randomized tree ensemble
   - Faster training and often more robust than Random Forest

---

##  Workflow

1. Load and explore the dataset  
2. Handle missing values  
3. Encode categorical features  
4. Split data into training and testing sets  
5. Train each regression model  
6. Evaluate performance using:
   - Mean Squared Error (MSE)
   - Root Mean Squared Error (RMSE)
   - R² Score
7. Visualize results using predicted vs. actual scatter plots  
8. Compare model performance and generalization

---

##  Evaluation Metrics

| Metric | Description |
|------|------------|
| MSE | Measures average squared prediction error |
| RMSE | Square root of MSE (interpretable in target units) |
| R² Score | Proportion of variance explained by the model |

---

##  Visualizations

For each model, a **Predicted vs. Actual** scatter plot is generated to visually assess:
- Prediction accuracy
- Bias and variance
- Generalization behavior

---

##  Results Summary

- **Decision Tree** shows higher variance and overfitting.
- **Random Forest** significantly improves accuracy and stability.
- **Extra Trees** achieves the best generalization due to increased randomness.

Overall, ensemble methods outperform the single-tree model in both accuracy and robustness.

---

##  Technologies Used

- Python 3.x  
- pandas  
- NumPy  
- scikit-learn  
- Matplotlib  

---

##  How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/sakshi17317/Decision-Tree
   
