# Content-Based-Movie-Recommender
Developed a content-based recommendation engine using Python and NLP techniques to suggest similar movies based on plot, genre, cast, and keywords. Utilized cosine similarity on text-processed features and integrated TMDB API to dynamically fetch movie posters. Built an interactive user interface using Streamlit to allow real-time movie selection and recommendation display.

Features
✅ Recommends 5 similar movies based on the selected title

✅ Uses cosine similarity over NLP-based feature vectors

✅ Interactive UI with real-time results via Streamlit

✅ Fetches posters dynamically from the TMDB API

🧠 How It Works
Data Source:

Used tmdb_5000_movies.csv and tmdb_5000_credits.csv.

Feature Engineering:

Combined features: genres, overview, keywords, cast, and crew.

Applied NLP (tokenization, stemming, etc.)

Created a tags column used to vectorize movie content.

Model Building:

Used CountVectorizer to convert text to numeric vectors.

Calculated cosine similarity to measure movie similarity.

Saved movie_list.pkl and similarity.pkl for fast runtime performance.

App UI:

Built using Streamlit.

Allows users to select a movie and view 5 similar recommendations with posters fetched via TMDB API.

🛠️ Installation & Setup
Clone the repo

bash
Copy
Edit
git clone https://github.com/yourusername/movie-recommender.git
cd movie-recommender
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
Run the Streamlit app

bash
Copy
Edit
streamlit run app.py

