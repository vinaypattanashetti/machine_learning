# Project pipeline for any machine learning project:
1. Define business case or Problem statement

2. Import the basic Libraries
   - numpy, pandas, seaborn, matlplolib...
    
3. Load the dataset

4. Domain analysis
   - Determine what data is necessary to build the model
    
5. Basic checks
   - data.shape, data.info(), data.head(), data.tail(), dtype, data.describe(), data.unique(),data.valuecounts()
    
6. Exploratory data analysis(EDA)
    - Univariate analysis
        - Used to analyze and summarize data involving only one variable.
        - Histogram, boxplot, countplot
        
    - Bivaraite analysis
        - Bivariate analysis involves the analysis of two variables simultaneously to determine if there exists a relationship or association between them
        - scatter plot, line lot, box plot, bar plot
        
    - Multivaraite analysis
       -Multivariate analysis involves the simultaneous analysis of three or more variables to understand the relationships, patterns, and interactions among them.
         - pair plot
            
7. Data Preprocessing 

    - Data cleaning: 
        - Handling missing values, 
        - remove duplicates 
        - identify outliers and treating them
            - Handle outliers using IQR, Z-score(sigma rule)-[-3,3]
    
        
    - Data transformation: 
        - Numerical data: Scaling--Normalization[0,1], standardization-- mean value 0, standard deviation 1
        - Categorical data: Encoding categorical variables into numerical
        
    - Balancing
        - handling imbalance in the data using resampling techniques
        
    
8. Feature selection
    - Drop the irrelevant columns
    - select the best features
    - check for corr and drop the columns
    - splitting of independent and dependent variable, and check for correlation
     
9. Model creation
    - training and testing data creation like x_train,x_test,y_train, y_test
    - Optimize hyperparameters using techniques like grid search, random search, or Bayesian optimization.
    - Select the right algorithm based on learning objective and data requirements. 
    - For example, linear regression is a popular option for mapping correlations between two variables in a data set.
    
10. Model Evaluation-- increasing the model performance
    - Evaluate the trained model's using the testing dataset to assess their performance.
    - Use appropriate metrics such as R2 score for regression and accuracy, precision, recall, F1-score for classification
    - Determine confusion matrix values for classification problems
    - Perform cross-validation to ensure robustness and generalize well to unseen data.
    
11. Hyperparameter tunning 
    - selecting the optimal hyperparameters for a machine learning model to maximize its optimal performance on unseen data.
    
12. Deployment
    - Deploy the model with a means of continually measuring and monitoring its performance.
    
13. Maintenance and Iteration
    - Develop a baseline or benchmark against which you can measure future iterations of the model.
    - Monitor the deployed model's performance in production and retrain or update it periodically with new data.
    - Continuously iterate on different aspects of the model to improve overall performance.
