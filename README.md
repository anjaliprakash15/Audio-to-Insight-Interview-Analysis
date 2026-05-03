# 🎯 Audio-to-Insight Interview Analysis

End-to-end NLP pipeline to convert interview audio into transcripts, extract key themes using BERTopic, and visualize insights through interactive dashboards.

---

## 📌 Overview

This project builds an end-to-end pipeline to analyze interview audio and extract meaningful insights using **Automatic Speech Recognition (ASR)** and **Natural Language Processing (NLP)**.

It transforms raw interview recordings into structured and interpretable data that can be used for analysis and decision-making.

---

## 🚀 What This Project Does

The pipeline processes raw audio interviews and converts them into:

- 📄 Clean transcripts  
- 🧠 Extracted topics and themes  
- 📊 Structured datasets  
- 📈 Interactive visual dashboards  

---

## 🔄 Pipeline Workflow

### 1. Audio Processing
- Converts `.m4a` files to `.wav` format
- Standardizes audio to 16kHz mono

### 2. Speech-to-Text (ASR)
- Uses **NVIDIA NeMo (Parakeet model)** for transcription
- Generates:
  - `.txt` transcripts  
  - `.srt` subtitle files  
  - `.csv` timestamped segments  

### 3. Speaker Segmentation
- Identifies and separates speakers
- Focuses on **participant responses** for analysis

### 4. Text Preprocessing
- Removes filler words (um, like, etc.)
- Normalizes and cleans text
- Improves data quality for modeling

### 5. Document Creation
- Converts transcripts into smaller chunks
- Uses sliding window technique for better context

### 6. Topic Modeling
- Applies **BERTopic**
- Uses:
  - Sentence Transformers (MiniLM)
  - UMAP (dimensionality reduction)
  - HDBSCAN (clustering)

### 7. Visualization
- Interactive dashboards using **Plotly**
- Displays:
  - Topic distribution
  - Topic importance scores
  - Document-topic relationships

---

## 📊 Key Insights Extracted

The model identifies themes such as:

- 🎓 Education & GED pathways  
- 💼 Career goals & job readiness  
- 🧠 Mental health & personal challenges  
- 🎨 Creative interests  
- 🚗 Transportation barriers  
- 📱 Technology access issues  

---

## 📂 Project Structure
├── data/ # Input audio files

├── work/ # Intermediate processed files

├── outputs/ # Final transcripts & results

├── dashboard/ # Interactive HTML dashboards

├── notebooks/ # Colab notebooks / scripts

├── README.md


---

## ⚙️ Tech Stack

- Python  
- NVIDIA NeMo (ASR)  
- BERTopic  
- Sentence Transformers  
- UMAP + HDBSCAN  
- Plotly (Visualization)  
- Google Colab  

---

## 📈 Results

- Processed interview audio into structured transcripts  
- Generated document chunks for analysis  
- Extracted meaningful topics across interviews  
- Built interactive dashboards for easy exploration  

---

## 🎯 Impact

This project helps:

- Automate analysis of interview data  
- Identify patterns across participants  
- Extract insights from unstructured audio  
- Support data-driven decision-making  

---

## ⚠️ Limitations

- Small dataset size  
- Some topic overlap  
- Dependent on transcription quality  

---

## 🔮 Future Improvements

- Improve speaker diarization  
- Add sentiment analysis  
- Build real-time dashboard  
- Integrate recommendation system  

---

## 👩‍💻 Author

**Anjali Prakash**  
Master’s in Computer & Information Sciences  
University of North Florida  

---
