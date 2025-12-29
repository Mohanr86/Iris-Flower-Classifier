# 🌸 Iris Flower Classification Web Application

## 🧠 1. Abstract

The **Iris Flower Classification Web Application** is a machine learning-based tool designed to automate the identification of Iris flower species. By leveraging the Iris dataset and a supervised learning approach, the application classifies flowers into three species: **Setosa, Versicolor, and Virginica**. The project integrates a trained Scikit-learn model with an interactive **Streamlit** frontend, providing a seamless, real-time prediction experience.

---

## 🚀 Live Demo

🔗 **Access the live application here:**  
**https://iris-flower-classifier-j6lkotxkbeprd6natqx4vh.streamlit.app/**

---

## 🖼️ Application Preview


> ![image](https://github.com/Mohanr86/repo/assets/demo.png)


---

## ✨ 2. Key Features

- **Real-time Prediction:** Instant classification results upon adjusting input parameters.
- **Interactive UI:** Uses sliders for precise numerical input of flower attributes.
- **Lightweight Architecture:** Minimalistic backend ensuring fast load times.
- **Responsive Design:** Optimized for various screen sizes via the Streamlit framework.
- **Model Persistence:** Utilizes serialized `.pkl` files for efficient model loading without retraining.

---

## 🛠️ 3. Technology Stack

| **Layer**               | **Technology**                     |
| ----------------------- | ---------------------------------- |
| Frontend / Backend      | Streamlit (Python-based framework) |
| Machine Learning        | Scikit-learn, NumPy, Pandas        |
| Model Serialization     | Joblib / Pickle                    |
| Environment             | Python 3.8+                        |

---

## 🏗️ 4. System Architecture & Workflow

The application follows a standard **Model–View–Controller (MVC)** influenced workflow:

1. **User Input:** Users provide flower measurements (Sepal & Petal length/width) via Streamlit sliders.
2. **Data Processing:** Inputs are captured as a NumPy array and reshaped for model compatibility.
3. **Model Inference:** The pre-trained `.pkl` model processes the input data to predict the class.
4. **Output Display:** The predicted Iris species is displayed instantly on the UI.

---

## 📊 5. Dataset & Model Details

### 🌼 Iris Dataset

- Contains **150 samples** with **4 numerical features**:
  - Sepal Length
  - Sepal Width
  - Petal Length
  - Petal Width

### 🤖 Prediction Model

- Uses a **Supervised Machine Learning algorithm** (e.g., Logistic Regression / Random Forest).
- Trained offline and saved as `iris_model.pkl`.
- Ensures fast inference during deployment without retraining.

---

## 📁 6. Project Structure

```
Iris-Classifier/
├── app.py                # Main Streamlit application
├── iris_model.pkl        # Trained ML model
├── requirements.txt      # Python dependencies
├── README.md             # Project documentation
└── assets/
    └── demo.png          # Application screenshot
```

---

## ⚙️ 7. Installation & Usage

### ✅ Prerequisites

- Python 3.8 or above

### 🔧 Setup Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/iris-classifier.git
   cd iris-classifier
   ```

2. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Application**
   ```bash
   streamlit run app.py
   ```

---

## ✅ 8. Conclusion

This project demonstrates the complete lifecycle of a machine learning application—from model training to real-time deployment. It serves as an excellent academic and practical example of integrating ML models with modern web interfaces using Streamlit.

---

## 📚 References

- Scikit-learn Documentation
- Streamlit Official Docs
- UCI Machine Learning Repository – Iris Dataset

