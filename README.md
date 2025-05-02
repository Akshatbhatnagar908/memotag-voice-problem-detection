# 🗣️ Voice Problem Detection using NLP and Machine Learning

This project is a prototype system for identifying potential voice and speech disorders using speech recognition, natural language processing (NLP), and machine learning. It focuses on detecting fluency issues in spoken language such as long pauses, hesitation words, and irregular speech timing. These features can help in early identification of cognitive or motor speech impairments.

## 🔍 Project Overview

The system captures live speech input, transcribes it using Google's Speech Recognition API, and then analyzes the text for signs of disfluency. It combines rule-based detection (for pauses and hesitations) with machine learning-based clustering and vectorization to analyze and flag potentially abnormal patterns.

## 🚀 Features

- 🎙️ **Real-Time Audio Input**: Uses a microphone to capture spoken input.
- 📝 **Speech-to-Text**: Transcribes audio using Google’s `recognize_google` API.
- ⏸️ **Pause Detection**: Detects unnatural pauses based on punctuation and timing.
- 🤔 **Hesitation Word Detection**: Identifies filler words like "uh", "um", "erm".
- 🧠 **Text Representation**:
  - **Bag of Words (BoW)** using `CountVectorizer`
  - **TF-IDF** using `TfidfVectorizer`
- 🔀 **Clustering**: Uses KMeans to group pause timings and analyze fluency patterns.
- 📊 **Visualization**: Optionally plots clusters to show delay pattern distribution.

## 🧰 Tech Stack

- Python 3
- Jupyter Notebook
- `speechrecognition`
- `sklearn` (for vectorization and clustering)
- `numpy`, `re`, `matplotlib`

## 📦 Installation

1. Clone the repository:
```bash
git clone https://github.com/akshatbhatnagar908/voice-problem-detection.git
cd voice-problem-detection
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Launch the notebook:
```bash
jupyter notebook memotag_voice_problem_detection.ipynb
```

## 📓 Example Workflow

1. User speaks into the microphone.
2. Audio is transcribed to text.
3. System detects pauses and hesitation words.
4. Time delays (simulated or real) are clustered using KMeans.
5. Transcription and fluency features are vectorized using BoW and TF-IDF.
6. Output includes visual and printed feedback indicating potential fluency issues.

## 🔬 Future Improvements

- Add support for **supervised ML models** using labeled clinical data.
- Extract **acoustic features** (e.g., jitter, shimmer, MFCCs).
- Integrate **deep learning models** (LSTM, CNN, BERT) for more accuracy.
- Build a **web interface** or mobile app for easier testing and use in clinics.
- Collaborate with **clinicians and speech-language pathologists** for validation.
linkedin-https://www.linkedin.com/in/akshatbhatnagar908/


