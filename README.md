# Movie Recommendation System

A hybrid movie recommendation system that combines content-based filtering and collaborative filtering to provide personalized movie recommendations. Built using Python, this system processes the MovieLens 25M Dataset to suggest movies based on both title similarity and user rating patterns.

## 🎯 Features

- **Title-based Search**: Find movies using fuzzy text matching
- **Collaborative Filtering**: Get recommendations based on similar users' preferences
- **Interactive Interface**: Real-time recommendations using Jupyter widgets
- **Hybrid Approach**: Combines content-based and collaborative filtering techniques
- **Scoring System**: Sophisticated scoring that balances similarity and popularity

## 🛠️ Technologies Used

- Python 3.11
- pandas
- scikit-learn
- NumPy
- Jupyter Notebooks
- ipywidgets

## 📦 Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/movie-recommendation-system.git
cd movie-recommendation-system
```

2. Create a virtual environment (optional but recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows, use: venv\Scripts\activate
```

3. Install required packages:
```bash
pip install pandas scikit-learn numpy jupyter ipywidgets
```

4. Download the MovieLens 25M Dataset from [GroupLens](https://grouplens.org/datasets/movielens/25m/) and extract it to the project directory.

## 🚀 Usage

1. Start Jupyter Notebook:
```bash
jupyter notebook
```

2. Open `Movie_recs.ipynb`

3. Run all cells to initialize the recommendation system

4. Use the interactive widgets to:
   - Search for movies by title
   - Get personalized recommendations
   - Explore similar movies

## 💡 How It Works

### Content-Based Filtering
- Uses TF-IDF vectorization for movie title similarity
- Implements cosine similarity for comparing movie titles
- Handles special characters and standardizes movie titles

### Collaborative Filtering
- Identifies users with similar movie preferences
- Analyzes rating patterns across user groups
- Calculates recommendation scores based on user behavior

### Scoring System
- Combines similarity scores with user rating patterns
- Normalizes recommendations against general popularity
- Provides weighted scores for final recommendations

## 📊 Data Processing

The system processes two main datasets:
1. **movies.csv**: Contains movie information (ID, title, genres)
2. **ratings.csv**: Contains user ratings (userID, movieID, rating, timestamp)

Data preparation steps:
1. Clean movie titles
2. Vectorize text data
3. Process user ratings
4. Calculate similarity metrics
5. Generate recommendation scores

## 🎯 Example

```python
# Search for movies
search("The Matrix")

# Get recommendations
find_similar_movies(movie_id=89745)
```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


## 🙏 Acknowledgments

- [MovieLens](https://grouplens.org/datasets/movielens/) for providing the dataset
- [scikit-learn](https://scikit-learn.org/) for machine learning tools
- [pandas](https://pandas.pydata.org/) for data manipulation capabilities

## 📫 Contact
Mani Pourfazli - manipourfazli1384@gmail.com
