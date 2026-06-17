Iris Flower Classification using Random Forest
Project Overview

This project uses the Iris Dataset to build a Machine Learning model that classifies iris flowers into different species based on their sepal and petal measurements.

The model is trained using the Random Forest Classifier from Scikit-learn and achieves high prediction accuracy.

Dataset

The dataset contains the following features:

Id
SepalLengthCm
SepalWidthCm
PetalLengthCm
PetalWidthCm
Species (Target Variable)

The species include:

Iris-setosa
Iris-versicolor
Iris-virginica
Technologies Used
Python
Pandas
Scikit-learn
Matplotlib
Google Colab
Project Steps
1. Import Dataset

The Iris dataset is uploaded and loaded using Pandas.

df = pd.read_csv("Iris.csv")
2. Data Preprocessing

Separate the features and target variable.

X = df.drop("Species", axis=1)
y = df["Species"]
3. Split Dataset

The dataset is divided into training and testing sets.

train_test_split()
4. Train Model

A Random Forest Classifier is used for training.

model = RandomForestClassifier(random_state=42)
model.fit(X_train, y_train)
5. Make Predictions

Predict species for the test dataset.

y_pred = model.predict(X_test)
6. Evaluate Model

Calculate model accuracy.

accuracy_score(y_test, y_pred)
7. Data Visualization

A scatter plot is created to visualize the relationship between Sepal Length and Petal Length.

plt.scatter(df["SepalLengthCm"], df["PetalLengthCm"])
Output

Model Accuracy:

Accuracy: 1.0

Visualization:

Scatter Plot of Sepal Length vs Petal Length
How to Run
Upload the Iris.csv dataset.
Open the notebook in Google Colab or Jupyter Notebook.
Run all cells sequentially.
View the model accuracy and visualization results.
Future Improvements
Compare multiple machine learning algorithms.
Add confusion matrix and classification report.
Deploy the model as a web application.
Perform hyperparameter tuning for better performance.

Machine Learning Mini Project using the Iris Dataset.
