# ML_Learning

- Learned and implemented models including `LinearRegression` and `RandomForestRegressor()` using scikit-learn.
- Tested these models on the **diabetes dataset** from `sklearn.datasets`, a well-known regression challenge.
- Achieved an R2 of approximately **0.51 with Linear Regression** and **0.49 with Random Forest**, using well-tuned configurations.
- Explored various **model evaluation techniques**, including **scatter plots of actual vs. predicted values** to visually assess overfitting and underfitting.
- Built visualizations using `matplotlib` and `seaborn` to assess model quality.
  
## Hyperparameter Tuning
- Learned different hyperparameter tuning methods:
  - **Manual tuning** by iterating over parameter values and observing performance.
  - **Automated tuning** using tools such as `RandomizedSearchCV` and `GridSearchCV`.
  - Developed an **adaptive tuning loop** that adjusts parameter ranges after each run based on previous best parameters.

## Linear Regression Enhancements
- Started by analyzing a **correlation matrix**, and created a process to **automatically drop features** below a chosen correlation threshold to simplify the model.
- Evaluated **model coefficients** post-training to understand feature influence and remove those with low explanatory power.
- Introduced **interaction terms** (e.g., `bmi * age`, `bp * bmi`) to capture more complex relationships in the data and improve R² performance.
- Used `PolynomialFeatures` from `sklearn` to automate the generation of interaction features.

## Automation and Optimization
- Built a full **automated pipeline** that handled:
  - Preprocessing (e.g., interaction generation)
  - Model training
  - Parameter tuning
  - Performance logging (including score tracking across runs)
- Created reusable functions to generate performance tables and visualize the impact of different hyperparameter configurations.

## Reflection
- After getting used to the sklearn, I found it was the same process each time of cleaning the data (preprocessing) then creating the model
- Monitoring the model was fun using the plots and graphs charts to see if it is being random and such
- It is interesting to see the idea of simplicity vs total accuracy since we want to be able to see how to change the values we use 
- Overfitting was the biggest concept for me to grasp since I do realize there is a significant difference between seeing the relation of something working on a subset of the sample
- Using stratified sampling is very interesting too since that allowed me to avoid overfitting a lot more
