# Diabetes Prediction - Artificial Neural Network (ANN)

This project is an Artificial Neural Network (ANN) model designed to predict the diabetes risk of patients using the Pima Indians Diabetes Dataset. It is developed using TensorFlow and Keras libraries.

## Dataset

The dataset contains diagnostic measurements for 768 female patients:
* Pregnancies
* Glucose
* BloodPressure
* SkinThickness
* Insulin
* BMI (Body Mass Index)
* DiabetesPedigreeFunction
* Age
* Outcome (0: No Diabetes, 1: Diabetes)

## Technologies Used

* Python 3
* TensorFlow / Keras
* Pandas & NumPy (Data Processing)
* Scikit-learn (Preprocessing and Metrics)
* Matplotlib & Seaborn (Visualization)

## Project Steps

1. **Data Preprocessing:**
   * Zero values in specific columns (Glucose, Blood Pressure, etc.) were treated as missing data and filled with the median value of that column.
   * Features were scaled using `StandardScaler`.
   * The dataset was split into 80% training and 20% testing sets.

2. **Model Architecture:**
   * Fully Connected Neural Network.
   * Hidden Layers: Layers with 32, 16, and 8 neurons (ReLU activation).
   * Regularization: Dropout layers were added to prevent overfitting.
   * Output Layer: 1 neuron (Sigmoid activation).

3. **Training:**
   * Optimizer: Adam
   * Loss Function: Binary Crossentropy
   * Epochs: 100

## Results

The model was evaluated on the test set:
* **Test Accuracy:** ~73%
* **Evaluation:** Performance was analyzed using Confusion Matrix, Classification Report, and ROC-AUC score.
