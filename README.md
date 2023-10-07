
# Twitter Sentiment analysis

A brief description of what this project does and who it's for


Twitter sentiment analysis is a powerful tool for understanding public opinion and trends on social media. It has applications in marketing, politics, customer service, and many other fields where understanding public sentiment is valuable.
## Acknowledgements

 - https://www.kaggle.com/datasets/jp797498e/twitter-entity-sentiment-analysis/
 


## Appendix

A.1 Data Preprocessing



Data Cleaning: i have  checked for and handled missing values in the dataset, ensuring that no crucial information was lost during the process.

Feature Scaling: i have to standardized the input features to have a mean of 0 and a standard deviation of 1. This scaling was applied to ensure that all features contribute equally to the model's training.

Train-Test Split: The dataset was split into training and testing sets with an 80-20 ratio, respectively. This separation allowed us to evaluate the model's performance on unseen data.


A.2 Model Architecture



Input Layer: The input layer consists of 10 neurons, corresponding to the 10 features in the dataset.

Hidden Layers: The model includes two hidden layers. The first hidden layer has 128 neurons with ReLU activation, and the second hidden layer has 64 neurons with ReLU activation.

Dropout Layer: A dropout layer with a dropout rate of 0.2 was added after the first hidden layer. This layer helps prevent overfitting during training.

Output Layer: The output layer has a single neuron with sigmoid activation, suitable for binary classification tasks.

Optimizer: We used the Adam optimizer with a learning rate of 0.001 to minimize the binary cross-entropy loss function during training.


A.3 Hyperparameter Tuning

The model's hyperparameters were tuned to optimize its performance. Some of the hyperparameters adjusted during tuning include:

Learning Rate: Different learning rates were tested to find an optimal value that balances training convergence and speed.

Number of Epochs: We experimented with the number of training epochs to find a balance between underfitting and overfitting.

Batch Size: Various batch sizes were tested to determine their impact on training.


A.4 Model Evaluation


Confusion Matrix: A confusion matrix was generated to provide insights into the model's performance in terms of true positives, true negatives, false positives, and false negatives.

Precision, Recall, and F1-Score: These metrics were calculated to assess the model's performance in binary classification.


