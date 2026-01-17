# Project Name
> A regression model using regularization techniques (Ridge & Lasso) to predict house prices for Surprise Housing's market entry into Australia.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
Surprise Housing, a US-based housing company, aims to enter the Australian real estate market. The company's business model involves:
- Let the company make purchase decisions based on the saleprice.
- We are trying to predict the house price based on historic data.
- House sales data from Australia (train.csv)

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Linear Regression model is not suited for the given usecase as overfitting is happening based on the evaluation. 
    Linear Regression Summary : 
        Training R2: 0.9483
        Test R2: 0.8259
        R2 Difference: 0.1223 (12.90%)
        Training MSE: 323471053.3658
        Test MSE: 1120330869.0300
- Regularize using Lasso regression
    Lasso Regression Summary : 
        Training R2: 0.8971
        Test R2: 0.8634
        R2 Difference: 0.0337 (3.76%)
        Training MSE: 0.0162
        Test MSE: 0.0225
    Its recommended to use Lasso as most of the features are cutdown as a result of feature selection. only 27 features out of 200+ final features remain.
- Ridge regression
    Ridge Regression Summary : 
        Training R2: 0.9344
        Test R2: 0.8767
        R2 Difference: 0.0576 (6.17%)
        Training MSE: 0.0103
        Test MSE: 0.0203
    Rige has better accuracy but used more features.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Python - 3.8+
- NumPy - 1.21.0
- Pandas - 1.3.0
- Scikit-learn

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was inspired by...
- References if any...
- This project was based on [this tutorial](https://www.example.com).


## Contact
Created by [@muhilkennedy] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->