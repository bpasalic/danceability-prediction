# Danceability Prediction using Machine Learning
This project was developed as a part of a Machine Learning for Engineers course at Universidad Pontificia Comillas, Madrid.
It predicts the danceability of Spotify tracks using machine learning techniques. We used a dataset from Kaggle and tested four regression models to find the most accurate approach for estimating a song’s danceability score.

## Dataset

We used the publicly available dataset from Kaggle:  
https://www.kaggle.com/datasets/zaheenhamidani/ultimate-spotify-tracks-db

It contains over 232,000 entries of Spotify songs with various audio features such as energy, valence, tempo, loudness, and more.

## Models Used

- Linear Regression  
- Decision Tree  
- Random Forest  
- XGBoost (Best performing)

XGBoost achieved the best results with the lowest MSE and highest R² score, making it the final model used for prediction.

## Features

Key audio features used for prediction include:

- Valence: Positivity of the track (0.0 to 1.0)  
- Energy: Intensity and activity (0.0 to 1.0)  
- Tempo: Beats per minute  
- Loudness, Speechiness, Instrumentalness, etc.

## Project Highlights

- Data cleaning and preprocessing (duplicates removed, irrelevant columns dropped)  
- One-hot, binary, and ordinal encoding  
- Rescaling using MinMax and Robust Scalers  
- Feature importance analysis  
- Regression-to-classification interpretability (Low, Medium, High danceability)  
- Model comparison and performance evaluation (MSE, RMSE, R², Adjusted R²)

## How to Download the Dataset

To fetch the dataset used in this project:

1. Go to the Kaggle dataset: https://www.kaggle.com/datasets/zaheenhamidani/ultimate-spotify-tracks-db
2. Sign in with your Kaggle account (create one if needed)
3. Click “Download” on the top right
4. Extract the ZIP file and place `SpotifyFeatures.csv` into your working directory
5. Rename it if needed to match any expected filename (e.g., `dataset.csv`)

## Running the Code

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/danceability-prediction.git
   cd danceability-prediction
   ```

2. Create and activate a virtual environment (optional but recommended):
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the Jupyter notebook or Python scripts as provided.

## Results Summary

| Model              | MSE     | RMSE    | R² Score | Adjusted R² |
|-------------------|---------|---------|----------|-------------|
| Linear Regression | 0.0142  | 0.1190  | 0.609    | 0.608       |
| Decision Tree     | 0.0134  | 0.1160  | 0.628    | 0.628       |
| Random Forest     | 0.0097  | 0.0985  | 0.732    | 0.731       |
| XGBoost           | 0.0087  | 0.0932  | 0.760    | 0.760       |

## Authors

- Barbara Pašalić  
- Mihovil Njegovan  
- Rikardo Radešić  
- Neven Spaček  
- Karlo Vrdoljak  
- Blanka Wójcik
