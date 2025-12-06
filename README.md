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


🔧 Technologies Used

Python

TensorFlow / Keras

NumPy, Pandas, Scikit-learn

MATNILM architecture

Google Colab

Google App Script

Blynk IoT Platform

📊 Dataset

Dataset includes:

Date

Time

Total Power (W)

Total Current (A)

Individual appliance power (M1, M2, M3, M4)

🧠 Model Training

The MATNILM model was adapted for this dataset.
Training steps are available in:
notebook folder

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


🙏 Credits

This project uses and extends the MATNILM model from the following repository:

MATNILM by jxiong22
GitHub: https://github.com/jxiong22/MATNilm

I have modified the code to match my dataset and deployment pipeline.


✉️ Contact

If you want to discuss this project or collaborate:
Md Istiauk Hossain Rifat — istiaukhossain@gmail.com
