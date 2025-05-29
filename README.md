# Dead-Stock-Detection-and-Auto-Clearance-System-Implementation

# Dead Stock Detection and Auto Clearance System Implementation

## Project Overview

This project implements a system for detecting dead stock in a grocery inventory and recommending automated clearance strategies. By leveraging data analysis and machine learning, the system aims to optimize inventory management, reduce losses from unsold goods, and improve overall operational efficiency.

## Key Features

* **Data Loading & Exploration**: Loads and performs initial exploration of a grocery inventory and sales dataset.
* **Data Preprocessing & Cleaning**: Handles missing values, converts data types, and encodes categorical variables.
* **Dead Stock Identification**: Defines and identifies dead stock based on inventory turnover rates.
* **Exploratory Data Analysis (EDA)**: Visualizes turnover rate distribution, dead stock by category, and relationships between stock quantity and sales volume.
* **Machine Learning Model Training**:

  * **Classification Model (Random Forest)**: Predicts dead stock based on inventory attributes.
  * **Clustering Model (K-Means)**: Groups similar products to identify patterns that inform clearance strategies.
* **Model Evaluation**: Assesses the classification model using metrics like accuracy and classification reports.
* **Auto Clearance Strategy Recommendations**: Provides actionable insights for clearing dead stock.

## Technologies Used

* **Programming Language**: Python
* **Libraries**:

  * `pandas`, `numpy`: Data manipulation and numerical operations
  * `matplotlib`, `seaborn`: Data visualization
  * `scikit-learn`: Machine learning tools (`LabelEncoder`, `train_test_split`, `RandomForestClassifier`, `classification_report`, `accuracy_score`, `KMeans`, `StandardScaler`)

## Setup and Installation

### Prerequisites

* Python 3.x
* pip

### Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

Alternatively, if a `requirements.txt` is provided:

```bash
pip install -r requirements.txt
```

### Dataset Placement

Place the `Grocery_Inventory_and_Sales_Dataset.csv` file in the same directory as the notebook. Update the file path in the code if it's located elsewhere.

## How to Run

1. Launch Jupyter Notebook:

```bash
jupyter notebook "Dead Stock Detection and Auto Clearance System Implementation.ipynb"
```

2. Run each cell sequentially to perform data loading, cleaning, analysis, model training, and strategy recommendation.

## Motivation and Purpose

The project aims to address the challenge of dead stock in grocery inventory management. By proactively identifying unsellable items, businesses can apply timely clearance strategies to minimize financial loss and free up space.

## Challenges Faced & Solutions

* **Data Quality**: Inconsistent formats and missing values.

  * *Solution*: Imputation techniques and data type conversions.
* **Dead Stock Definition**: Need for a quantifiable threshold.

  * *Solution*: Used the 10th percentile of `Inventory_Turnover_Rate` to define dead stock.
* **Feature Engineering**: Relevant predictors needed for ML models.

  * *Solution*: Created features like `Days_Until_Expiration`, and encoded categorical features.

## Learning Outcomes

* Hands-on experience in full-cycle ML project development.
* Improved skills in cleaning, preprocessing, and visualization.
* Practical application of Random Forest and K-Means clustering.
* Interpreting classification metrics and integrating business use cases.

## Future Enhancements / Roadmap

### Continuous Improvement Plan

* **Data Quality**:

  * Automated validation checks
  * Regular audits and data governance policies
* **Model Retraining**:

  * Schedule quarterly retraining
  * Monitor metrics monthly
  * Conduct A/B testing
* **Process Optimization**:

  * Gather feedback from inventory teams
  * Adjust strategies based on observed results
  * Calibrate early warning thresholds
* **System Integration**:

  * Integrate with POS and procurement systems
  * Link with finance tools for ROI tracking

### Additional Enhancements

* **Automated Reporting**
* **Interactive Dashboard** for product managers
* **Advanced Clearance Algorithms** for dynamic pricing
* **Real-Time Processing** for inventory updates

## License

This project is open-source and available under the MIT License.

## Acknowledgments

* Dataset: `Grocery_Inventory_and_Sales_Dataset.csv` (add source if known)
* Libraries: pandas, scikit-learn, matplotlib, seaborn

## Contact

For questions or suggestions, please connect via [LinkedIn](https://linkedin.com/in/pranjalpatil) or email.
