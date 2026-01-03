# Cart Abandonment Analysis

A comprehensive analysis of cart abandonment patterns across multiple e-commerce datasets, identifying key factors that influence customer purchase completion rates.

## Project Overview

This project analyzes cart abandonment behavior using data from three major e-commerce platforms:
- **Olist**: Brazilian e-commerce marketplace dataset
- **Otto**: Recommendation system dataset
- **Retail Rocket**: E-commerce behavior dataset

The goal is to understand why customers abandon their shopping carts and identify actionable insights to improve conversion rates.

## Datasets

### Olist Dataset
- `olist_customers_dataset.csv` - Customer information and location
- `olist_orders_dataset.csv` - Order details and status
- `olist_order_items_dataset.csv` - Items in each order
- `olist_order_payments_dataset.csv` - Payment information
- `olist_order_reviews_dataset.csv` - Customer reviews and ratings
- `olist_products_dataset.csv` - Product catalog
- `olist_sellers_dataset.csv` - Seller information
- `olist_geolocation_dataset.csv` - Geographic data
- `product_category_name_translation.csv` - Category translations

### Otto Dataset
- `otto-recsys-train.jsonl` - Training data for recommendation systems
- `otto-recsys-test.jsonl` - Test data for recommendation systems

### Retail Rocket Dataset
- `events.csv` - User event logs
- `category_tree.csv` - Product category hierarchy
- `item_properties_part1.csv` & `item_properties_part2.csv` - Product attributes

### Additional Data
- `online_retail_II.csv` - UK online retail transaction data

## Analysis

The Jupyter notebook (`notebook.ipynb`) contains:
- **Exploratory Data Analysis (EDA)** - Understanding data distributions and patterns
- **Data Preprocessing** - Cleaning and preparing data for analysis
- **Cart Abandonment Patterns** - Identifying abandonment trends
- **Feature Engineering** - Creating meaningful features for analysis
- **Visualizations** - Key insights and findings
- **Recommendations** - Actionable strategies to reduce cart abandonment

## Key Findings

(Refer to the notebook for detailed findings and visualizations)

## How to Use

1. **View the Analysis**: Open `notebook.ipynb` in Jupyter or Google Colab
2. **Run the Code**: Execute cells sequentially to reproduce the analysis
3. **Customize**: Modify queries and parameters to explore different aspects

## Requirements

- Python 3.7+
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- plotly (for interactive visualizations)

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
