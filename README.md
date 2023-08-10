# TITANIC
Data Science Project for Titanic Survival Prediction.

1. Importing Modules
    - Pandas is used for creating structured dataframes of the dataset that is being used.
    - train_test_split is used to split the dataset into subsets of training and testing.
    - Random Forest Classifier is a machine learning algorithm that uses creation of trees for classification.
    - accuracy_score is used to calculate the accuracy of the prediction model.
      
2. Basic Functions on Dataset
    - We load the dataset into a variable using read_csv function of pandas library.
    - We then fetch the first 5 rows of the dataset.
    - The number of rows and columns are also fetched with the help of the shape function.
    - The info() is used to get a detailed information of the dataset.
    - We then find the total count of the null values for each column with the help of isna() and sum() fucntions.
      
3. Data Preprocessing
    - We first clean the data by dropping unnecessary columns such as passenger id, name, cabin, ticket etc.
    - We then encode the categorical data sex and embarked with the help of mapping.
    - We then fill the empty values of age and fare using median and of embarked using mode.
    - After the cleaning and transformation of the dataset, we split it into the training and testing subsets.
    - The X variable stores everything from the dataset except for the Survived column and the Y variable viceversa.
    - The test size is given as 0.2 which mean 20% for training and 80% for testing.
      
4. Training and Evaluating the Model
    - We create a model which uses Random Forest Classifier as the algorithm and then fit the training dataset into the model.
    - We then create a prediction variable using testing subset.
    - The accuracy is then checked using testing subset and prediction variable.
      
5. Function for Manual Testing
    - The test_survival() function takes all necessary column values from the user.
    - The collected data is then stored into an array which is then passed for prediction in the created model.
    - If the result obtained is 0 it refers that the person did not survive and else it is survived.
    - The function name is called inorder to execute it.
