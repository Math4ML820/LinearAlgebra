# Introduction - Math for Machine Learning

**Machine learning** is a field of study that gives computers the ability to learn, without being explicitly programmed.

## Stages in Machine Learning Pipeline

**Data Processing** - This is where you format the data in a way algorithms can ingest. Uses Linear Algebra.
**Feature Engineering Selection** - This is where you transform the data to make it easy for algorithms to understand. Uses Vectors and Matrices.
**Modeling** - This is where you define the problem in a way the algorithm can optimize. Uses geometry, probability, norms and statistics.
**Optimization** - This is where you iterate until some conditions are met and then you chose the best model.  Uses Vector Calculus.

## An Example to understand how Math is used in Machine Learning

### Data Processing:
- Obtain the animal dataset, which includes information about different animals such as size, weight, habitat, etc.
- Use linear algebra to organize the dataset into rows and columns, forming a structured representation that machine learning algorithms can understand.
- Perform data cleaning, which involves handling missing values, removing outliers, and ensuring data consistency.

### Feature Engineering and Selection:
- Select the relevant features from the dataset that are important for distinguishing mammals from other animals. This involves __domain knowledge__ and understanding of the problem.
- **Transform the selected features** using mathematical operations. For example, if one of the features is the presence of fur, you might represent it as a binary value (0 for no fur, 1 for fur). These transformations help make the data easier for algorithms to process.
Use vectors and matrices to represent and manipulate the transformed features. For example, you can represent each animal as a vector with its feature values, and perform mathematical operations like dot products or matrix operations to analyze the relationships between features.

### Modeling
- Define the problem as a classification task, where the goal is to classify animals as mammals or non-mammals based on their features.
- Choose an appropriate machine learning algorithm for classification, such as logistic regression, decision trees, or support vector machines.
- Use mathematical concepts like geometry, probability, norms, and statistics to train the model. This involves estimating model parameters and optimizing them to fit the data.

### Optimization
- Split the dataset into training and testing sets to evaluate the model's performance.
- Use vector calculus and optimization techniques to iteratively adjust the model's parameters, minimizing a loss function that measures the difference between the predicted outputs and the actual labels.
- Iterate this process until the model's performance reaches a satisfactory level.
- Select the best model based on evaluation metrics, such as accuracy, precision, recall, or F1 score.

### Prediction
- Use the trained model to predict whether a new animal belongs to the mammal class or not based on its features.
- Apply the learned mathematical relationships to the new animal's feature values to make a prediction.
- Evaluate the model's prediction performance on unseen data to assess its generalization ability.

By going through these stages in the machine learning pipeline, we can use mathematics to process, transform, model, and optimize data to make predictions or solve problems in various real-world scenarios, such as predicting whether an animal is a mammal based on its characteristics.

## How Calculus, Probability and Staticstics are used in Machine Learning Pipeline

### Calculus 
- Calculus, specifically vector calculus, can be used in the optimization stage of the machine learning pipeline. It helps in adjusting the model's parameters to minimize a loss function, which measures the difference between the predicted outputs and the actual labels.
- Optimization algorithms, such as gradient descent, utilize calculus to calculate the gradients of the loss function with respect to the model's parameters. These gradients guide the iterative updates to the parameters, aiming to find the optimal values that minimize the loss and improve the model's performance.

### Probability
- Probability theory is used in modeling and making predictions. In this example, probability concepts can be applied to estimate the likelihood of an animal being a mammal based on its observed features.
- The machine learning algorithm can utilize conditional probabilities to calculate the probability of an animal being a mammal given its specific features. This involves estimating the probability distribution of the features for different classes (mammal or non-mammal) and using Bayes' theorem to update the probabilities based on observed evidence.

### Statistics
- Statistics plays a crucial role in various stages of the machine learning pipeline, including data processing, modeling, and evaluation.
- In the data processing stage, statistical techniques can be used to handle missing values, detect and handle outliers, and ensure data consistency.
- When building the model, statistics helps in estimating the parameters of the machine learning algorithm based on the training data. This involves techniques such as maximum likelihood estimation or least squares estimation.
- Statistics also enables the evaluation of the model's performance using metrics like accuracy, precision, recall, or F1 score. These metrics provide statistical measures of how well the model is predicting the correct class labels.