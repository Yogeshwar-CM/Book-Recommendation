# Book Recommendation System

This project implements a book recommendation system using collaborative filtering, content-based filtering, and a hybrid approach.

## Project Overview

1. **Data Preparation:**

   - Utilizes datasets including books, users, and ratings.
   - Handles missing values and duplicates.
   - Filters data to focus on users with extensive ratings and popular books.

2. **Collaborative Filtering:**

   - Recommends books based on similar users' ratings.
   - Uses cosine similarity to identify similar users and suggest books they liked.

3. **Content-Based Filtering:**

   - Recommends books similar to a given book based on features like title, author, and publisher.
   - Employs TF-IDF and Nearest Neighbors for feature extraction and similarity search.

4. **Hybrid Recommendation System:**
   - Combines collaborative and content-based recommendations to provide a comprehensive list of suggestions.

## Functions

- **recommend_books_collaborative(user_id, num_recommendations=5):**

  - Provides book recommendations based on collaborative filtering for a given user.

- **recommend_books_content_based(book_title, num_recommendations=5):**

  - Suggests books similar to a given book title using content-based filtering.

- **hybrid_recommendation(user_id, book_title, num_recommendations=5):**
  - Merges collaborative and content-based recommendations for a more robust suggestion list.

## Example Usage

```python
user_id_example = 277427
book_title_example = "Classical Mythology"

print("Collaborative Filtering Recommendations:")
print(recommend_books_collaborative(user_id_example))

print("\nContent-Based Recommendations:")
print(recommend_books_content_based(book_title_example))

print("\nHybrid Recommendations:")
print(hybrid_recommendation(user_id_example, book_title_example))
```

Feel free to use and modify this project.
