# 🚗 Autonomous Driving Safety Predictor Using Raw Sensor Data and Pre-Engineered Features

## 📜 Project Overview

This project focuses on building a **machine learning model** to predict **safety-critical scenarios** in autonomous driving using both **raw sensor data** and **pre-engineered features**. By leveraging data from accelerometer and gyroscope sensors, we engineered various statistical features and used them to train an **XGBoost Classifier** and **timeseries forescasting**. The model is designed to detect potential safety issues, making it a critical component for autonomous driving systems, which aim to enhance road safety.

### 🚀 Why This Project Matters

Autonomous driving is at the forefront of future transportation, but ensuring safety remains the biggest challenge. By using machine learning to predict dangerous scenarios in real-time, this project contributes to a safer driving experience. The project showcases:

- Feature engineering on raw sensor data (gyroscope and accelerometer readings).
- Use of **XGBoost**, a powerful machine learning algorithm, to classify safety-critical scenarios.
- Comparison between raw sensor data and pre-engineered feature sets to understand the importance of feature engineering.
- A starting point for developers, data scientists, and researchers who want to contribute to autonomous driving safety through machine learning.

---

## 📂 Project Structure

```plaintext
├── data/                           # Folder for storing raw and pre-engineered datasets
│   ├── features_14.csv              # Pre-engineered features from sensor data
│   ├── sensor_raw.csv               # Raw sensor data
│   ├── sero_features_4.csv          # Pre-engineered features (sero_features 4-20)
│   ├── sero_features_5.csv
│   ├── sero_features_6.csv
│   ├── sero_features_7.csv
│   ├── sero_features_8.csv
│   ├── sero_features_9.csv
│   ├── sero_features_10.csv
│   ├── sero_features_11.csv
│   ├── sero_features_12.csv
│   ├── sero_features_13.csv
│   ├── sero_features_14.csv
│   ├── sero_features_15.csv
│   ├── sero_features_16.csv
│   ├── sero_features_17.csv
│   ├── sero_features_18.csv
│   ├── sero_features_19.csv
│   ├── sero_features_20.csv
├── PreEngineered_Features.ipynb                        # Notebook of Project using Pre Engineered Features data
├── Raw_Sensor_Data.ipynb                        # Notebook of Project using raw sensor data
├── README.md                        # Project documentation (this file)
├── requirements.txt                 # Python dependencies
└── LICENSE                          # License file

```

---

## 🔧 Setup Instructions

### 1. **Clone the Repository**

To get started, clone this repository to your local machine using:

```
git clone https://github.com/GudiVaraprasad/Autonomous-Driving-Safety-Predictor.git
cd Autonomous-Driving-Safety-Predictor
```

### 2. **Install Dependencies**

Install the necessary dependencies using `pip`. It's recommended to create a virtual environment before installing them.

```bash
pip install -r requirements.txt
```

### 3. **Run Jupyter Notebooks**

The entire project has been executed and documented in a Jupyter notebook. To run the notebook:

```bash
jupyter notebook PreEngineered_Features.ipynb

jupyter notebook Raw_Sensor_Data.ipynb
```

---

## 💻 Running the Project

### **Dataset**

- **sensor_raw.csv**: Contains the raw accelerometer and gyroscope data.
- **sero_features_19.csv**: Contains pre-engineered features, which are statistical summaries (mean, variance, etc.) derived from the raw sensor data.

### **Steps**:

1. **Feature Engineering**:
   - If working with raw sensor data, manually engineer statistical features such as mean, variance, skewness, etc.
   - For pre-engineered data, load the features directly.
2. **Data Splitting**:

   - Split the data into training (80%) and testing (20%) sets.

3. **Model Training**:

   - Train the XGBoost classifier on the training set, and evaluate its performance on the test set.

4. **Model Evaluation**:
   - Generate performance metrics such as accuracy, precision, recall, and F1-score to understand model performance.

---

## 📊 Results

- **Test Accuracy**: 97% (for raw data)
- **Test Accuracy**: 100% (for prefeatured data)

---

## 📚 Learn More

If you're new to autonomous driving and machine learning, here are some great resources to help you learn more:

- [XGBoost Documentation](https://xgboost.readthedocs.io/en/stable/)
- [CARLA Autonomous Driving Simulator](https://carla.readthedocs.io/en/latest/)
- [Scikit-learn: Machine Learning in Python](https://scikit-learn.org/stable/)

---

## 🤝 How to Contribute

We welcome contributions from the community! If you'd like to contribute, here's how you can help:

1. **Fork the Repository**: Click the "Fork" button on the top right of the repository page and clone your fork to your local machine.
2. **Create a Branch**: Create a new feature branch for your contribution.
   ```bash
   git checkout -b feature-branch
   ```
3. **Make Your Changes**: Implement your feature, fix bugs, or improve the code.
4. **Submit a Pull Request**: Once your changes are ready, submit a pull request to the `main` branch.

---

## 🛠️ Future Work

Some potential areas of improvement and next steps for the project:

- **Hyperparameter Tuning**: Further optimize the XGBoost model to achieve better accuracy using RandomizedSearchCV or GridSearchCV.
- **Real-Time Deployment**: Integrate the model into an autonomous driving simulation to test predictions in real-time.
- **Expand Dataset**: Use more diverse sensor data to generalize the model for broader use cases.

---

## ✨ Acknowledgments

We'd like to thank the open-source community and the creators of libraries like XGBoost, Scikit-learn, and Jupyter, without which this project would not be possible.

---

## 📬 Contact

For any questions, feel free to reach out:

- **Vara Prasad Gudi**
- [gudi.varaprasad@gmail.com](mailto:gudi.varaprasad@gmail.com)
- Connect on my [LinkedIn](https://www.linkedin.com/in/varaprasad-gudi/)

---
