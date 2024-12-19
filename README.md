# GooglePlayStore_App_Rating
# App Rating Prediction on Google Play Store

## Description
This project uses data from the Google Play Store to analyze and predict app ratings. By performing data cleaning, exploration, and building a prediction model (Linear Regression), the project aims to determine which factors influence app ratings on the Play Store.

## Dataset
The dataset used in this project is sourced from a collection of apps on the Google Play Store. The dataset contains information such as:
- `App`: Name of the app
- `Category`: Category the app belongs to
- `Rating`: Average user rating of the app
- `Reviews`: Number of user reviews
- `Size`: Size of the app
- `Installs`: Number of installs of the app
- `Price`: Price of the app (in USD)

You can find the dataset in the file `googleplaystore.zip` included in this repository. **Before running the project**, unzip this file to access the dataset.

Steps:
1. Download and extract the file `googleplaystore.zip`.
2. Ensure that the extracted dataset file is in the same folder as the Jupyter Notebook (`GooglePlayStore1.ipynb`).

## Technologies Used
- **Python 3.x**
- **Libraries**: 
    - `pandas` for data manipulation
    - `numpy` for numerical calculations
    - `matplotlib` and `seaborn` for data visualization
    - `scikit-learn` for building the Linear Regression model
- **Tools**: Jupyter Notebook for data analysis and visualization

## Functionality
### Data Cleaning and Preprocessing
- Removed null values from the dataset.
- Converted string columns (e.g., `Size`, `Reviews`, `Installs`, `Price`) into numeric formats for analysis.
- Ensured that the data meets sanity checks, such as:
  - Average ratings should be between 1 and 5.
  - `Reviews` should not exceed `Installs`.
  - Free apps should have a price of 0.

### Data Analysis
- Performed **univariate analysis** (e.g., boxplots for `Price`, `Reviews` and histograms for `Rating` and `Size`).
- Identified outliers and removed extreme values.

### Prediction Model
- Built a **Linear Regression model** to predict app ratings based on other features.

## How to Use

### Requirements
Make sure you have **Python 3.x** installed. You can install the necessary dependencies by running the following command in your terminal:

```bash
pip install -r requirements.txt
