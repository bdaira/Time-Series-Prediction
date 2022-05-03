# Time-Series-Prediction
 prices of a certain stock for the past 5 years, that can accurately predict the most recent 20% prices.
# Prerequisites
A good understanding of Python programming language.
A good understanding of neural networks.
# Development environment
Install Python and Tensorflow locally.
Google Colab
# Libraries
 pandas,
 numpy ,
 matplotlib,
keras,
sklearn,
# Run
 pip install requirements.txt
# Describtion
Splitting Data into a Training set and a Test set
You will use the mid price calculated by taking the average of the highest and lowest recorded prices on a day.

Now you can split the training data and test data. 
# Normalizing the Data
Now you need to define a scaler to normalize the data. MinMaxScalar scales all the data to be in the region of 0 and 1. You can also reshape the training and test data to be in the shape [data_size, num_features].
Due to the observation you made earlier, that is, different time periods of data have different value ranges, you normalize the data by splitting the full series into windows. If you don't do this, the earlier data will be close to 0 and will not add much value to the learning process. Here you choose a window size of 2500.

Tip: when choosing the window size make sure it's not too small, because when you perform windowed-normalization, it can introduce a break at the very end of each window, as each window is normalized independently.
