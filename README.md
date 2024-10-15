# Oculens 

# Project Overview
**Oculens** is a data-driven project designed to assess myopia (nearsightedness) severity using personal and behavioral attributes. By collecting various input parameters from individuals, such as age, study time, screen time, gender, etc., the system estimates a numeric severity score of myopia for each person. This personalized myopia severity score aims to provide insights for individuals about their eye health and can assist healthcare professionals in identifying high-risk individuals for intervention.

The project employs machine learning techniques, including regression models and clustering, to create a predictive model that estimates the severity of myopia based on input data.

## Features
- **Personalized Myopia Severity Score**: Predicts the severity of myopia for each individual based on personal and lifestyle factors.
- **Data Analysis and Feature Engineering**: Preprocesses input data to extract meaningful features that contribute to myopia severity prediction.
- **Machine Learning Models**: Utilizes linear regression models and K-Means clustering to predict severity scores and group individuals with similar attributes.
- **Classification of Myopia Severity**: Classifies the predicted scores into different severity levels for better interpretation.
- **User Input Interface**: Allows users to input their details and predict their myopia severity score.
- **Data Visualization**: Visualizes the results of clustering and regression using charts, enhancing interpretability.

## Dataset and Attributes
The dataset contains personal and behavioral attributes of individuals related to myopia. The attributes used include:
- **Age**: The individual’s age.
- **Gender**: Male/Female.
- **Study Time**: Time spent studying.
- **Screen Time**: Time spent on screens.
- **Myopia Sensitivity**: A target variable indicating the sensitivity to myopia.

## Data Preprocessing
The dataset undergoes the following preprocessing steps:
- **Feature Selection**: Attributes irrelevant to myopia prediction, such as 'ID,' 'STUDY YEAR,' and 'AGE,' are removed from the dataset.
- **Correlation Analysis**: The correlation between the remaining attributes and myopia is calculated using the `corrwith()` function to identify significant features.
- **Train-Test Split**: The dataset is split into training and testing sets using the `train_test_split()` function to evaluate model performance.


## User Input Interface
The project includes a user-friendly interface where users can input:
- Age
- Gender
- Screen time
- Study time
- Myopia realization year
The model then predicts the severity of myopia for the individual based on these inputs.

## How to Run the Project
1. **Clone the Repository**: Clone the repository to your local machine.
   ```bash
   git clone https://github.com/your-repo/Oculens.git
   ```
2. **Install Dependencies**: Install the required dependencies from `requirements.txt`.
   ```bash
   pip install -r requirements.txt
   ```
3. **Prepare the Dataset**: Ensure the dataset is available in the project directory and properly formatted.
4. **Run the Model**: Execute the script to preprocess data, train the model, and make predictions.
   ```bash
   python oculens_model.py
   ```
5. **User Input Interface**: Use the input interface to enter personal details and predict myopia severity.

## Dependencies
- Python 3.x
- scikit-learn
- pandas
- numpy
- matplotlib

## Results
- **Severity Scores**: The model generates myopia severity scores for each individual.
- **Classification**: Scores are classified into severity levels for easy interpretation.
- **Clustering**: The K-Means clustering results help in understanding the grouping of individuals based on similar myopia attributes.

