# Cart Abandonment Prediction – Model Training & Evaluation

A complete machine learning pipeline to predict cart abandonment using multiple classification models, model comparison, hyperparameter tuning, and performance evaluation.

---

## 📌 Project Overview

This project builds and evaluates multiple machine learning models to predict whether a customer will abandon their cart.

The workflow includes:

- Data loading and preprocessing
- Feature encoding and scaling
- Training five classification algorithms
- Model comparison using evaluation metrics
- Automatic best model selection
- Hyperparameter tuning
- Performance comparison (before vs after tuning)
- Visual performance analysis

The objective is to identify the most effective model for predicting cart abandonment and interpret its business impact.

---

## 📂 Dataset

**File Used:** `cart_abandonment_data.csv`

### 🎯 Target Variable:
- `Cart_Abandoned`
  - 1 → Abandoned
  - 0 → Purchased

### 📊 Features Include:
- Customer behavior indicators
- Product interaction features
- Session-level information
- `Customer_Segment_Type`
- `Is_Product_Details_viewed` (Yes/No)
- Numerical engagement metrics

---

## 🛠 Notebook Workflow (`Model_Training.ipynb`)

### STEP 1 – Load Data
- Load dataset using pandas
- Display head, info, and null values
- Analyze class distribution

### STEP 2 – Preprocessing
- Separate features (X) and target (y)
- Map Yes/No → 1/0
- One-hot encode `Customer_Segment_Type`
- Scale numerical features using `StandardScaler`
- Use `ColumnTransformer` for consistent preprocessing

### STEP 3 – Train-Test Split
- 80% Training
- 20% Testing
- Stratified split
- `random_state=42`

---

## 🤖 Models Trained

The following five classification models were trained separately:

1. Logistic Regression  
2. Decision Tree  
3. Random Forest  
4. Support Vector Machine (SVM)  
5. Gradient Boosting  

Each model was evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC

---

## 📈 Model Comparison

- All models were compared using a structured DataFrame.
- Models were sorted based on **F1 Score**.
- The best-performing model was automatically selected.

---

## ⚙ Hyperparameter Tuning

- Performed using `GridSearchCV`
- 5-Fold Cross Validation
- Optimized for F1 Score
- Compared performance before and after tuning

---

## 📊 Visualizations

For the tuned best model:

- Confusion Matrix (Heatmap)
- ROC Curve
- Precision-Recall Curve
- Feature Importance Plot (tree-based models)
  OR
- Coefficient Visualization (linear models)

---

## ✅ Key Outcomes

- Identified the best classification model
- Improved performance via hyperparameter tuning
- Evaluated using multiple metrics
- Built a complete ML evaluation pipeline

---

## 📦 Requirements

- Python 3.7+
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

Install dependencies:

```bash
pip install -r requirements.txt

## Installation

```bash
# Clone the repository
git clone https://github.com/aryamansingh04/Cart-Abandonment.git
cd Cart-Abandonment

# Install required packages
pip install -r requirements.txt
```

## Running Locally

To run the notebook locally:

```bash
# Start Jupyter
jupyter notebook

# Open notebook.ipynb in the browser
```

Or use Google Colab:
```bash
# Upload the notebook to Google Colab
# Or open directly: https://colab.research.google.com
```

## Author

Aryaman Singh

## License

This project is open source and available under the MIT License.

## Contributing

Contributions are welcome! Please feel free to submit issues or pull requests.

---

For detailed analysis and insights, please refer to the Jupyter notebook in this repository.
