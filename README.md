# 🏆 AI IPL Win Predictor

An interactive web application that predicts the winning probability of an IPL team during a live match using real-time input parameters and machine learning.

## 🎯 Objective
- To build a data-driven and user-interactive tool that enhances IPL viewing by predicting match outcomes in real time using machine learning.

## 📌 Project Description

This project leverages machine learning and real-time match data to predict the outcome of IPL matches. Built with **Streamlit**, it allows users to input live match conditions (like score, overs, wickets, etc.) and outputs the winning probability for both batting and bowling teams. The model is trained using historical IPL data, and predictions are generated using a **Logistic Regression** algorithm encapsulated inside a reusable ML pipeline.

## 🚀 Features

- Predicts win probability based on live match inputs  
- Uses a trained Logistic Regression model for predictions  
- Clean and interactive web interface with visual elements  
- Validates user input (e.g., same team cannot be selected for both roles)  
- Lightweight and runs locally using Streamlit  


## 🧠 Technologies Used

- **Python 3.x**  
- **Streamlit** – for building the web interface  
- **Scikit-learn** – for machine learning model and preprocessing  
- **Pandas** – for data manipulation  
- **Pickle** – to store the ML pipeline  


## 📁 Project Structure
aiipl-win-predictor/ │ ├── app.py # Main Streamlit app file
  ├── pipe.pkl # Saved ML pipeline (preprocessing + model)
  ├── ipl.ipynb # Notebook for data cleaning & model training
  ├── matches.csv # Historical match-level IPL data
  ├── deliveries.csv # Ball-by-ball IPL data
  ├── final_df # Final preprocessed dataset used for training
  ├── requirements.txt # Required Python packages
  
## ⚙️ How to Run
1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/aiipl-win-predictor.git
   cd aiipl-win-predictor

2. **Create a Virtual Environment**
   ```bash
   python -m venv .venv

3. **Activate the Virtual Environment**

- **On Windows:**
```bash
.venv\Scripts\activate
```

- **On macOS/Linux:**
```bash
source .venv/bin/activate
```

4. **Install Dependencies**

```bash
pip install -r requirements.txt
```

5. **Run the App**

```bash
streamlit run app.py
```

The app will open in your default browser. If not, follow the URL printed in the terminal.

## 🧪 Future Improvements
. Integrate live API to fetch ongoing match data automatically
. Improve prediction accuracy with ensemble models (e.g., Random Forest).
. Add charts and historical comparison for user engagement
