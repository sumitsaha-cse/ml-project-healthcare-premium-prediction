# 🏥 Health Insurance Premium Predictor

Hey there! 👋 Welcome to my Health Insurance Premium Predictor. 

This is a Machine Learning project I built to estimate health insurance costs. Have you ever wondered how much your health insurance might cost based on factors like your age, whether you smoke, or your medical history? This app takes all those details and gives you a data-driven estimate in seconds!

## ✨ What it does
* **Keeps things simple:** I used Streamlit to build a clean, interactive webpage where you can just plug in your info and hit predict. No complicated setups required.
* **Smart predictions under the hood:** The app actually uses two different Machine Learning models (trained using XGBoost). It routes younger people and older people to different models to make sure the predictions are as accurate as possible!
* **Looks at the whole picture:** It calculates your premium based on age, BMI, medical history (like diabetes or heart disease), smoking habits, and even the region you live in.

## 🛠️ What I used to build it
* **Python** for pretty much everything.
* **Streamlit** to turn the Python scripts into a web app.
* **Scikit-learn & XGBoost** for training the brains of the operation.
* **Pandas & NumPy** for crunching and cleaning the data.
* **Joblib** to save and load the trained models.

## 🚀 Want to run it on your own computer?

If you want to play around with the code yourself, it's super easy to set up!

1. **Grab the code:**
   ```bash
   git clone https://github.com/sumitsaha-cse/ml-project-healthcare-premium-prediction.git
   cd ml-project-healthcare-premium-prediction
   ```

2. **Install the required libraries:**
   (I highly recommend doing this inside a virtual environment!)
   ```bash
   pip install -r requirements.txt
   ```

3. **Fire it up:**
   ```bash
   streamlit run main.py
   ```
   Your browser should automatically pop open a new tab at `http://localhost:8501` with the app running.

## 📁 How the code is organized
* `main.py`: This is the Streamlit app itself—the sliders, buttons, and layout you see on the screen.
* `prediction_helper.py`: The behind-the-scenes worker. It scales the user's input and asks the saved models to make a prediction.
* `artifacts/`: A folder holding the pre-trained models and data scalers (the `.joblib` files).
* `requirements.txt`: A simple list of all the Python packages you need to run the app.

## 🙏 Big Thanks!
A quick shoutout to the amazing ML course by [codebasics.io](https://codebasics.io/) which guided the creation of this project.