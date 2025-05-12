# Driver Drowsiness Detection using Eye State Classification

This project is a Machine Learning-based system to detect driver drowsiness using webcam input by monitoring the state of the eyes (open, closed, or not detected). If the eyes remain closed for more than 3 seconds, an alert beep is triggered to wake the driver.

Features
- Eye state classification using a CNN model
- Alerts:
  - **"Eyes Open"**
  - **"Eyes Closed"**
  - **"Eyes Not Detected"**
- Continuous beep sound if eyes are closed for more than 3 seconds
- Trained model (`.h5` file) and pickled feature data included
- Real-time webcam detection

Model
- CNN trained to classify eye state (Open or Closed)
- Model files:
  - `my_model_drowsiness.h5` – final model
  - `mt_model.h5` – initial training model
- Uses `X.pickle` and `y.pickle` for data storage

Folder Structure:
drowsiness_detection_ML_Project/
│
├── drowsiness_detector.ipynb # Main Jupyter notebook
├── my_model_drowsiness.h5 # Trained CNN model
├── mt_model.h5 # Another model (optional)
├── X.pickle, y.pickle # Pickled training data
├── alert/ # Beep sound file
├── data/ # dataset(images)
├── .ipynb_checkpoints/ # Jupyter notebook autosaves


🛠️ Requirements

Install dependencies with:

```bash
pip install opencv-python tensorflow keras numpy matplotlib

pip install playsound
```
📦 How to Run
- Clone the repository or upload the folder.
- Open drowsiness_detector.ipynb in Jupyter Notebook or VS Code.
- Run the cells step by step.
- Ensure webcam is working for real-time detection.

📢 Alert Mechanism
- If eyes are detected as closed for > 3 seconds, a beep sound (alert/beep.wav) is played.
- If eyes are not detected at all, the system warns with "Eyes Not Detected".

🙏 Acknowledgment
This project is based on the tutorial by DeepLearning_by_PhDScholar link: [https://youtu.be/qwUIFKi4V48?si=NtrxgGylRK0Rp63l] and extended with additional alert features.

Enhancements Made:
- Added an alert for "Eyes Not Detected"
- Implemented continuous beep when eyes are closed for more than 3 seconds

