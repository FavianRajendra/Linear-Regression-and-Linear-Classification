Iris Dataset: Perceptron and Linear Regression Binary Classification

This repository contains a detailed Jupyter Notebook (Iris.ipynb) demonstrating the fundamental concepts of machine learning by implementing two classic classification algorithms from scratch: the Perceptron and a Linear Regression model for binary classification.

The project uses the classic Iris flower dataset as the foundation for exploring data preparation, model training, and performance evaluation.

🌟 Project Goals

Implement Core Algorithms from Scratch: Define and implement the Perceptron and Linear Regression (used as a binary classifier) algorithms using only fundamental Python libraries (NumPy) for a deep understanding of their mechanics.

Binary Classification Focus: Transform the multi-class Iris dataset into a binary classification problem for both model implementations.

Data Preprocessing: Demonstrate essential steps like feature scaling and label encoding.

Performance Visualization: Evaluate and visualize model performance using metrics and the decision boundary plot.

🛠️ Implementation Details

The notebook is divided into distinct phases:

1. Data Acquisition & Preprocessing

Dataset: Uses the iris.csv dataset, which contains features like Sepal Length/Width and Petal Length/Width.

Encoding: The categorical Species column is converted to numerical labels using LabelEncoder.

Binary Conversion: The three species (Iris-setosa, Iris-versicolor, Iris-virginica) are intentionally collapsed into a two-class problem (0 and 1), making it suitable for the binary classifiers.

Train/Test Split: Data is split 80/20 for training and testing with random_state=42 for reproducibility.

Standardization: Features are scaled using StandardScaler to ensure optimal model convergence.

2. Custom Perceptron Implementation (Binary Classification)

A custom Perceptron class is defined and trained on a subset of the Iris features.

Training: The fit method uses iterative updating of weights (w) and bias (b) based on prediction errors and a defined learning_rate and max_epochs.

Evaluation: The model achieves perfect classification on the simplified binary task, with an Accuracy, Precision, Recall, and F1 Score of 1.00. A confusion matrix is also generated.

3. Custom Linear Regression for Binary Classification

A second implementation focuses on using Linear Regression combined with a Sigmoid Activation Function to perform logistic-style binary classification.

Sigmoid Function: The core sigmoid function is defined to map linear outputs to probabilities between 0 and 1.

Gradient Descent: The fit method utilizes gradient descent to minimize the error between predicted probabilities and true labels.

Results: This classifier also demonstrates strong performance on the simplified binary problem, achieving 1.00 accuracy on both the training and test sets.

4. Visualization

The notebook includes a scatter plot showing the data distribution and a visualization of the decision boundary created by the custom Linear Regression model (using only the first two features for 2D plotting).

🚀 How to Run the Notebook

Prerequisites: Ensure you have Python installed along with the following libraries:

numpy

pandas

scikit-learn (sklearn)

matplotlib

seaborn

Dataset: Make sure the iris.csv file is in the same directory as the notebook.

Execution: Open the Iris.ipynb file in a Jupyter environment and run the cells sequentially.
