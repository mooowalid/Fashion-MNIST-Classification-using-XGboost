wesome work, Mohamed! 🎉 Your project covers everything from preprocessing to deployment — well done.

Here’s a clean, professional README.md you can use for your GitHub repository:

markdown
Copy
Edit
# 👕 Fashion-MNIST Classification with Random Forest, XGBoost & Gradio

This project is a complete machine learning pipeline built for classifying images from the **Fashion-MNIST** dataset. It includes data preprocessing, exploratory data analysis (EDA), model training (Random Forest & XGBoost), model comparison, and an interactive web app deployed using **Gradio**.

## 📁 Dataset

The [Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist) dataset is a drop-in replacement for the original MNIST dataset, consisting of 70,000 grayscale images of 10 fashion categories (28x28 pixels).

- **Training set:** 60,000 images  
- **Test set:** 10,000 images  
- Each image is labeled as one of 10 classes (e.g., T-shirt, Trouser, Sneaker, etc.)

## ⚙️ Project Pipeline

### ✅ Preprocessing
- Removed duplicate samples
- Checked for missing values
- Normalized pixel values to [0, 1] range
- Separated features and labels

### 📊 EDA
- Visualized label distributions
- Displayed sample images by class

### 🧠 Models Used
- **Random Forest Classifier** with Grid Search for hyperparameter tuning
- **XGBoost Classifier** with sample weight balancing for better generalization

### 📈 Evaluation Metrics
- Accuracy score
- Classification report
- Confusion matrix
- Train vs Test accuracy comparison

### 🔬 Model Comparison
- Compared performance of both models visually and numerically
- XGBoost showed slightly better generalization performance

### 💾 Model Saving
- Best XGBoost model saved as `xgboost_model.pkl` using `joblib`

## 🌐 Deployment

The best model was deployed using **Gradio**, allowing users to upload images and get real-time predictions.

### ▶️ Try the App (Locally)

```bash
pip install gradio joblib xgboost scikit-learn pandas numpy pillow
streamlit run app.py

