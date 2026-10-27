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

## Exercise 2, Part 2: MNIST Classification and YOLO Object Detection

### Project Overview

This exercise explores two applications of machine learning: handwritten-digit classification using the MNIST dataset and object detection using YOLOv5.

### Part A: MNIST Handwritten-Digit Classification

The MNIST dataset contains 70,000 images of handwritten digits ranging from 0 to 9. Three machine-learning models were trained and evaluated to compare their ability to classify handwritten digits.

The models included Random Forest, Logistic Regression, and a Multilayer Perceptron (MLP) Neural Network.

### MNIST Classification Results

| Model | Test Accuracy |
|---|---|
| Random Forest | 96.75% |
| Logistic Regression | 92.02% |
| MLP Neural Network | 97.55% |

### MNIST Accuracy Comparison

![MNIST Classification Model Accuracy Comparison](graphs/mnist_model_accuracy_comparison.png)

**Results:** The MLP Neural Network achieved the highest classification accuracy at 97.55%, followed by Random Forest at 96.75% and Logistic Regression at 92.02%.

These results demonstrate that all three models performed well in recognizing handwritten digits. The MLP Neural Network achieved the strongest performance on the test dataset.

### Part B: YOLO Object Detection

The YOLOv5 object detection model was used to analyze an uploaded photograph containing a person.

The model successfully detected the person and generated a bounding box around the subject with a confidence score of 0.58 (58%).

### YOLO Detection Results

![YOLO Person Detection](graphs/yolo_person_detection.png)

**Results:** The model successfully identified a person within the uploaded image. The bounding box indicates the detected object's location, while the confidence score represents the model's confidence in that detection.

Although the model detected the person, it did not specifically identify the face because the pretrained YOLOv5 model performs general object detection rather than dedicated facial detection.

### Conclusion

Exercise 2 demonstrated two important applications of machine learning. The MNIST classification task compared three models for recognizing handwritten digits, with the MLP Neural Network achieving the highest accuracy. The YOLO object detection task demonstrated how deep-learning-based computer vision can identify and locate objects within an image.

Together, these exercises provided practical experience in classification, model evaluation, and object detection.
