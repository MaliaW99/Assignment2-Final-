# NANO706 — Assignment 2

## Exercise 2, Part 1: Wine Classification

### Project Overview

This exercise uses machine learning to classify wine samples based on their chemical characteristics. Three classification models were evaluated: Support Vector Machine (SVM), Decision Tree, and Logistic Regression.

The goal was to visualize the dataset, train the classification models, evaluate their accuracy, and compare their performance.

### Dataset Visualization

The Wine dataset contains three wine classes and multiple chemical features. A scatter plot was created to examine the relationship between alcohol content and malic acid.

![Wine Dataset Scatter Plot](graphs/wine_dataset_scatter_plot.png.png)

**Results:** The scatter plot shows some separation between the three wine classes, although several samples overlap. This suggests that alcohol and malic acid provide useful information for classification, but additional chemical features can help distinguish the classes.

### Data Preprocessing and Testing

The dataset was divided into training and testing sets using a 70/30 split with `random_state=42`.

Standardization was performed after splitting the dataset. The scaler was fitted using only the training data and then applied to the testing data to prevent data leakage.

Each classification model was trained using the training set and evaluated using the testing set.

### Machine Learning Model Results

| Model | Test Accuracy |
|---|---|
| Support Vector Machine (SVM) | 98% |
| Decision Tree | 96% |
| Logistic Regression | 98% |

### Model Accuracy Comparison

![Wine Classification Accuracy Comparison](graphs/wine_model_accuracy_comparison.png.png)

**Results:** SVM and Logistic Regression achieved the highest accuracy at 98%, while Decision Tree achieved 96%.

All three models demonstrated strong classification performance. The results indicate that the Wine dataset's chemical features are useful for distinguishing between the three wine classes.

### Conclusion

This exercise demonstrated how machine-learning algorithms can classify samples using chemical measurements. SVM and Logistic Regression performed slightly better than Decision Tree on the selected test set. Correct preprocessing helped ensure that the testing data did not influence the standardization of the training data.

### Exercise 2, Part 2

To be completed.
