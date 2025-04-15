# marathon-performance-predictor
## A Data Analytics and Machine Learning Project on Ultra Marathon Races Between 2021 and 2023 

#### This project aims to predict athlete performance in various sports events based on event details, athlete demographics, and other relevant factors. The goal is to build a machine learning model that can analyze historical data and make accurate predictions for new inputs.

### Overview
- Preprocessing data set of athlete performance alongside athlete metadata and event details
- Applying target encoding to categorize event names (Mean of atheltes performances in a specific event)
- Applyed label encoding for binary variables (Athlete Gender)
- Utilized a random forest regressor to perform predictions based on given inputs
- Created a simple data pipeline to handle user inputs into formattable model preset and make predictions

### Project Workflow
#### Dataset Preparation:
- The dataset contains columns like athlete age, gender, event name, event distance, and the target variable: athlete performance.
- Categorical variables are encoded using appropriate methods (e.g., target and label encoding).
### Data Preprocessing:
- Split the dataset into training and testing sets.
- Apply target encoding for high-cardinality features like event names.
- Apply label encoding for binary features like gender.
### Model Training:
- Train a Random Forest Regressor on the preprocessed data.
- Evaluate the model using metrics like Mean Absolute Error (MAE) and R² score.
### User Prediction:
- Create a pipeline to preprocess user input and predict athlete performance for new scenarios.

### Setup Instructions
#### Clone the repository
git clone https://github.com/bryanleesantoso/marathon-performance-predictor.git  
cd marathon-performance-predictor

#### Set up virtual Dependencies
python -m venv .venv  
source .venv/bin/activate       # On macOS/Linux  
.venv\Scripts\activate          # On Windows  

#### Install Dependencies
pip install -r requirements.txt  
requirements are given in the repository

pip install notebook

### Technologies used
- Python -> Core programming language.
- Pandas -> Data manipulation, cleaning, and preporcessing
- scikit-learn -> Machine learning model training and evaluation
- matplotlib -> visualizing data

### Future Enhancements
- Hyperparameter tuning -> Optimizing the Random forest model for better performance
- Data Augmentation -> Adding more features to improve realistic prediction
- Explainability -> Using SHAP or LIME to explain more about the nature of the model's prediction

### Contributing
#### You are welcome to contribute! Feel free to fork the repository and submit a pull request
1. Fork the project
2. Create a feature branch: git checkout -b feature-name
3. Commit your changes : git commit -m "Your message"
4. Push to the branch: git push origin feature-name
5. Open a pull request.

[Dataset Kaggle source]( https://www.kaggle.com/datasets/aiaiaidavid/the-big-dataset-of-ultra-marathon-running?resource=download&select=TWO_CENTURIES_OF_UM_RACES.csv  )
