
# 🧠 Mental Wellness Chatbot

An AI-powered chatbot that provides educational support and advice related to mental wellness. It uses Natural Language Processing (NLP), semantic search, and curated mental health content to offer meaningful, non-judgmental interactions to users seeking initial support on topics such as anxiety, depression, self-care, and mindfulness.

---

## 📌 Project Overview

The Mental Wellness Chatbot is built to help individuals access reliable mental health information and guidance in a conversational way. It acts as a digital wellness assistant, retrieving relevant advice, resources, and educational content based on user queries using semantic similarity techniques.

It is **not** a replacement for therapy or professional help but serves as an easily accessible source of mental health knowledge and self-care strategies.

---

## 🎯 Objectives

- To develop a mental health support chatbot using NLP and semantic search.
- To categorize and retrieve responses on specific topics like anxiety, stress, mindfulness, and more.
- To use vector-based document retrieval for better semantic understanding of user queries.
- To make mental health knowledge more accessible and user-friendly through chatbot interaction.

---

## 🛠️ Tools & Technologies Used

- **Python 3.x**
- **Jupyter Notebook / VS Code**
- **Flask** – For chatbot UI (optional)
- **LangChain** – Framework for building context-aware applications
- **FAISS** – Fast similarity search over dense vectors
- **HuggingFace Embeddings** – Converts text to semantic vectors
- **NLTK, BeautifulSoup** – For NLP preprocessing and HTML parsing
- **Pandas, NumPy** – For data handling and cleaning
- **HTML/CSV** – Data source and storage format
- **IBM Cloud (Optional)** – For hosting and deployment

---

## 📚 Data Sources

The project uses web-scraped mental health articles from credible sources such as:
- [Healthline](https://www.healthline.com)
- [Medical News Today](https://www.medicalnewstoday.com)
- [NIH News in Health](https://newsinhealth.nih.gov)

All articles are categorized by topics like:
- Anxiety
- Depression
- Stress
- Sleep
- Self-care
- Mindfulness
- Gratitude
- Exercise
- And many more...

> 📝 A CSV file maps each topic to relevant article URLs for preprocessing and reference.

---

## 🧩 Project Structure

```
mental-wellness-chatbot/
│
├── HTML Files/                     # Raw HTML articles
├── mental_wellness_articles.csv   # Topic-to-URLs mapping
├── chatbot_logic.ipynb            # Main logic and NLP processing
├── chatbot_interface.py           # Flask-based web interface (optional)
├── templates/                     # HTML templates for UI
├── static/                        # CSS/JS assets
├── README.md                      # Project description and usage
└── requirements.txt               # Python dependencies
```

---

## ⚙️ How It Works

1. **HTML Parsing**: Web articles are parsed using BeautifulSoup to extract clean text.
2. **Preprocessing**: Tokenization, stopword removal, and optional lemmatization using NLTK.
3. **Document Splitting**: Articles are split into chunks for better context handling.
4. **Embeddings Generation**: Each chunk is converted into a semantic vector using HuggingFace models.
5. **FAISS Indexing**: Vectors are indexed using FAISS for high-performance semantic search.
6. **Query Handling**: User queries are embedded and matched to the most relevant chunks.
7. **Response Generation**: Matching content is retrieved and shown as chatbot responses.
8. **(Optional)**: Flask app to provide a browser-based interface for user interaction.

---

## 💬 Sample Use Case

**Query:** "How do I manage anxiety?"  
**Response:** A relevant chunk from trusted content is retrieved, e.g., breathing techniques, lifestyle changes, and cognitive strategies related to anxiety management.

---

## 🔗 Live Demo / GitHub Pages / Deployment (Optional)

*You can deploy the chatbot using IBM Cloud, Heroku, or locally with Flask.*  
🔗 **🟢 Try it live → https://mental-wellness-buddy.streamlit.app/**

---

## 🧪 Challenges Faced

- **Inconsistent HTML structures**  
  ✅ Solved using robust BeautifulSoup parsing logic.

- **Semantic accuracy issues**  
  ✅ Tuned chunk sizes, embedding models, and overlap parameters.

- **LangChain integration difficulties**  
  ✅ Resolved by referring to official docs and working examples.

---

## ✅ Future Improvements

- Add user sentiment detection for emotional tone classification  
- Enhance UI with chat history and feedback mechanism  
- Integrate voice input for accessibility  
- Expand the content base and multilingual support  

---

## 📎 References

- https://www.healthline.com  
- https://www.medicalnewstoday.com  
- https://newsinhealth.nih.gov  
- LangChain Docs: https://docs.langchain.com  
- FAISS: https://github.com/facebookresearch/faiss

---

## 👤 Author

**Makadia Nidat Chandreshbhai**  
CSE (AI & ML), VIT Bhopal  
*Feel free to connect for collaboration or improvements!*

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

