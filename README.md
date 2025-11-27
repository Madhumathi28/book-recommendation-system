# 📚 Book Recommendation Engine using KNN

This project is part of the FreeCodeCamp Machine Learning Certification.

It uses the **Book-Crossings dataset** and builds a **KNN-based book recommendation model** using `NearestNeighbors` from `sklearn`.

## Features
- Removes users with fewer than 200 ratings
- Removes books with fewer than 100 ratings
- Creates a pivot matrix: books × users
- Fits a KNN model using cosine similarity
- Implements `get_recommends(title)` that returns 5 most similar books

## How to Run
Open the notebook in Google Colab:

1. Upload `book_recommender.ipynb`
2. Run all cells
3. The final cell tests your implementation

## Example Output

```python
get_recommends("The Queen of the Damned (Vampire Chronicles (Paperback))")
```

Should return:

```
[
  "The Queen of the Damned (Vampire Chronicles (Paperback))",
  [
    ["Catch 22", 0.793983519077301],
    ["The Witching Hour (Lives of the Mayfair Witches)", 0.7448656558990479],
    ["Interview with the Vampire", 0.7345068454742432],
    ["The Tale of the Body Thief (Vampire Chronicles (Paperback))", 0.5376338362693787],
    ["The Vampire Lestat (Vampire Chronicles, Book II)", 0.5178412199020386]
  ]
]
```

This notebook passes the official FCC test.
