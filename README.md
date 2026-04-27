# SmartAlign-AI-Powered-Resume-Screener
SmartAlign is an end-to-end NLP application designed to bridge the gap between job seekers and Applicant Tracking Systems (ATS). Built with Streamlit and Scikit-learn, the tool automates the comparison of professional resumes against job descriptions using advanced text vectorization.

## 🚀 Features
- **PDF Text Extraction:** Automatically parses text from uploaded resume files.
- **NLP Preprocessing:** Cleans data by removing punctuation, converting to lowercase, and filtering out "stopwords" (common words like 'the', 'is', etc.).
- **Vectorization:** Uses **TF-IDF** to convert text into numerical vectors, emphasizing unique technical skills.
- **Similarity Scoring:** Calculates the **Cosine Similarity** between the resume and the job description.
- **Visual Analytics:** Displays a dynamic progress bar indicating "Low", "Good", or "Excellent" match quality.

## 🛠️ Tech Stack
- **Language:** Python 3.12+
- **Frontend:** Streamlit
- **NLP Library:** NLTK (Natural Language Toolkit)
- **Machine Learning:** Scikit-learn
- **PDF Parsing:** PyPDF2
- **Data Visualization:** Matplotlib

## 📦 Installation & Setup

pip install streamlit scikit-learn PyPDF2 matplotlib nltk

streamlit run app.py



📊 How It Works
SmartAlign follows a classic NLP pipeline:

Extraction: Extracts raw text from the uploaded PDF.

Cleaning: Uses Regular Expressions (re) to remove non-alphabetic characters.

Tokenization: Breaks text into individual words using nltk.

Scoring: Transforms the text into a TF-IDF matrix and measures the angle between the two vectors (Resume vs. JD).

🔮 Future Enhancements
Keyword Extraction: Identify specifically which skills (e.g., "Python", "AWS") are missing from the resume.

Semantic Search: Implementing BERT or LLM embeddings to understand synonyms (e.g., matching "ML" to "Machine Learning").

Cloud Deployment: Deploying the app via AWS or Streamlit Community Cloud.



   
