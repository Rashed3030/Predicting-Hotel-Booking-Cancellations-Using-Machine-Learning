# Predicting-Hotel-Booking-Cancellations-Using-Machine-Learning

# Hotel Booking Cancellation Predictor

A Streamlit web application that predicts the likelihood of hotel booking cancellations based on booking details.

## Features

- Predicts booking cancellation probability
- User-friendly interface
- Real-time prediction
- Visual explanations of predictions
- Responsive design

## Prerequisites

- Python 3.8+
- pip (Python package manager)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/hotel-booking-app.git
   cd hotel-booking-app
   ```

2. Create a virtual environment (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: .\venv\Scripts\activate
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Running the App

1. First, save your trained model and scaler by running:
   ```bash
   python save_model.py
   ```
   (Make sure to replace the dummy model in `save_model.py` with your actual trained model)

2. Start the Streamlit app:
   ```bash
   streamlit run app.py
   ```

3. Open your browser and navigate to `http://localhost:8501`

## Project Structure

```
hotel-booking-app/
├── app.py                 # Main Streamlit application
├── save_model.py          # Script to save the trained model
├── requirements.txt       # Python dependencies
├── README.md              # This file
└── model/                 # Directory for saved models
    ├── xgboost_model.pkl  # Trained XGBoost model
    └── scaler.pkl         # Fitted StandardScaler
```

## Customization

- **Model**: Replace the dummy model in `save_model.py` with your actual trained model
- **Styling**: Modify the CSS in `app.py` to change the app's appearance
- **Features**: Update the feature engineering in the `preprocess_input` function in `app.py` to match your model's requirements

## Deployment

To deploy this app on Streamlit Sharing or another cloud platform:

1. Push your code to a GitHub repository
2. Sign up for a Streamlit Sharing account (https://share.streamlit.io/)
3. Click "New app" and connect your GitHub repository
4. Select the main branch and set the main file to `app.py`
5. Click "Deploy!"

