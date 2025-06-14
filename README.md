# Diabetes_Prediction
A machine learning project to predict the likelihood of diabetes using health-related data and classification algorithms.

## ⚙️ How to Run the Code Without Hassle in google colab

Follow the steps below to get started easily:

1. 📥 **Run the following cell in the notebook:**

   ```python
   from google.colab import files
   files.upload()
2.🔐 Upload your Kaggle token (kaggle.json) when prompted.

3.✅ Now the code is ready to run — all necessary permissions and access will be set up!

## ⚙️ How to Set Up the Project Locally (Kaggle API Method)

Follow these steps if you want to use the Kaggle API to download the dataset directly:

1. 🔑 **Get Your Kaggle API Credentials**  
   - Go to your [Kaggle Account Settings](https://www.kaggle.com/account)
   - Click on **"Create New API Token"**
   - This will download a file called `kaggle.json`

2. 📁 **Place the Token File**  
   - Move `kaggle.json` to the `.kaggle` folder:
     - On Windows: `C:\Users\<YourUsername>\.kaggle\kaggle.json`
     - On macOS/Linux: `~/.kaggle/kaggle.json`

3. 🧠 **Use the Following Code to Programmatically Download the Dataset**

   ```python
   import os
   import kaggle

   # Set Kaggle credentials (optional if kaggle.json is correctly placed)
   os.environ['KAGGLE_USERNAME'] = 'your_username'
   os.environ['KAGGLE_KEY'] = 'your_key'

   # Download and unzip the dataset
   kaggle.api.dataset_download_files('dataset', path='.', unzip=True)
## 📌 Project Highlights

- ✅ Binary classification to detect diabetes (Yes/No)
- 📊 Data preprocessing including handling missing values and scaling
- 🧠 Trains multiple models: Logistic Regression, Decision Tree, Random Forest, XGBoost
- ⚖️ Handles class imbalance using SMOTE
- 🔍 Evaluates models with accuracy, confusion matrix, and classification report
- 📦 Saves trained model using Pickle for real-time predictions

---

## 🧠 Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Matplotlib, Seaborn
- Imbalanced-learn (SMOTE)
- Pickle

---

## 🧪 Example Use Case

The model can predict diabetes likelihood given inputs such as:
- Glucose level
- BMI
- Age
- Blood pressure
- Insulin
- Skin thickness

---

## 📌 Future Improvements

- Add a web interface using Streamlit or Flask
- Apply hyperparameter tuning
- Use advanced ensemble models for better accuracy
