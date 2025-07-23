# 🛍️ E-commerce Product Recommendation System

A machine learning-based recommendation system for e-commerce platforms that provides personalized product suggestions using collaborative filtering techniques. This system enhances user experience by recommending relevant products based on user preferences and historical data.

---

## 🚀 Features

- 🔍 **User-Based Collaborative Filtering**  
  Recommends products by finding similar users and suggesting what they liked.

- 🎯 **Item-Based Collaborative Filtering**  
  Suggests products similar to items a user has previously interacted with.

- 📈 **Evaluation Metrics**  
  Includes RMSE and MAE for measuring prediction accuracy.

- 🧹 **Clean Data Pipeline**  
  Preprocessing steps to clean and format the dataset for effective training.

---

## 📁 Project Structure

Ecommerce-Recommender/
│
├── data/ # Contains dataset CSV
├── notebooks/ # Jupyter notebooks for EDA and experiments
├── recommender/ # Python modules for training and inference
│ ├── train.py # Builds and trains the model
│ └── infer.py # Generates recommendations
│
├── utils/ # Utility functions
├── requirements.txt # Python dependencies
└── README.md # Project documentation

---

## 📊 Dataset

- Source: [Kaggle E-commerce Dataset](https://www.kaggle.com)
- Contains:
  - `user_id`
  - `product_id`
  - `rating`
  - `timestamp`

> *Note: You can replace the dataset with your custom user-product interactions as well.*

---

## ⚙️ How it Works

1. **Data Preprocessing**  
   Load and filter users/items with sufficient interactions.

2. **Model Training**  
   Matrix Factorization using `Surprise` library's SVD (Singular Value Decomposition).

3. **Recommendation Generation**  
   Predict top-N items for a given user using learned latent factors.


