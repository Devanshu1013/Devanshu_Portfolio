# Hi, I'm Devanshu Prajapati 👋

Machine Learning | Data Science | AI Systems

M.Sc. in Data Science and Analytics @ Toronto Metropolitan University. I build machine learning systems and AI-driven applications across recommendation systems, time-series forecasting, NLP, and LLM-based tools.

📫 [LinkedIn](https://www.linkedin.com/in/devanshu1013/) &nbsp;|&nbsp; 💻 [GitHub](https://github.com/Devanshu1013)

---

## 🚀 Projects

| # | Project |
|---|---------|
| 1 | [Modeling Urban Crime Risk & Arrest Probability](#1-modeling-urban-crime-risk-and-arrest-probability-using-spatio-temporal-machine-learning-techniques) |
| 2 | [Movies Recommendation System](#2-movies-recommendation-system) |
| 3 | [DeepPaper Predictor](#3-deeppaper-predictor) |
| 4 | [WhatsApp Chat Analyzer](#4-whatsapp-chat-analyzer) |
| 5 | [Edit Intent Classification](#5-edit-intent-classification) |
| 6 | [Energy Forecasting](#6-energy-forecasting) |
| 7 | [Saransh — Text Summarizer](#7-saransh--text-summarizer) |
| 8 | [Audio to Text Converter](#8-audio-to-text-converter) |
| 9 | [Resume Parser & PDF Generator](#9-resume-parser--pdf-generator) |

---

### 1. [Modeling Urban Crime Risk and Arrest Probability Using Spatio-Temporal Machine Learning Techniques](https://github.com/Devanshu1013/MODELING-URBAN-CRIME-RISK-AND-ARREST-PROBABILITY-USING-SPATIO-TEMPORAL-MACHINE-LEARNING-TECHNIQUES)

A large-scale research project that builds a machine learning framework to predict arrests from over two decades of Chicago crime records (2001–2023), enriched with socio-economic, weather, and mobility data. Multiple classifiers and class-imbalance handling techniques were benchmarked, with a Random Forest model combined with oversampling delivering the strongest results — aimed at supporting data-driven public safety decisions.

**Highlights:**
- 20+ years of real-world crime data integrated with external socio-economic, weather, and mobility sources
- Benchmarks 14 machine learning models with multiple class-balancing strategies
- Full pipeline: literature review → preprocessing → EDA → feature engineering → experiments → results
- Written up as a formal research paper

**Tech stack:** `Python` `Scikit-learn` `Pandas` `Spatio-Temporal Feature Engineering`

<!-- Add a screenshot of your EDA charts or results here, e.g.: -->
<!-- ![Crime Risk Project](./assets/crime-risk-preview.png) -->

---

### 2. [Movies Recommendation System](https://github.com/Devanshu1013/Movies-Recommendation)

A DS8001 course project comparing multiple recommendation strategies — content-based, collaborative filtering, popularity-based, hybrid, and SVD — using real-world movie data from Kaggle, with a focus on evaluating each approach's strengths and trade-offs.

**Highlights:**
- Compares 5 different recommendation strategies on the same dataset
- Includes matrix factorization (SVD) alongside classic collaborative and content-based methods
- Evaluation-driven approach to compare recommendation quality across models

**Tech stack:** `Python` `Pandas` `Scikit-learn` `SVD` `Collaborative Filtering`

<!-- ![Movies Recommendation](./assets/movies-recommendation-preview.png) -->

---

### 3. [DeepPaper Predictor](https://github.com/Devanshu1013/DeepPaper-Predictor)

A web application that helps researchers discover relevant papers and predicts the subject area of a research paper directly from its abstract, using NLP techniques such as TF-IDF and similarity ranking.

**Highlights:**
- Predicts subject area of academic papers from abstract text
- Uses TF-IDF and similarity ranking to recommend related papers
- Packaged as an interactive web application

**Tech stack:** `Python` `NLP` `TF-IDF` `Scikit-learn` `Jupyter Notebook`

<!-- ![DeepPaper Predictor](./assets/deeppaper-preview.png) -->

---

### 4. [WhatsApp Chat Analyzer](https://github.com/Devanshu1013/WhatsApp-Chat-Analyzer)

A tool that extracts insights from exported WhatsApp chat data, giving a comprehensive overview of conversation patterns — including message frequency, media sharing trends, and sentiment analysis.

**Highlights:**
- Parses raw WhatsApp chat export files
- Visualizes message frequency, activity timelines, and media-sharing patterns
- Includes sentiment analysis on chat text

**Tech stack:** `Python` `Pandas` `Matplotlib/Seaborn` `NLP`

<!-- ![WhatsApp Chat Analyzer](./assets/whatsapp-analyzer-preview.png) -->

---

### 5. [Edit Intent Classification](https://github.com/Devanshu1013/Edit_Intent)

A transformer-based text classification system that identifies the *purpose* behind an edit made to a piece of text. Given a source sentence and its edited version, the model classifies the underlying intent behind the change.

**Highlights:**
- Transformer-based fine-tuning for intent classification
- Structured evaluation pipeline for comparing model performance
- Works on paired (original, edited) sentence data

**Tech stack:** `Python` `Transformers` `Deep Learning` `Jupyter Notebook`

<!-- ![Edit Intent Classification](./assets/edit-intent-preview.png) -->

---

### 6. [Energy Forecasting](https://github.com/Devanshu1013/Energy-Forecasting)

A comparative study of deep learning architectures for multivariate energy time-series forecasting. Uses 8 hours of historical sensor readings to predict the next energy consumption reading, benchmarking four different model families.

**Highlights:**
- Compares LSTM, TCN, Transformer, and LSTNet architectures on the same forecasting task
- Trained on the UCI Appliances Energy Prediction dataset (~19,700 rows, 10-minute intervals)
- Includes multi-horizon forecasting and sequence-length ablation experiments
- Chronological train/val/test split to avoid data leakage

**Tech stack:** `Python` `PyTorch` `LSTM` `TCN` `Transformer` `LSTNet`

<!-- ![Energy Forecasting](./assets/energy-forecasting-preview.png) -->

---

### 7. [Saransh — Text Summarizer](https://github.com/Devanshu1013/Saransh)

A text summarization and translation tool that accepts both plain text and PDF input. It uses NLTK-based summarization with lemmatization for improved accuracy, and can output the summary as an audio file — including in multiple languages.

**Highlights:**
- Extracts text directly from PDF documents
- NLTK + lemmatization based extractive summarization with adjustable summary length
- Converts summaries to speech (text-to-audio) using `pyttsx3`
- Translates summaries into multiple languages, with chunked translation for long text

**Tech stack:** `Python` `NLTK` `PyMuPDF` `pyttsx3` `Translation`

<!-- ![Saransh](./assets/saransh-preview.png) -->

---

### 8. [Audio to Text Converter](https://github.com/Devanshu1013/Audio_To_Text)

A simple utility that converts audio files into text transcripts using the `speech_recognition` library.

**Highlights:**
- Converts spoken audio into text transcripts
- Lightweight, notebook-based implementation

**Tech stack:** `Python` `SpeechRecognition` `Jupyter Notebook`

<!-- ![Audio to Text](./assets/audio-to-text-preview.png) -->

---

### 9. [Resume Parser & PDF Generator](https://github.com/Devanshu1013/Resume_Converter)

A tool that extracts text from an uploaded resume PDF, pulls out structured information (name, skills, experience, education, projects, hackathons, and achievements), and regenerates it as a clean, professionally formatted PDF resume — making it easier to review and compare resumes in one consistent format.

**Highlights:**
- Extracts structured fields from raw resume PDFs using `PyPDF2` and regex
- Generates a standardized, professional PDF resume with `ReportLab`
- Simple upload-and-generate interface built with Streamlit

**Tech stack:** `Python` `Streamlit` `PyPDF2` `ReportLab`

<!-- ![Resume Converter](./assets/resume-converter-preview.png) -->

---

## 🛠️ Technical Skills

**Languages:** Python, Java, C++
**Machine Learning:** Supervised & Unsupervised Learning, Classification, Regression, Feature Engineering, Model Evaluation, Cross-Validation
**Deep Learning:** TensorFlow, PyTorch, Keras, CNN, RNN, LSTM, Transformers
**NLP:** Text Preprocessing, TF-IDF, Word Embeddings, Text Classification
**Data Analysis & Visualization:** Pandas, NumPy, Matplotlib, Seaborn
**Databases & Tools:** MySQL, Git, Streamlit

---

## 📫 Contact

- LinkedIn: [linkedin.com/in/devanshu1013](https://www.linkedin.com/in/devanshu1013/)
- GitHub: [github.com/Devanshu1013](https://github.com/Devanshu1013)
