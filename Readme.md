# 🌸 Iris Flower Classification Web Application

## 1. Abstract


The **Iris Flower Classification Web A## 🧠 1. Abstracts a machine learning-based tool designed to automate the identification of Iris flower species. By leveraging the Iris dataset and a supervised learning approach, the application classifies flowers into three species: **Setosa, Versicolor, and Virginica**. The project integrates a trained Scikit-learn model with an interactive **Streamlit** frontend, providing a seamless, real-time prediction experience.

## ✨ 2. Key Features


- **Real-time Prediction:** Instant classification results upon adjusting input parameters.
- **Interactive UI:** Uses sliders for precise numerical input of flower attributes.
- **Lightweight Architecture:** Minimalistic backend ensuring fast load times.
- **Responsive Design:** Optimized for various screen sizes via the Streamlit framework.
- **Model Persistence:** Utilizes serialized `.pkl` files for efficient model loading without retraining.

## 🛠️ 3. Technology Stack

| **Layer**               | **Technology**                     |
| ----------------------- | ---------------------------------- |
| **Frontend/Backend**    | Streamlit (Python-based framework) |
| **Machine Learning**    | Scikit-learn, NumPy, Pandas        |
| **Model Serialization** | Joblib / Pickle                    |
| **Environment**         | Python 3.8+                        |

## 🏗️ 4. System Architecture & Workflow

The application follows a standard **Model-View-Controller (MVC)** influenced workflow:

1. **User Input:** The user provides flower measurements (Sepal/Petal length and width) via Streamlit sliders.
2. **Data Processing:** Inputs are captured as a NumPy array and reshaped for model compatibility.
3. **Model Inference:** The pre-trained `.pkl` model performs a forward pass on the input data.
4. **Output:** The predicted class index is mapped to the species name and displayed on the UI.

## 📊 5. Dataset & Model Details

### The Iris Dataset

A classic dataset in ML containing 150 samples across four features:

- Sepal Length, Sepal Width, Petal Length, and Petal Width.

### Prediction Model

The system uses a **Supervised Learning algorithm** (e.g., Random Forest or Logistic Regression) trained to high accuracy. The model is saved as `iris_model.pkl` to decouple the training phase from the deployment phase.

## 📁 6. Project Structure

```
Iris-Classifier/
├── app.py                # Main Streamlit application logic
├── iris_model.pkl        # Serialized pre-trained ML model
├── requirements.txt      # List of Python dependencies
├── README.md             # Project documentation
└── assets/               # UI components (images/CSS)

```

## ⚙️ 7. Installation & Usage

### Prerequisites

- Python 3.8 or higher installed.

### Setup Instructions

1. **Clone the Repository:**

   ```
   git clone https://github.com/your-username/iris-classifier.git
   cd iris-classifier

   ```
2. **Install Dependencies:**

   ```
   pip install -r requirements.txt

   ```
3. **Run the App:**

   ```
   streamlit run app.py

   ```


## ✅ 8. Conclusion

This project serves as a comprehensive example of bridging the gap between a standalone machine learning script and a functional user-centric product. It highlights the importance of model deployment and provides a scalable foundation for more complex classification tasks.

---

### 📚 References

- [Scikit-learn Official Documentation](https://scikit-learn.org/)
- [Streamlit API Reference](https://docs.streamlit.io/)
- [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/iris)
