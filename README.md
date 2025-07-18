# Zee_Recommender_Systems
  - This project builds a personalized movie recommender system using the MovieLens dataset to enhance user experience by suggesting movies based on user ratings and preferences.
  
  - The system implements multiple approaches:

    - Collaborative Filtering (User-based & Item-based)
    
    - Pearson Correlation
    
    - Cosine Similarity (with KNN)
    
    - Matrix Factorization (Surprise Library / CMFRec)

## 📂 Dataset

  - **ratings.dat:** UserID, MovieID, Rating, Timestamp
  
  - **users.dat:** User demographics (Gender, Age, Occupation, Zip-code)
  
  - **movies.dat:** Movie Title & Genres

## 🚀 Features
  **1. Data Preprocessing**
  - Merged ratings, movies, and users into a single dataframe
  - Extracted Release Year from titles and handled missing values
  - Aggregated average ratings and number of ratings per movie

  **2. Exploratory Data Analysis (EDA)**
  - Visualized rating distribution by genre, age, and popularity
  - Analyzed average ratings vs. number of ratings

  **3. Recommendation Engines**
  - Item-based (Pearson Correlation): Recommend 5 similar movies
  - Cosine Similarity (KNN): Generate user-item similarity matrices
  - Matrix Factorization (d=4): RMSE & MAPE evaluated; embeddings visualized

  **4. User-based Collaborative Filtering**
  - Find top 10 most similar users
  - Recommend top 10 movies based on weighted ratings

## 🛠 Tech Stack
  - Python, Pandas, NumPy, Matplotlib, Seaborn
  
  - Scikit-learn (Cosine Similarity & KNN)
  
  - Surprise / CMFRec (Matrix Factorization)

## 📈 Evaluation
  - Root Mean Squared Error (RMSE)
  
  - Mean Absolute Percentage Error (MAPE)
  
  - Visualization of embeddings (d=2 & d=4)
## 📌 Future Work
  - Deploy as a Flask/Streamlit Web App
  
  - Incorporate content-based filtering (genres & metadata)
  
  - Implement hybrid recommendation models
