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

# First calculate the mid prices from the highest and lowest
high_prices = df.loc[:,'High'].as_matrix()
low_prices = df.loc[:,'Low'].as_matrix()
mid_prices = (high_prices+low_prices)/2.0
Now you can split the training data and test data. The training data will be the first 11,000 data points of the time series and rest will be test data.

train_data = mid_prices[:11000]
test_data = mid_prices[11000:]
