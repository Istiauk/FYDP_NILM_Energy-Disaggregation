# FYDP_NILM_Energy-Disaggregation
Non-Intrusive Load Monitoring using MATNILM + Custom Dataset + Blynk Deployment

This project implements a complete NILM (Non-Intrusive Load Monitoring) pipeline using the MATNILM model.
The model is trained using a custom multi-appliance dataset, and deployed for real-time monitoring through Google Sheets → Model → Blynk App.

📌 Features

✔ Power disaggregation for multiple appliances

✔ Real-time prediction using trained MATNILM model

✔ Google Sheets input → Python backend → Blynk output

✔ Jupyter notebooks for training & deployment

✔ Fully documented dataset and working colab files

✔ Clean modular project structure

✔ Includes credits to the original MATNILM repository

📁 Project Structure
NILM-Disaggregation-Project/
│
├── README.md
│
├── dataset/                  
│   ├── my_dataset.csv
│   ├── data_description.md
│   └── raw/ , processed/ (optional)
│
├── notebooks/
│   ├── training_notebook.ipynb       # Modified MATNILM training code
│   ├── realtime_blynk.ipynb          # Google Sheet → Prediction → Blynk
│   └── model_architecture_notes.md
│
├── models/
│   ├── trained_model.h5
│   └── scaler.pkl
│
├── deployment/
│   ├── google_sheet_script.txt       # Example Google Script
│   ├── blynk_api_usage.md
│   └── requirements.txt
│
├── images/
│   ├── workflow_diagram.png
│   ├── training_loss_plot.png
│   ├── prediction_example.png
│   └── blynk_screenshot.png
│
└── CITATION.md / LICENSE

🔧 Technologies Used

Python

TensorFlow / Keras

NumPy, Pandas, Scikit-learn

MATNILM architecture

Google Colab

Google App Script

Blynk IoT Platform

📊 Dataset

Your dataset includes:

Date

Time

Total Power (W)

Total Current (A)

Individual appliance power (M1, M2, M3, M4)

A detailed explanation is included in:
dataset/data_description.md

🧠 Model Training

The MATNILM model was adapted for this dataset.
Training steps are available in:
notebooks/training_notebook.ipynb

✔ Preprocessing
✔ Normalization
✔ Train/validation split
✔ Training curve plots
✔ Final model saved in /models/

⚡ Real-time Deployment (Google Sheets → Blynk)

Real-time workflow:

User input → Google Sheets  
↓
App Script sends data to backend  
↓
Python model loads trained_model.h5  
↓
Predicted appliance power  
↓
Sent to Blynk (Virtual Pins)


Relevant files:

deployment/google_sheet_script.txt

deployment/blynk_api_usage.md

notebooks/realtime_blynk.ipynb

🙏 Credits

This project uses and extends the MATNILM model from the following repository:

MATNILM by jxiong22
GitHub: https://github.com/jxiong22/MATNilm

I have modified the code to match my dataset and deployment pipeline.

📜 License

If required, add a LICENSE file such as MIT or Apache-2.0.

✉️ Contact

If you want to discuss this project or collaborate:
Your Name — your email here
