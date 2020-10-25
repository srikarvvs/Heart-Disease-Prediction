## Heart-Disease-Prediction
Machine Learning is used to predict the Heart Disease. The Algorithms used are 
1. KNeighborsClassifier
2. DecisionTreeClassifier
3. RandomForestClassifier


# K-Nearest Neighbors
The KNN algorithm assumes that similar things exist in close proximity. In other words, similar things are near to each other.
 
1.Load the data
2.Initialize K to your chosen number of neighbors
3. For each example in the data
3.1 Calculate the distance between the query example and the current example from the data.
3.2 Add the distance and the index of the example to an ordered collection
4. Sort the ordered collection of distances and indices from smallest to largest (in ascending order) by the distances
5. Pick the first K entries from the sorted collection
6. Get the labels of the selected K entries
7. If regression, return the mean of the K labels
8. If classification, return the mode of the K labels

# DecisionTree Classifier

A decision tree is a flowchart-like structure in which each internal node represents a test on a feature (e.g. whether a coin flip comes up heads or tails) , each leaf node represents a class label (decision taken after computing all features) and branches represent conjunctions of features that lead to those class labels. The paths from root to leaf represent classification rules

Steps for Making decision tree
1.Get list of rows (dataset) which are taken into consideration for making decision tree (recursively at each nodes).
2.Calculate uncertanity of our dataset or Gini impurity or how much our data is mixed up etc.
3.Generate list of all question which needs to be asked at that node.
4.Partition rows into True rows and False rows based on each question asked.
5.Calculate information gain based on gini impurity and partition of data from previous step.
6.Update highest information gain based on each question asked.
7.Update best question based on information gain (higher information gain).
8.Divide the node on best question. Repeat again from step 1 again until we get pure node (leaf nodes).

# RandomForestClassifier
Random forest, like its name implies, consists of a large number of individual decision trees that operate as an ensemble. Each individual tree in the random forest spits out a class prediction and the class with the most votes becomes our model’s prediction 

We can understand the working of Random Forest algorithm with the help of following steps −

Step 1 − First, start with the selection of random samples from a given dataset.

Step 2 − Next, this algorithm will construct a decision tree for every sample. Then it will get the prediction result from every decision tree.

Step 3 − In this step, voting will be performed for every predicted result.

Step 4 − At last, select the most voted prediction result as the final prediction result.

# Attribute Information ( Data set ) :
age
sex
chest pain type (4 values)
resting blood pressure
serum cholestoral in mg/dl
fasting blood sugar > 120 mg/dl
resting electrocardiographic results (values 0,1,2)
maximum heart rate achieved
exercise induced angina
oldpeak = ST depression induced by exercise relative to rest
the slope of the peak exercise ST segment
number of major vessels (0-3) colored by flourosopy
thal: 3 = normal; 6 = fixed defect; 7 = reversable defect
