# Deforestation
AICTE INTRENSHIP
# Classification of Fire Types in India Using MODIS Satellite Data

## Project Overview
This project performs classification of fire types in India using satellite data collected from the MODIS instrument. The datasets include fire-related observations from the years 2021, 2022, and 2023. The notebook explores and prepares the data, performs basic analysis, and sets up machine learning models for classification.

---

## Dataset Description
The following datasets are used:
- `modis_2021_India.csv`
- `modis_2022_India.csv`
- `modis_2023_India.csv`

Each dataset contains information such as:
- Geographical coordinates (latitude, longitude)
- Date/time of observation
- Fire intensity/confidence levels
- Potential labels or types of fire

---

## Workflow Summary

### 1. Importing Libraries
Essential Python libraries for data science and machine learning are imported:
- `pandas`, `numpy` for data handling
- `matplotlib`, `seaborn` for visualization
- `scikit-learn` for machine learning models and evaluation
- `xgboost` for advanced classification
- `missingno` for visualizing missing data

### 2. Data Loading
Three yearly CSV files are loaded into DataFrames:
```python
df1 = pd.read_csv('modis_2021_India.csv')
df2 = pd.read_csv('modis_2022_India.csv')
df3 = pd.read_csv('modis_2023_India.csv')
3. Exploring Dataset Shape, Structure, and Samples
Used .shape, .info(), .head(), .tail() to understand:

Size of the dataset

Column types and completeness

First and last few rows of data

4. (Planned for Extension)
Other analyses like:

Missing value checks

Duplicates removal

Target distribution visualization

Correlation heatmaps

Feature selection and model training
are suggested but not implemented in the current notebook.

Output
This version of the notebook primarily loads the datasets and provides initial insights into their structure and content.

No machine learning model training or prediction steps are executed in the current version.

File List
Copy
Edit
├── Classification_of_Fire_Types_in_India_Using_MODIS_Satellite_Data.ipynb
├── modis_2021_India.csv
├── modis_2022_India.csv
├── modis_2023_India.csv
└── README.md
How to Run
Make sure all required .csv files are in the same directory as the notebook.

Open the notebook in Jupyter or any IDE that supports .ipynb.

Run all cells to see data structure insights.

Next Steps (Suggested Enhancements)
Handle missing values and duplicates

Explore feature importance

Build and evaluate classification models

Visualize model performance
