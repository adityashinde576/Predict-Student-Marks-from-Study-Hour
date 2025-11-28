Study Hours vs Marks Prediction using Linear Regression
Project Overview

This project demonstrates a simple Linear Regression model to predict student marks based on the number of hours studied. It is designed as a beginner-friendly machine learning example to understand end-to-end ML workflow:

Data preparation

Model training

Prediction

Visualization

Model evaluation

The dataset is small and synthetic, but the workflow can be applied to larger real-world datasets.

Project Features

Predict marks for given study hours

Visualize actual vs predicted marks using a regression line

Evaluate model performance using:

Mean Squared Error (MSE)

R² Score

Technology Stack

Python 3.x

Libraries:

pandas – for data handling

numpy – for numerical operations

matplotlib – for data visualization

scikit-learn – for linear regression and evaluation metrics

Folder Structure
study-hours-marks-prediction/
│
├── main.py                 # Python script with model code
├── README.md               # This documentation
└── requirements.txt        # Python dependencies

Setup Instructions (VS Code / Local Machine)
1. Clone the Repository
git clone <your-repo-url>
cd study-hours-marks-prediction

2. Create a Virtual Environment (Recommended)
python -m venv venv         # Create virtual environment
source venv/bin/activate    # On Linux/Mac
venv\Scripts\activate       # On Windows

3. Install Dependencies
pip install -r requirements.txt


If requirements.txt does not exist, install manually:

pip install pandas numpy matplotlib scikit-learn

4. Run the Project in VS Code

Open VS Code and open the project folder.

Open main.py.

Run the script:

Using terminal:

python main.py


Or press F5 (Run Python file in VS Code).

How the Code Works

Load Data

The dataset is defined as a dictionary with "Hours_studied" and "Marks" columns.

Converted to a Pandas DataFrame for convenience.

Prepare Features & Target

X → Feature (Hours_studied)

y → Target (Marks)

Reshape X to 2D array for scikit-learn.

Train Linear Regression Model

model.fit(X, y) trains the model.

Coefficients and intercept are printed.

Make Predictions

Predict marks for 5, 9, and 12 study hours.

Can easily modify for other hours.

Visualize

Scatter plot for actual data.

Regression line shows predicted trend.

Evaluate Model

Mean Squared Error (MSE) measures prediction error.

R² Score measures goodness of fit.

Example Output
Dataset:
   Hours_studied  Marks
0              1     35
1              2     40
2              3     50
3              4     60
4              5     70
5              6     75
6              7     85

Model Training Completed.
Slope (m): 8.21
Intercept (b): 29.29

Predictions:
Marks for 5 hours: 70.33
Marks for 9 hours: 103.07
Marks for 12 hours: 127.71

Model Evaluation:
MSE (Mean Squared Error): 8.62
R² Score: 0.98

Dependencies

Python >= 3.8

pandas

numpy

matplotlib

scikit-learn

Create requirements.txt with:

pandas
numpy
matplotlib
scikit-learn

Future Improvements

Allow dynamic input of study hours using input()

Use larger datasets from CSV or Excel

Experiment with Polynomial Regression for non-linear trends

Deploy as a simple web app using Flask or Streamlit

License

This project is open-source and free to use under the MIT License.
