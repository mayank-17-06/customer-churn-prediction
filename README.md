# Customer Churn Prediction

Can we predict which bank customers are about to leave? That's what this project is about.

## The idea

I was reading about how banks lose millions every year because they can't tell 
which customers are unhappy until it's too late. That got me curious — can a 
machine learning model actually catch this early?

So I took a dataset of 10,000 real bank customers and tried to answer that question.

## What I actually did

The data had things like age, account balance, credit score, country, and whether 
the customer eventually left or stayed. First I cleaned it up — dropped the stuff 
that doesn't matter like customer IDs and surnames, encoded the text columns, 
and scaled everything so the models could work with it properly.

Then I trained three different models on the same data to see which one does best:
- Logistic Regression gave 80.5%
- XGBoost gave 84.7%  
- Random Forest came out on top with 86.4%

I also plotted the confusion matrix and feature importance to understand 
what the model is actually picking up on — turns out age and account balance 
are the strongest signals.

## Results

| Model | Accuracy |
|-------|----------|
| Logistic Regression | 80.5% |
| Random Forest | 86.4% |
| XGBoost | 84.7% |

## Stack

- Python
- Pandas, NumPy
- Scikit-learn, XGBoost
- Matplotlib, Seaborn
- Google Colab

## Dataset

Kaggle — Bank Customer Churn dataset
10,000 customer records — age, balance, credit score, geography, tenure and more

## How to run

1. Clone the repo
   git clone https://github.com/mayank-17-06/customer-churn-prediction.git

2. Open churn_prediction.ipynb in Jupyter or Google Colab

3. Upload Churn_Modelling.csv from Kaggle

4. Run all cells top to bottom

## Contact

Mayank Yadav
GitHub: https://github.com/mayank-17-06
LinkedIn: https://linkedin.com/in/mayank-yadav-17
Email: yadavmayank1706@gmail.com