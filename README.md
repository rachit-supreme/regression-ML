# Diamond Price Prediction Model

A machine learning project that predicts diamond prices using Linear Regression based on various diamond characteristics.

## Project Overview

This project implements a predictive model for diamond prices using the following features:
- Carat weight
- Cut quality 
- Color grade
- Clarity grade
- Depth percentage
- Table percentage
- Diamond dimensions (x, y, z)
# Diamond Price Prediction Model

## Setup Instructions

1. **Clone the repository:**
```bash
git clone [repository-url]
cd regression-ML
```

2. **Create a virtual environment (recommended):**
```bash
python -m venv venv
# For Windows
venv\Scripts\activate
# For Linux/Mac
source venv/bin/activate
```

3. **Install required dependencies:**
```bash
pip install numpy pandas matplotlib seaborn sklearn jupyter
```

4. **Download the dataset:**
- Place the `diamonds.csv` file in the project root directory
- Dataset should contain columns: carat, cut, clarity, color, depth, table, price, x, y, z

## Usage

1. **Launch Jupyter Notebook:**
```bash
jupyter notebook
```

2. **Open and run the notebook:**
- Navigate to `diamonds.ipynb`
- Run cells sequentially to:
  - Load and preprocess data
  - Visualize feature relationships
  - Train the linear regression model
  - Evaluate model performance

## File Structure

```
Task1_LR/
│
├── diamonds.ipynb     # Main notebook with analysis and model
├── diamonds.csv       # Dataset file
└── README.md         # Project documentation
```

## Running the Model

The notebook contains several key sections:

1. **Data Preprocessing:**
   - Handles missing values
   - Removes zero-value dimensions
   - Encodes categorical variables

2. **Exploratory Data Analysis:**
   - Feature correlation analysis
   - Distribution plots
   - Feature relationship visualizations

3. **Model Training:**
   - Splits data (75% train, 25% test)
   - Scales numerical features
   - Fits linear regression model

4. **Evaluation:**
   - Calculates RMSE and R² score
   - Visualizes predictions vs actual values

## Model Performance Metrics

- R-squared (R²) score: 0.92
- Root Mean Square Error (RMSE): ~$1,478.32

## Requirements

- Python 3.7+
- NumPy
- Pandas
- Matplotlib
- Seaborn
- scikit-learn
- Jupyter Notebook

## Technologies Used

- **Data Processing & Analysis**
  - Pandas & NumPy for data manipulation
  - Matplotlib & Seaborn for data visualization

- **Machine Learning**
  - scikit-learn for model implementation
  - StandardScaler for numerical feature scaling
  - LabelEncoder for categorical feature encoding
  - Linear Regression model for price prediction

## Model Performance

- R-squared (R²) score: 0.89 (92% accuracy)
- Root Mean Square Error (RMSE): ~$1478.32
- Model trained on 75% data and tested on 25% data

## Key Features

- Comprehensive data preprocessing including:
  - Handling missing values
  - Removing zero-value dimensions
  - Feature scaling and encoding
- Exploratory data analysis with visualizations
- Correlation analysis between features
- Model evaluation using standard metrics

## Data Insights

- Used the 4C's of diamonds (Carat, Cut, Color, Clarity) as primary features
- Identified strong correlations between price and physical dimensions
- Discovered positive price skewness in the dataset
- Visualized feature distributions using various plots

## Future Improvements

- Experiment with different regression algorithms
- Feature engineering to improve accuracy
- Hyperparameter tuning
- Cross-validation for more robust evaluation
