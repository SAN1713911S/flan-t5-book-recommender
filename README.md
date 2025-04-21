# 📚 Semantic Book Recommender using LLM (FLAN-T5)

This project is a **content-based book recommendation system** that uses **Google's FLAN-T5** language model to understand and compare books at a semantic level. Instead of relying on ratings or user behavior, it analyzes textual metadata—such as title, description, author, and categories—to recommend books that are meaningfully similar.

---

## 🚀 Features

- Uses a powerful **Large Language Model (LLM)** for generating semantic embeddings
- Generates **book recommendations** based on similarity of content
- Embedding generation using the **encoder of FLAN-T5**
- Book similarity measured via **cosine similarity**
- Can handle **partial or ambiguous book titles**
- Returns recommendations with **detailed metadata and similarity scores**

---

## 🧠 How It Works

1. Metadata for each book (title, author, description, etc.) is combined into a natural-language text.
2. Each book's text is passed through the FLAN-T5 encoder to generate a vector embedding.
3. Cosine similarity is computed between the query book and all others in the dataset.
4. Top similar books are returned as recommendations.

---

## 📦 Dataset

The project uses a Kaggle dataset containing metadata for over 7,000 books:  
**[7K Books with Metadata](https://www.kaggle.com/dylanjcastillo/7k-books-with-metadata)**

---

## 🛠️ Tech Stack

- Python
- PyTorch
- HuggingFace Transformers (`flan-t5-base`)
- Pandas & NumPy
- Scikit-learn
- tqdm
- kagglehub

---

## 📋 Example: Query = `"Treasure"`

The system found multiple matches for the title **"Treasure"**:

1) Treasure Box

2) Five on a Treasure Island

3) Mayflower Treasure Hunt

4) Dragon's Treasure

5) Encyclopedia Brown and the Case of the Treasure Hunt

6) Treasure Island

7) The Treasure Principle


Once the user selects the appropriate book, the system returns recommendations based on semantic similarity:

---

### 📚 Recommendations for: `Treasure`


================================================================================ ### 📚 Recommendations for: `Treasure`

---

**📚 Similarity:** `0.9893`  
**Title:** *The Left Hand Dreams of Him*  
**Authors:** Satoru Kannagi  
**Published Year:** 2006  
**Number of Pages:** 242  
**Category:** Comics & Graphic Novels  
**Description:** The growing romance between high school students Yuichi and Wataru is endangered by scholastic stress and well-meant deceptions....

---

**📚 Similarity:** `0.9573`  
**Title:** *The Mouse and His Child*  
**Authors:** Russell Hoban; David Small  
**Published Year:** 2001  
**Number of Pages:** 244  
**Category:** Juvenile Fiction  
**Description:** Two discarded toy mice survive perilous adventures in a hostile world before finding security and happiness with old friends and new....

---

**📚 Similarity:** `0.9566`  
**Title:** *Pippi Goes on Board*  
**Authors:** Astrid Lindgren; Louis S. Glanzman  
**Published Year:** 1977  
**Number of Pages:** 140  
**Category:** Juvenile Fiction  
**Description:** The further adventures of Pippi and her friends Tommy and Annika....

---

**📚 Similarity:** `0.9562`  
**Title:** *The Far Side of Evil*  
**Authors:** Sylvia Engdahl  
**Published Year:** 2005  
**Number of Pages:** 324  
**Category:** Juvenile Fiction  
**Description:** A young girl from an advanced civilization is sent as an observer to a planet whose people have not yet learned to control their use of atomic power....

---

**📚 Similarity:** `0.9494`  
**Title:** *The Pizza Monster*  
**Authors:** Marjorie Weinman Sharmat; Mitchell Sharmat  
**Published Year:** 2005  
**Number of Pages:** 80  
**Category:** Juvenile Fiction  
**Description:** Wealthy secret agent Olivia Sharp helps depressed Duncan find a friend....

---


## 📈 Future Improvements

- Add a simple web interface (Streamlit or Flask)
- Allow filtering by category, page length, or year
- Compare performance with other LLMs (e.g., BERT, GPT-3)
- Enable multilingual input and recommendation
- Add vector database (e.g., FAISS) for faster retrieval

## 🧑‍💻 Author

Developed with 💙 by Santiago Niño

## 📄 License

This project is licensed under the MIT License.  
Feel free to use, modify, and share it!
