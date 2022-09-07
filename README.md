# Three Predictive Models 

In the Jupyter Notebook [ThreePredictiveModels.ipynb](ThreePredictiveModels.ipynb) ([rendered as html here](ThreePredictiveModels.html)) I investigate a [data set](Data Set Description.md) ([rendered as html here](Data Set Description.html)) gathered to understand which Bank customers are likely to subscribe to a product when targeted during an advertisement campaign. I then create three very different ML models to predict which customers will subscribe based on the other data in the set. The models I use are

 - [X] Linear Regression
 - [X] Random Forest
 - [x] Neural Network

 These particular models were chosen to highlight their respective strengths and weaknesses.

 # Environment Setup

 I use the Jupyter Lab plugin Lux for data exploration, Scikit-Learn for linear regression, and H2O for (categorical) Random Forests. The data set is not checked into git but is assumed to be in the `bank-additional` directory. For convenience, the script `h2o.sh` starts the H2O server. Downloading and unzipping h2o-3.36.1.4.zip will create this directory. You will also need to install `h2b-3.36.1.4/python/h2o-3.36.1.4-py2.py3-none-any.whl` into your virtuanl environment.

**Estimated time spent: ~12 hours**

Much of that time was spent wrestling with SciKit-Learn's pipeline API, which I am not very familiar with. I also wasted a lot of time trying to bootstrap TensorFlow on my machine, but I ultimately gave up.