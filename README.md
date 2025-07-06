# 📊 Autism Spectrum Disorder Prediction using Machine Learning

Hey! This is a simple machine learning project I worked on to predict the likelihood of Autism Spectrum Disorder (ASD) based on screening questionnaire data. I used a publicly available dataset containing scores from 10 autism screening questions, along with some personal details like age, gender, ethnicity, and a few medical history indicators.

---

## 📑 What I Did

The project follows a typical machine learning workflow:
- Loaded and explored the dataset to understand its structure.
- Handled missing and unknown values (the dataset used '?' for missing entries).
- Applied label encoding to convert categorical columns into numeric values.
- Split the data into training and testing sets.
- Trained three different models:
  - Decision Tree  
  - Random Forest  
  - XGBoost  
- Evaluated each model’s performance using accuracy, confusion matrix, and classification report.
- Saved the trained Random Forest model (which performed best) and the encoders for future use.

---

## 📂 Dataset Overview

The dataset includes:
- Scores from 10 yes/no autism screening questions (`A1_Score` to `A10_Score`)
- Age, gender, and ethnicity
- Information about jaundice at birth, family history of autism, country of residence, screening result score, relation of respondent to the child
- A final diagnosis column (`Class/ASD`) indicating whether the person was actually diagnosed with ASD.

---

## 📊 Model Results

After training the models, here’s how they performed:

| Model             | Accuracy |
|:-----------------|:----------|
| Decision Tree     | 92%      |
| Random Forest     | **96%**  |
| XGBoost           | 94%      |

I went ahead and saved the Random Forest model since it gave the highest accuracy.
