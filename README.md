# 📊 ANN Classification - Churn Prediction

## 📌 Overview

This project focuses on predicting **customer churn** using an **Artificial Neural Network (ANN)**.
Customer churn prediction is crucial for businesses to identify at-risk customers and take preventive measures to improve customer retention.

By leveraging **deep learning techniques**, this project aims to:

* Build an accurate churn prediction model.
* Provide an interactive **Streamlit web app** for real-world usage.
* Serve as a learning resource for **ANNs, preprocessing, and model deployment**.

---

## 🌟 Objectives

* Develop a **deep learning ANN model** to predict customer churn.
* Perform **data preprocessing** including encoding and scaling.
* Conduct **exploratory data analysis (EDA)** and **hyperparameter tuning**.
* Deploy the solution using a **Streamlit web application**.

---

## 🗂️ Project Structure

```
ANN-Classification-Churn-Prediction/
├── Churn_Modelling.csv        # Dataset used for training and evaluation
├── LICENSE                    # Project license (GPL-3.0)
├── README.md                  # Project documentation
├── app.py                     # Streamlit app for deploying the churn prediction model
├── experiments.ipynb          # Exploratory data analysis & initial model training
├── hyperparametertuning.ipynb # Hyperparameter tuning of the ANN model
├── label_encoder_gender.pkl   # Pre-trained label encoder for Gender
├── model.h5                   # Trained ANN model saved in HDF5 format
├── onehot_encoder_geo.pkl     # Pre-trained one-hot encoder for Geography
├── predictions.ipynb          # Model predictions on sample data
├── requirements.txt           # Project dependencies
└── scaler.pickle              # Pre-trained scaler for data preprocessing
```

---

## 🧐 Model Architecture

The **ANN model** is structured as follows:

* **Input Layer:** Accepts numerical + encoded categorical features.
* **Hidden Layers:**

  * Dense Layer (ReLU activation)
  * Dense Layer (ReLU activation)
* **Output Layer:**

  * Single neuron with **Sigmoid activation** → Binary classification (Churn / No Churn).

---

## 🛠️ Data Preprocessing

* **Label Encoding** → Gender (`Male`, `Female`) → numeric values.
* **One-Hot Encoding** → Geography (`France`, `Germany`, `Spain`) → binary columns.
* **Feature Scaling** → StandardScaler applied to numeric features (`Credit Score`, `Age`, `Balance`, etc.).

---

## 🚀 How to Run the Project

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/venu0807/ANN-Classification-Churn-Prediction.git
cd ANN-Classification-Churn-Prediction
```

### 2️⃣ Install Dependencies

Make sure Python **3.7+** is installed. Then run:

```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Streamlit App

Launch the churn prediction web app:

```bash
streamlit run app.py
```

This will open a local web app where you can **input customer details** and get churn predictions.

### 4️⃣ Explore Jupyter Notebooks

* **experiments.ipynb** → EDA & initial model training.
* **hyperparametertuning.ipynb** → Fine-tuning ANN hyperparameters.
* **predictions.ipynb** → Test model on new data samples.

---

## 📈 Model Performance

* Achieved **\~86% accuracy** on the test dataset.
* Demonstrates effective classification of customer churn.

---

## 📜 License

This project is licensed under the **GPL-3.0 License**.
See the [LICENSE](LICENSE) file for more details.

---

## 🤝 Contributing

Contributions are welcome!
If you’d like to improve the project:

1. Fork the repo.
2. Create a feature branch (`git checkout -b feature-name`).
3. Commit changes (`git commit -m "Add feature"`).
4. Push to the branch (`git push origin feature-name`).
5. Open a Pull Request.

---

## 🔗 Links

* 🗂 [GitHub Repository](https://github.com/venu0807/ANN-Classification-Churn-Prediction)
