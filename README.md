# Iris-Classification-Using-kNN
# Iris Flower Species Classification Using k-Nearest Neighbors (kNN)

## Project Overview

This project focuses on classifying Iris flowers into three species using the **k-Nearest Neighbors (kNN)** machine learning algorithm.

The model uses four flower measurements to predict the species:

- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

The three species are:
1. Iris Setosa
2. Iris Versicolor
3. Iris Virginica

## Objectives

- Understand the k-Nearest Neighbors algorithm.
- Implement a supervised machine learning classification model.
- Train and test the model using the Iris dataset.
- Evaluate model performance using accuracy and a confusion matrix.
- Identify correct and incorrect predictions.

## Dataset

The project uses the built-in Iris dataset from Scikit-learn.

| Property | Description |
|---|---|
| Total samples | 150 |
| Features | 4 |
| Classes | 3 |
| Samples per class | 50 |
| Dataset type | Classification |

## Technologies Used

- Python
- NumPy
- Pandas
- Scikit-learn
- Jupyter Notebook / Google Colab

## Algorithm: k-Nearest Neighbors

kNN is a supervised machine learning algorithm that classifies a new data point based on the majority class of its nearest neighbours.

**Euclidean Distance Formula:**

\[
d(x,y)=\sqrt{\sum_{i=1}^{n}(x_i-y_i)^2}
\]

In this project:
- k = 5
- Distance metric = Euclidean
- Train-test split = 80:20
- Feature scaling = StandardScaler

## Project Workflow

1. Import the required libraries.
2. Load the Iris dataset.
3. Separate features and target labels.
4. Split the dataset into training and testing data.
5. Standardize the features.
6. Train the kNN classifier.
7. Predict flower species.
8. Evaluate the model using performance metrics.

## Model Performance

The model was evaluated using a test set of 30 samples.

| Metric | Result |
|---|---:|
| Test Accuracy | 93.33% |
| Correct Predictions | 28 |
| Incorrect Predictions | 2 |
| k Value | 5 |

### Confusion Matrix

```text
[[10  0  0]
 [ 0 10  0]
 [ 0  2  8]]
```

The model correctly classified all Setosa and Versicolor test samples. Two Virginica samples were incorrectly classified as Versicolor.

## Installation

Install the required Python libraries:

```bash
pip install numpy pandas scikit-learn
```

## How to Run

1. Clone this repository:

```bash
git clone https://github.com/your-username/iris-knn-classification.git
```

2. Open the project folder:

```bash
cd iris-knn-classification
```

3. Run the Python file:

```bash
python iris_knn.py
```

You can also run the code using Google Colab or Jupyter Notebook.

## Project Structure

```text
Iris-kNN-Classification/
│
├── iris_knn.py
├── README.md
└── requirements.txt
```

## Applications

- Flower species identification
- Botanical research
- Machine learning education
- Pattern recognition
- Classification problems

## Conclusion

This project demonstrates how the k-Nearest Neighbors algorithm can classify Iris flower species using their physical measurements. The model achieved **93.33% test accuracy** with five nearest neighbours. It demonstrates that kNN is a simple and effective algorithm for classification tasks.

## References

1. R. A. Fisher, "The Use of Multiple Measurements in Taxonomic Problems," *Annals of Eugenics*, vol. 7, no. 2, pp. 179–188, 1936.
2. Scikit-learn Documentation: https://scikit-learn.org/
3. Iris Dataset: https://scikit-learn.org/stable/datasets/toy_dataset.html

---

**Author:** SURYA TEJA K  
**Roll Number:** AP24110011287

**Project:** Iris Flower Species Classification Using kNN
