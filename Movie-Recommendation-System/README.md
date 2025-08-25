
# Movie Recommendation System 

A content-based movie recommendation system that suggests similar movies based on the metadata of movies like genres, cast, crew, and keywords. The system utilizes technique like vectorization to recommend movies from a dataset of 5000+ movies.

## Features
- Recommend 5 similar movies based on the selected movie.
- Utilizes **Bag of Words** and **Cosine Similarity** for calculating the similarity between movies.
- Built with an interactive web app using **Streamlit** for easy user interaction.

## Project Structure
- **`app.py`**: Streamlit web app that takes movie input and shows recommendations.
- **`movie_dict.pkl`**: Pickle file containing preprocessed movie data (for faster loading).
- **`similarity.pkl`**: Pickle file storing precomputed similarity matrix between movies.
- **`Procfile`** and **`setup.sh`**: Configuration files for the app's environment setup.
- **`requirements.txt`**: List of dependencies required to run the project.

## Dataset
The dataset contains information about 5000+ movies, including:
- **Genres**
- **Cast**
- **Crew (Director)**
- **Keywords**
- **Overview (Description)**

## How It Works
1. **Data Preprocessing**:
    - Remove unnecessary columns and handle missing data.
    - Extract and clean the metadata such as genres, keywords, cast, and crew.
    - Combine relevant features into a `tags` column for better analysis.
    
2. **Vectorization**:
    - Convert the `tags` into numerical vectors using **Bag of Words**.
    - Apply **stemming** using **PorterStemmer** to reduce words to their base forms (e.g., 'loved' becomes 'love').
    
3. **Similarity Calculation**:
    - Use **Cosine Similarity** to compute the distance between the movie vectors.
    - Recommend 5 movies with the highest similarity to the selected movie.

## Web Application
The web app allows users to:
- Select a movie from a dropdown list.
- Get 5 similar movie recommendations based on content similarity.

## Installation and Usage

1. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```


## Dependencies
- **Pandas**
- **Streamlit**
- **Scikit-learn**
- **NLTK**
- **Pickle**

Install all dependencies by running:
```bash
pip install -r requirements.txt
```

## How to Contribute
Feel free to contribute by:
- Forking the repository.
- Creating a new branch.
- Making the changes.
- Submitting a pull request.
