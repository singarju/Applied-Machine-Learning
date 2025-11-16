# Applied-Machine-Learning
The goal of this problem is for you to explore how to properly analyze, visualize, split, clean and format data and perform linear regression, polynomial regression and regularization. You will use the happiness data (e.g. happiness data.csv: train data located here Download hereand test data located here Download here. The data consists of the following attributes:

Life ladder: information about how happy people are (happiness score)
Log GDP per capita: market values of goods and services in a country
Social support: how people feel they are supported by those around them
Healthy life expectancy at birth (years)
Freedom to make life choices: how much freedom contributes to one’s feeling of happiness
Generosity: have you donated money
Perceptions of corruption: how do people perceive that there is corruption
Positive affect: do you feel happiness, laughter and enjoyment?
Negative affect: do you feel worry, anger or sadness?
Your task is to build a model that given attributes/features: Log GDP per capita, Social support, Freedom to make life choices, Generosity, Perceptions of corruption, Positive affect, Negative affect and Healthy life expectancy, predicts  Life ladder (happiness score).

Answer the questions below directly in your Jupyter Notebook, using Markdown cells. Be sure to clearly indicate that your comment is an answer to a particular question. For questions A to E use only training data. For question F use test data. 

Summarize the data. How much data is present? What attributes/features are continuous valued? Which attributes are categorical? [5 points]
Display the statistical values for each of the attributes, along with visualizations (e.g., histogram) of the distributions for each attribute. Explain noticeable traits for key attributes. Are there any attributes that might require special treatment? If so, what special treatment might they require? [5 points]
Analyze the relationships between the data attributes, and between the data attributes and label. This involves computing the Pearson Correlation Coefficient (PCC) and generating scatter plots. [10 points]
Train a Linear Regression model using the training data with four-fold cross-validation and with appropriate evaluation metric. Do this with a closed-form solution (using the Normal Equation or SVD) and with SGD. Then focus on SGD and perform Ridge, Lasso and Elastic Net regularization – try three values of penalty term and describe its impact. Explore the impact of other hyperparameters of your choice, such as learning rate (no need for grid search). Describe your findings. Select the best-performing regularization set of hyperparameters and train that model on the entire training dataset. For SGD, display the training and validation loss as a function of training epochs for the selected model. (Hint: In scikit-learn, max_iter counts epochs (full passes over the training set). To plot training/validation loss by epoch with SGDRegressor, set max_iter=1 and warm_start=True, then call fit(...) in a loop; after each call (each epoch), compute and record Train and Validation RMSE). Ensure reproducibility by using a seed. [10 points]
Repeat everything from part D with polynomial regression and using SGD. Using validation loss, explore if your model overfits/underfits the data and report your findings. Ensure reproducibility by using a seed.  [10 points]
Make predictions of the labels on the test data, using the trained model with chosen (best) hyperparameters. Summarize performance using the RMSE. Three teams with the lowest RMSE (who followed correctly all the previous steps) will receive bonus points.  [10 points]
