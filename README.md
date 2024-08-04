# 🌳 MNIST Dataset - PCA and Decision Custom-Decision-Tree-Implementation
Welcome to the MNIST Dataset project focusing on classes 0, 1, and 2. This repository contains code and documentation to perform a series of tasks on the MNIST dataset, specifically reducing dimensions using PCA and implementing a decision tree without using libraries that automatically handle the fitting and prediction processes. Let's get started! 🚀

## 📁 Dataset

Use the [MNIST dataset](https://storage.googleapis.com/tensorflow/tf-keras-datasets/mnist.npz) for the following tasks, focusing on classes 0, 1, and 2.

## 🧩 Task 1: Principal Component Analysis (PCA)

1. **Apply PCA** and reduce the dimension to **p = 10**.
2. Use the entire training set of these 3 classes to obtain the PCA matrix.
3. For the remaining tasks, use the reduced dimension dataset.

## 🌲 Task 2: Decision Tree Learning

1. **Learn a Decision Tree** using the training set.
   - Grow a decision tree with **3 terminal nodes**.
   - For the first split, consider all **p dimensions**.
   - For each dimension, consider one split which will divide the space into two regions.
   - Calculate the total **Gini index** for each split.
   - Find the best split by searching for the minimum Gini index.
   - Repeat the steps to find the best split and divide the p-dimensional space into three regions.

## 🧪 Task 3: Class Prediction on Test Set

1. **Predict the Class** of all samples in the test set of these 3 classes.
   - For a particular test sample, check where the sample lies in the segmented space.
   - The class for a particular sample is the class of the sample which is in majority in the region to which the test sample belongs.
2. **Report Accuracy**:
   - Overall accuracy.
   - Class-wise accuracy for the testing dataset.

## 🛠️ Task 4: Bagging

1. **Develop 5 Different Datasets** from the original dataset.
2. **Learn Trees** for all these datasets.
3. For test samples, use **majority voting** (at least 3 trees should predict the same class) to find the class of a given sample.
   - In case of a tie (e.g., two trees predict one class and two trees predict another class), you can choose either of the classes.
4. **Report Accuracy**:
   - Total accuracy.
   - Class-wise accuracy.


## 🤝 Contributing
Feel free to open issues or submit pull requests if you have any suggestions or improvements.

## 📄 License
This project is licensed under the MIT License.
