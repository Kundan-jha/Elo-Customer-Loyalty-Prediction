# Elo-Customer-Loyalty-Prediction
#### Helping a Leading Bank Understand Customer Loyalty
## Business Problem
Elo Merchant Category Recommendation is a Kaggle competition which is provided by Elo. As a payment Brand, Elo has built partnerships with merchants in order to offer promotions and discounts to card holders. Basically, These programs make the customer's choice more strongly towards the usage of Elo. But, they want to know, do these promotions actually work for customer and merchant. Elo needs to keep their customers so loyalty of the customers towards the brand is crucial. For Example, a customer using the Elo card with diverse merchants for a long time, this signifies the user's loyalty is high. The Problem is to find a metric which has to reflect the cardholder's loyalty with Elo payment brand. In this case study, I have attempted one such problem with the help of Machine Learning.
## My Approach – Solution
Initially I will be doing the EDA and Preproccesing of the data. The major insights at the end of EDA — Data is not complete as NaN values are present in the data, The categorical features present across the data set are larger in number than numerical features. One-hot encoding of categorical features should be done for better prediction. The given features are not sufficient for training. More features must be designed with the help of domain knowledge and the business problem given. After this step I will be implementing machine learning models with two different approach to find the improvement on one another.
1. The basic model: My approach for the baseline model is totally based on my understanding of business problem. I thought what could be the features which are really crucial in this domain on which loyalty of a customer depends. At first hand, I came up with the features num_of_transactions, purchase_amount, favorite merchant, number of transactions at favorite merchant including some date-time features like first_active month, purchase_date and dormancy (Inactive period of card). Though most of these features are not explicitly given in the data, I had to derive these all with feature engineering. The model performs fairly good acknowledging the fact that data contains outliers and we can’t remove them.
2. Main model : After EDA it is pretty much clear that the given features are not sufficient for training so apart from baseline features, I created a total of 195 features. These all features are fed into the model for training and prediction. The literature survey with the already available blogs and kaggle kernels, This is pretty much clear that the simple models does not perform well while predicting the target value. So, I have started with complex models. I have experimented with various models those are : AdaBoost, XGBoost, LightGBM, Stacking, MLP — 5 Layer with Dropout and Convolution-1D Model. Among all these the best performing model is Stacking using Ridge meta-learner. One major achievement for me is that on the kaggle leaderboard my public rank and private rank is almost similar. This indicates that the model generalizes well.

If you have made it till now, It seems you are really intrested in this case study! Then do checkout my blog where I have explained every step of my approach for solving this case study.

Blog link : [Elo Customer Loyalty Prediction — Case Study](https://kundan-jha.medium.com/elo-customer-loyalty-prediction-case-study-5248b0e7c004)

You can see the deployment part below :

https://user-images.githubusercontent.com/50130996/121783729-e6739200-cbcd-11eb-81b0-7407eb6fff27.mov

YouTube link : [https://youtu.be/D0A13SzI0_8](https://youtu.be/D0A13SzI0_8)

Feel free to play with codes, If you have a crazy idea, then pull request :)
