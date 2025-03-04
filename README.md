# Formula 1 Race Prediction

![Decoding motorsport dynamics with Machine Learning](predict.jpg "Decoding motorsport dynamics with Machine Learning")

This project aims to analyze historical Formula 1 race data and build predictive models to forecast race outcomes, focusing on podium finishes. 

## 1. Project Overview

**Objective:**

* Analyze historical F1 race data to understand performance trends of drivers and constructors.
* Build predictive models to forecast the Driver and Constructors' Champions for upcoming seasons.

**Data Source:**

The project uses the Ergast Developer API (http://ergast.com/mrd/) which provides historical Formula 1 data in a structured format. Data is extracted and saved as CSV files for analysis.

**Methodology:**

1. **Data Collection and Loading:** Historical race data, including results, driver and constructor information, lap times, qualifying results, etc., are collected and loaded into Pandas DataFrames.
2. **Exploratory Data Analysis (EDA):** Data is explored using visualizations and statistical analysis to understand relationships and patterns.
3. **Data Preprocessing and Feature Engineering:** Data is cleaned, transformed, and new features are created to enhance model performance. Features include driver experience, constructor wins, grid position, and more.
4. **Modeling:** Machine learning models, specifically the RandomForestClassifier, are trained to predict podium finishes.
5. **Model Evaluation and Tuning:** Model performance is evaluated using accuracy, cross-validation scores, and classification reports. Hyperparameter tuning is performed to optimize model performance.
6. **Prediction:** The trained model is used to predict race outcomes for upcoming races or seasons.

## 2. Key Findings and Insights

* **Strong correlation between Constructor Points and Wins:** A high positive correlation (0.96) was observed, indicating consistent high points are a strong indicator of championship potential.
* **Positive correlation between Driver Points and Wins:** Similar to constructors, a positive correlation (0.88) was found, although driver skill is influenced by team performance.
* **Grid Position is Highly Influential:** Starting position significantly impacts race outcomes, with front-row starters having a higher probability of winning.
* **Model Performance:** The RandomForestClassifier achieved high accuracy (98.98%) and cross-validation scores (90.90%) in predicting podium finishes.

## 3. Data and Features

**Datasets:**

* `races.csv`: Information about each race (date, circuit, etc.).
* `results.csv`: Race results for each driver (position, points, etc.).
* `drivers.csv`: Driver information (name, nationality, etc.).
* `constructors.csv`: Constructor (team) information (name, nationality, etc.).
* `...` (Include other relevant datasets)

**Key Features:**

* Driver Experience
* Constructor Wins
* Grid Position
* Driver Age
* Lap Times
* Pit Stop Strategies
* And more...

## 4. Model and Prediction

The project primarily utilizes the **RandomForestClassifier** model due to its strong performance in predicting podium finishes. The model was trained on historical data and evaluated rigorously. It can be used to predict the likelihood of drivers finishing in the top 3 positions for upcoming races.

## 5. Usage

**Running the Notebook:**

1. Clone the repository.
2. Open the Jupyter Notebook (`F1_Race_Prediction.ipynb`) in Google Colab or a compatible environment.
3. Execute the cells in the notebook to run the analysis and generate predictions.

**Making Predictions:**

The trained model can be used to make predictions on new race data by providing the necessary features (driver, constructor, grid position, etc.). 

## 6. Future Work

* Explore other machine learning models for improved prediction accuracy.
* Incorporate additional data sources, such as weather conditions and tire strategies.
* Develop a user interface for easier interaction with the model.
* Enhance visualizations for better understanding of race dynamics.

## 7. Contributing

Contributions to this project are welcome! If you have any suggestions, bug reports, or feature requests, please feel free to open an issue or submit a pull request.

## 8. License

This project is licensed under the MIT License. See the `LICENSE` file for details.
