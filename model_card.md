# Model Card

For additional information see the Model Card paper: https://arxiv.org/pdf/1810.03993.pdf

## Model Details
This model is a Random Forest Classifier implemented using the default hyperparameters from scikit-learn version 1.5.1. It is designed to predict whether an individual's income exceeds $50,000 annually based on demographic and employment attributes.

## Intended Use
The model is intended for educational purposes, specifically to demonstrate the application of machine learning techniques to structured tabular data. It classifies individuals into income categories (above or below $50K) using features such as age, education, occupation, and marital status.

## Training Data
The model was trained on 80% of the Census Income dataset (also known as the Adult dataset), which contains demographic and employment data extracted, by Barry Becker, from the 1994 U.S. Census database. The dataset is publicly available at the UCI Machine Learning Repository.

## Evaluation Data
The remaining 20% of the dataset, comprising 6,512 rows from the original 32,561-row census.csv file, was used for evaluation. This split ensures that the model is tested on data it has not seen during training.

## Metrics
The model was evaluated using three standard classification metrics:

Precision: 0.7419
Recall: 0.6384
F1 Score: 0.6863

Performance metrics were also calculated for specific data slices based on features such as workclass, education, marital-status, occupation, relationship, race, sex, and native-country. For a full breakdown of slice-specific metrics, refer to the file slice_output.txt.

## Ethical Considerations
The dataset originates from the 1994 U.S. Census, and may reflect historical societal biases present at that time. 

## Caveats and Recommendations
This model is intended solely for educational use and should not be used in production environments.
The model may exhibit biases due to the nature of the training data.