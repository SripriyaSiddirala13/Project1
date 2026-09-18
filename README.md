🏠 Real Estate Listing Classifier

Ensemble Text & Visual Anomaly Detection for Authentic Real Estate Listings

A Machine Learning project developed to identify potentially fake or misleading real-estate listings and classify them as Real Listing or Fake Listing using property-related information.

📌 Project Overview

Online real-estate platforms contain a large number of property listings. Some listings may contain misleading information about price, location, property size, amenities, or other details.

This project aims to build a machine-learning based system that can analyze listing information and help identify potentially fake listings.

The project uses an Extra Trees + Artificial Neural Network (ANN/MLP) workflow for feature selection and classification.

🎯 Objectives

Detect potentially fake real-estate listings.

Clean and preprocess real-estate data.

Handle missing values and categorical features.

Identify important features using Extra Trees.

Train a neural-network based classification model.

Evaluate the model using multiple classification metrics.

Save the trained model for future prediction use.

📊 Dataset

The supplied dataset contains:

Property

Value

Total records

2,452

Total columns

21

Target column

False Listing

Real listings

2,154

Fake listings

298

Input features after removing ID and target

19

The dataset contains property-related information used to distinguish between real and potentially false listings.

🔄 Project Workflow

Raw Real Estate Dataset
          ↓
Data Cleaning
          ↓
Missing Value Handling
          ↓
Categorical Encoding
          ↓
Feature Scaling
          ↓
Extra Trees Feature Importance
          ↓
Important Feature Selection
          ↓
ANN / MLP Classification
          ↓
Model Evaluation
          ↓
Saved Model

🧠 Machine Learning Approach

1. Data Preprocessing

The dataset is prepared before model training by:

Handling missing values.

Encoding categorical variables using LabelEncoder.

Standardizing selected numerical features.

Separating input features and target variable.

Splitting the dataset into training and testing data.

2. Feature Selection

Extra Trees Classifier is used to calculate feature importance.

The important features identified by the tree-based model are then used as inputs to the neural-network classifier.

3. Classification Model

The project uses:

Extra Trees Classifier for feature importance.

MLPClassifier (Artificial Neural Network) for classification.

The supplied ANN configuration uses hidden layers of:

128 → 64

📈 Model Evaluation

The project evaluates the classifier using:

Accuracy

Precision

Recall

F1-score

Confusion Matrix

ROC Curve

Recorded Experimental Result

Metric

Result

Accuracy

87.17%

Macro Precision

43.58%

Macro Recall

50.00%

Macro F1-score

46.57%

Note: The dataset is imbalanced, with substantially more real listings than fake listings. Therefore, accuracy should not be considered by itself. The recorded experiment also indicates that class-specific performance needs improvement, particularly for correctly identifying the real-listing class. These results are retained as the original experiment output rather than being overstated.

🛠️ Technologies Used

Python

Pandas

NumPy

Scikit-learn

Matplotlib

Seaborn

Joblib

Jupyter Notebook

📂 Project Structure

Real_Estate_Listing_Classifier/
│
├── source_code/
│   ├── real_estate_listing_classifier.ipynb
│   └── ann_baseline_experiment.ipynb
│
├── dataset/
│   └── real_estate_fake_real_dataset.csv
│
├── model/
│   └── saved model files
│
├── results/
│   ├── confusion matrix
│   └── ROC curve
│
├── Project_Report.pdf
├── requirements.txt
└── README.md

▶️ How to Run the Project

Step 1: Install Python

Install Python 3.x on your system.

Step 2: Install Required Libraries

Open Command Prompt or Terminal and run:

pip install pandas numpy scikit-learn matplotlib seaborn joblib jupyter

Or use:

pip install -r requirements.txt

Step 3: Open Jupyter Notebook

jupyter notebook

Step 4: Open the Main Notebook

Navigate to:

source_code/real_estate_listing_classifier.ipynb

Step 5: Run the Notebook

Run the cells in sequence to:

Load the dataset.

Clean the data.

Encode categorical features.

Scale numerical features.

Perform feature selection.

Train the ANN/MLP model.

Evaluate the model.

Generate evaluation plots.

🔮 Future Scope

The project can be improved by:

Using Stratified Train-Test Split.

Applying class weights or resampling to handle class imbalance.

Using a single saved preprocessing pipeline with the trained model.

Performing hyperparameter tuning.

Improving minority-class precision and recall.

Adding natural-language processing for listing descriptions.

Adding image-based analysis for property photographs.

Developing a web application or API for real-time listing verification.

Connecting the system with a database for storing verified listings.

👩‍💻 Skills Demonstrated

This project demonstrates practical skills in:

Data Cleaning

Data Preprocessing

Feature Engineering

Feature Selection

Machine Learning

Artificial Neural Networks

Model Evaluation

Data Visualization

Python Programming

Model Saving and Deployment Preparation

📜 Conclusion

The Real Estate Listing Classifier demonstrates an end-to-end machine-learning workflow for identifying potentially false real-estate listings.

The project combines Extra Trees feature importance with an ANN/MLP classifier, providing a foundation that can be further improved with class-imbalance techniques, NLP, image analysis, and deployment as a real-time verification application.
