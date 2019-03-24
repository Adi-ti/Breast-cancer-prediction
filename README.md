# Breast-cancer-prediction
Prediction of breast cancer using one of the algorithm of machine learning i.e., KNN(K- Nearest Neighbor).However, I am using euclidean distance which is often known as the default distance used in KNN or K-means (clustering) to find the "k closest points" of a particular sample point. 
Euclidean distance is just a distance measure between a pair of samples p and q in an n-dimensional feature space.
df = pd.read_csv('breast-cancer-wisconsin.data.txt')
First we will load the data.The data i used is available here:https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Original%29
First we will replace the missing data with a ?, drop the id column, and then convert the data to a list of lists. Note that we're explicitly converting the entire dataframe to float. 
First we shuffle the data (which contains both the features and labels). Then we prepare a dictionaries for the training and testing set to be populated. Next, we specify which chunk is the train_data and which is the test_data. We do this by selecting the first 80% as train_data (by doing logic that says to slice the list up to the last 20%), and then we create the test_data by slicing the final 20% of the shuffled data.
