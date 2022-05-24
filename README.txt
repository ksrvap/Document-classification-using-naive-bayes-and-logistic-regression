About the script:
-----------------
-The language used to implement the ID3 algorithm here is "python".
-There are two scripts uploaded that contain the code for each classifier.
-One of them is for Naive Bayes and the other is for Logistic Regression.
-The code in the notebook file can be seen as sections for better understanding.
-Both of them are executable under different environments and the instructions for execution are given below.

Instructions for execution:
---------------------------
Requirements:
1. Python 3.7 or above installed (for .py file)
2. Jupyter Notebook (for .ipynb file) OR
3. Google Colab (for .ipynb file) OR
4. Any other IDE that supports python execution.

Steps to execute:
-----------------
1. Load the file into the environment, either .py file or .ipynb file.

2. Changing path for training data
  - Change the path for the training data set.
  - Copy the path of the actual file in your system and paste as a parameter in the read_csv(method).
  - If Google colab is used, you can upload the file to the runtime and copy the path from there.

3. For splitting the original data into training and testing data,
  - Using train_test_split method, the data is split into two sets.
  - The size of the test set is .2 in this case which means 20% of the original data.
   
4. For the Naive Bayes Classifier,
  - The value of beta can be choosen from the given list.
  - We have started with the value 1/|v|.
  - The accuracy that is on the report is obtained when beta = 0.01
  - The training accuracy can be seen after executing the validation method on testing_data.
  - Then the actual testing function is defined and tested using the original_testing_data.
  - The actual testing data is imported by changing the path of the file.
  - The code after that generates a graph, a confusion matrix and a list of 100 words based on rank.

5. For the Logistic Regression Classifier,
  - The value of learning rate and penalty rate can be choosen from the given lists.
  - The accuracy that is on the report is obtained when lr=0.01, pr=0.005.
  - The training accuracy can be seen after executing the validation method on testing_data.
  - Then the actual testing function is defined and tested using the original_testing_data.
  - The actual testing data is imported by changing the path of the file.
  - The code after that generates a graph and a confusion matrix.


6. After following all the above steps, run all the cells(for .ipynb file) or run the entire code(for .py file).

7. The output file "predicted.csv/predicted_lr.csv" is generated in the specified folder.