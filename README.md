# README: Iris Dataset Classification using K-Nearest Neighbors (KNN)

## Description
This project implements classification on the Iris dataset using the K-Nearest Neighbors (KNN) algorithm. The dataset is split into training and testing sets, and the model's accuracy is evaluated on the test set.

## Features
- **Exploration of the Iris dataset**: Understanding its structure, features, and distribution.
- **Data visualization**: Scatter plot matrix to visualize feature relationships.
- **Implementation of KNN classifier**: Training and testing the model.
- **Evaluation of classification accuracy**.

## Dependencies
Ensure you have the required dependencies installed using:
```bash
pip install numpy pandas scikit-learn matplotlib
```

## Implementation Details
1. **Loading the Iris Dataset**:
   - Fetches the dataset using `sklearn.datasets.load_iris()`.
   - Extracts feature data and target labels.
   
2. **Dataset Exploration**:
   - Prints dataset structure (number of samples, features, and unique class distribution).
   - Visualizes feature relationships using a scatter plot matrix.
   
3. **Splitting Data for Training and Testing**:
   - Uses `train_test_split` to split the data (70% train, 30% test).
   - Stratified sampling ensures equal class distribution.
   
4. **K-Nearest Neighbors (KNN) Classification**:
   - Initializes the `KNeighborsClassifier()` model.
   - Fits the model on training data.
   - Predicts test labels.
   
5. **Model Evaluation**:
   - Computes accuracy as the mean of correct predictions.
   - Prints the accuracy score.

## Notes
- The accuracy may vary slightly depending on the random seed used in data splitting.
- KNN can be further optimized by tuning hyperparameters like `n_neighbors`.
