# Text Mining and Data Analysis

## Project Overview

This project aims to explore and analyze two different datasets: the **Titanic dataset** and the **Cereal dataset**. Through text mining, we clean and analyze passenger data, including extracting titles from passenger names, and correlate survival rates with various features. Additionally, the project performs exploratory data analysis (EDA) on a cereal dataset, analyzing nutritional information and building a logistic regression model for survival prediction.

## Dataset Overview

### Titanic Dataset
- **Source**: Titanic dataset (usually available on Kaggle or other data repositories).
- **Features**: 
  - `Name`: Contains passenger names, which will be processed for text mining.
  - `Age`: Age of the passengers.
  - `Fare`: Fare paid by the passengers.
  - `Pclass`: Passenger class (1st, 2nd, or 3rd).
  - `Survived`: Survival status (0 = No, 1 = Yes).

### Cereal Dataset
- **Source**: Cereal dataset (source can be any nutritional data of cereals).
- **Features**:
  - `calories`: Calories per serving.
  - `protein`: Protein content per serving.
  - `fat`: Fat content per serving.
  - `sodium`: Sodium content per serving.
  - `fiber`: Fiber content per serving.
  - `rating`: User rating for the cereal.

## Steps and Analysis

1. **Text Mining on Titanic Dataset**
    - Preprocessing passenger names to extract titles (Mr, Mrs, Miss, etc.).
    - Analyzing survival rates based on these extracted titles.
    - Conducting correlation analysis on numerical columns like Age, Fare, and Pclass.
    - Visualizing survival rates by gender and passenger class using bar plots.

2. **Exploratory Data Analysis on Cereal Dataset**
    - Summarizing cereal nutritional information.
    - Computing the correlation matrix for relevant numerical features like calories, fat, protein, sodium, and fiber.
    - Visualizing the correlation matrix using `ggcorrplot`.
    - Creating histograms and boxplots to visualize distributions and outliers in cereal data.

3. **Logistic Regression for Survival Prediction**
    - Building a logistic regression model to predict survival based on various features such as Pclass, Age, SibSp, Parch, Fare, and Sex.
    - Predicting survival probabilities for passengers using the logistic model.

## Key Features

- **Text Mining**: Extracts and processes passenger titles, analyzes correlations with survival rates.
- **Exploratory Data Analysis (EDA)**: Computes summary statistics and visualizes data patterns in both Titanic and Cereal datasets.
- **Logistic Regression**: Models and predicts passenger survival probabilities.

## Dependencies

The following libraries are required to run the project:

- `tm` - Text mining library for processing the Titanic dataset.
- `ggplot2` - For data visualization (e.g., bar plots, histograms, boxplots).
- `ggcorrplot` - For visualizing correlation matrices.
- `dplyr` - For data manipulation and analysis.
- `stats` - For statistical analysis (e.g., logistic regression).

You can install the required libraries by running:

```R
install.packages("tm")
install.packages("ggplot2")
install.packages("ggcorrplot")
install.packages("dplyr")
