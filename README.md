# CNN-with-Regularisation-techniques
This project explores Convolutional Neural Networks (CNNs) with a focus on regularization techniques,Batch Normalization and weight initializers for preventing overfitting. 

# Key Insights

**Dropout regularization** had the most significant positive impact on both accuracy and loss reduction, indicating its effectiveness in preventing overfitting.
**L1 and L2 regularization** methods also improved model performance, though not like dropout.
**Early stopping**, while preventing overfitting, led to a slightly lower accuracy compared to other methods.

# Dataset Creation
The numerical dataset used in this project is generated using scikit-learn's make_classification function. It consists of 10,000 samples with 100 features. Among these features, 5 are informative, and 15 are redundant. The dataset is designed to showcase the effectiveness of regularization techniques in handling different types of features.

# Regularization Techniques
Several regularization techniques are employed and compared in this project:

* **L1 Regularization (Lasso)**: Encourages sparsity in the model by adding the absolute values of the coefficients as a penalty term.
* **L2 Regularization (Ridge)**: Prevents overfitting by adding the squared values of the coefficients as a penalty term.
* **Dropout**: A technique that randomly drops a fraction of neurons during training, preventing overfitting and promoting robustness.
* **Data Augmentation** : Enhances the training dataset by applying random transformations to input data, effectively increasing the amount of training data.
* **Early Stopping**: stops training when the model's performance on a validation set starts to degrade, preventing overfitting.

# Impact of Regularization Methods on Model Performance
In this project, I have applied various regularization techniques to our Convolutional Neural Network (CNN) model and observed their impacts on model performance. Here's a summary of our findings:  
** Without Regularization **
Accuracy: 90.16%
Loss: 31.64
Without any regularization, our model achieved a respectable accuracy of 90.16%. However, the loss value indicates that the model might be overfitting to the training data.

**Dropout Regularization**
Accuracy: 91.16%
Loss: 23.28
The incorporation of dropout regularization resulted in an accuracy boost to 91.16% and a significant reduction in loss (23.28). Dropout helps prevent overfitting by randomly deactivating neurons during training, leading to a more robust model.

**L1 and L2 Regularization**
Accuracy: 90.56%
Loss: 28.53
Applying L1 and L2 regularization methods yielded an accuracy of 90.56% and reduced the loss to 28.53. These techniques add penalty terms to the model's weights, encouraging simpler and more generalizable representations.

**Early Stopping**
Accuracy: 89.16%
Loss: 31.06
With early stopping, the model achieved an accuracy of 89.16%. Early stopping monitors the model's performance on a validation set and halts training when it starts to degrade. This can prevent overfitting but may result in slightly lower accuracy (because the model cant training with more training data becasue the training is halted whem it starts to overfit).
