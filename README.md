# ECG_Project_Code-

ECG-Based Irregular Heart Rhythm Screening Using AI

1. Project Overview

This project is an AI-assisted ECG monitoring system designed to record electrocardiogram (ECG) signals, process them, and identify patterns that may indicate irregular heart rhythms. It combines hardware-based signal acquisition with machine learning to provide preliminary screening results for educational purposes, not medical diagnosis.

2. Project Workflow

The system uses a Raspberry Pi Pico W connected to an AD8232 ECG sensor to acquire electrical heart signals. The recorded data is transmitted wirelessly to a computer, where Python processes and analyzes the signal using filtering techniques, R-peak detection, and RR-interval feature extraction. A trained machine learning model evaluates the extracted features and classifies the recording.

3. Main Files

- "main.py": Records ECG signals and sends data through Wi-Fi.
- "server.py": Receives recordings and runs the analysis.
- "ecg_utils.py": Handles signal processing, feature extraction, and classification.
- "train_model.py": Prepares the dataset and trains the AI model.
- "ecg_model.joblib": Stores the trained model and classification threshold.
- "app.py": Provides an interactive Streamlit dashboard.
- "filteration.py": Demonstrates ECG filtering and peak detection.
- "features.csv": Stores extracted training features.

4. Running the Project

Install the required Python libraries, configure the Wi-Fi credentials and server IP in "main.py", then start the server using "python server.py". Run the Pico W recording program and launch the dashboard using "streamlit run app.py".

5. References

- "PhysioNet 2017 Challenge" (https://physionet.org/content/challenge-2017/1.0.0/)
- "Raspberry Pi Documentation" (https://www.raspberrypi.com/documentation/)
- "Streamlit Documentation" (https://docs.streamlit.io/)

Disclaimer: This project is an educational screening tool and is not intended to replace professional medical evaluation.
