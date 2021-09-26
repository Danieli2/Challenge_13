# Challenge_13
***

**Background**
I work as a risk management associate at Alphabet Soup, a venture capital firm. Alphabet Soup’s business team receives many funding applications from startups every day. The team has asked me to help them create a model that predicts whether applicants will be successful if funded by Alphabet Soup.

The business team has given me a CSV file containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. The CSV file contains a variety of information about each business, including whether or not it ultimately became successful. I will use machine learning and neural networks, to decide the features in the provided dataset to create a binary classifier model that will predict whether an applicant will become a successful business.

**I am Creating**
To predict whether Alphabet Soup funding applicants will be successful, I will create a binary classification model using a deep neural network.
This challenge consists of three technical deliverables. 
1. Preprocess data for a neural network model.
2. Use the model-fit-predict pattern to compile 
3. evaluate a binary classification model.

**Optimize the model**

Instructions:
The steps for this challenge are broken out into the following sections:

1.Prepare the data for use on a neural network model.

2.Compile and evaluate a binary classification model using a neural network.

3.Optimize the neural network model.

**Prepare the Data for Use on a Neural Network Model**
I used my knowledge of Pandas and scikit-learn’s StandardScaler() to preprocess the dataset so that I can use it to compile and evaluate the neural network model later.
I completed the following data preparation steps:
1. I read the applicants_data.csv file into a Pandas DataFrame. Review the DataFrame, looking for categorical variables that will need to be encoded, as well as        columns that could eventually define my features and target variables.
2. I droped the “EIN” (Employer Identification Number) and “NAME” columns from the DataFrame, because they are not relevant to the binary classification model.
3. I encoded the dataset’s categorical variables using OneHotEncoder, and then place the encoded variables into a new DataFrame.
4. I then added the original DataFrame’s numerical variables to the DataFrame containing the encoded variables.
5. I create the features (X) and target (y) datasets. The target dataset is defined by the preprocessed DataFrame column “IS_SUCCESSFUL”. The remaining columns are    define the features dataset.
6. I split the features and target sets into training and testing datasets.
7. I used scikit-learn's StandardScaler to scale the features data.

**Compile and Evaluate a Binary Classification Model Using a Neural Network**
I used my knowledge of TensorFlow to design a binary classification deep neural network model. This model  used the dataset’s features to predict whether an Alphabet Soup–funded startup will be successful based on the features in the dataset. I considered the number of inputs before determining the number of layers that your model will contain or the number of neurons on each layer. Then, I compiled and fit my model. Finally, I evaluated your binary classification model to calculate the model’s loss and accuracy.
I completed the following steps:
1. I created a deep neural network by assigning the number of input features, the number of layers, and the number of neurons on each layer using Tensorflow’s Keras.

2. I saved and exported my model to an HDF5 file, and name the file AlphabetSoup.h5.

**Optimize the Neural Network Model**
I used my knowledge of TensorFlow and Keras to optimize my model to improve the model's accuracy. 

I completed the following steps:

1. I Define at least two new deep neural network models (resulting in the original model, plus two optimization attempts). With each, try to improve on my first   
   model’s predictive accuracy.

2. After finishing my models, I display the accuracy scores achieved by each model, and compare the results.

3. I save each of my models as an HDF5 file.

