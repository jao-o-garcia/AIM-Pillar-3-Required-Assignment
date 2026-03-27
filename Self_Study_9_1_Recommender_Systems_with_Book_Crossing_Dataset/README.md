# Self-Study Assignment 9.1: Recommender Systems with the Book-Crossing Dataset

---

## 🎯 Learning Outcomes

- Apply advanced machine learning techniques in specialised areas such as:
  - Natural Language Processing (NLP)
  - Recommender systems
  - Time-series analysis  
- Integrate multiple advanced ML techniques into comprehensive solutions  
- Design and implement recommender systems using:
  - Information retrieval
  - Collaborative filtering  

---

## 📖 Scenario

An online bookstore wants to implement a recommendation engine to suggest relevant books to users based on their reading preferences.

You are tasked to:
- Explore user-item interaction data  
- Build:
  - User-based collaborative filtering model  
  - Item-based collaborative filtering model  
- Create a prototype that generates **Top-5 book recommendations** for selected users  

---

## 📂 Dataset

- `Users.csv` → User demographic data  
- `Books.csv` → Book metadata  
- `Ratings.csv` → User ratings for books  

**Tool:** Python 🐍

---

## 🧪 Tasks

---

### 🔹 Task 1: Data Preparation and EDA

#### Steps:
- Load and merge:
  - Books
  - Users
  - Ratings  
- Use appropriate keys for merging  

#### Data Cleaning:
- Drop missing values  
- Remove duplicate ratings  
- Filter out:
  - Users with fewer than 5 ratings  
  - Books with very few interactions  

#### Exploration:
- Analyze rating distribution  
- Identify:
  - Active users  
  - Popular books  

---

### 🔹 Task 2: User-Based Collaborative Filtering

#### Steps:
- Create a **user-item matrix**
  - Rows → Users  
  - Columns → Books  
  - Values → Ratings  

- Handle missing values:
  - Fill with zeros (or alternative strategy)

- Compute:
  - Cosine similarity between users  

#### Recommendation:
- Select a user ID  
- Identify **Top 5 most similar users**  
- Recommend:
  - Top 5 books the user hasn’t read  
  - Books highly rated by similar users  

---

### 🔹 Task 3: Item-Based Collaborative Filtering

#### Steps:
- Transpose the matrix → **item-user matrix**

- Compute:
  - Cosine similarity between items (books)

#### Recommendation:
- Select a book ID  
- Retrieve:
  - Top 5 similar books (based on rating patterns)  

- Recommend these books to:
  - Users who liked the original book  

---

### 🔹 Task 4: Evaluation and Insights

Provide insights on:

- 📊 Which filtering method performs better for **sparse data**?
- ⚙️ How to improve **scalability** of the model?
- 💡 How this system enhances **user experience**?

---

## Solution
You can continue to use the file - M 9 Non-graded Assignment 1.ipynb Download M 9 Non-graded Assignment 1.ipynb, which serves as a reference to help you validate your understanding. You can compare your code, implementation steps, and output against this solution to identify areas for improvement. However, we strongly recommend attempting the practice exercises first before reviewing the solution. 