# 💼 AI Interview Coach

An interactive web application built with **Streamlit** and the **Google GenAI SDK (Gemini)** that helps students and job seekers practice technical interview questions and receive structured, actionable AI feedback.

---

## ✨ Features

- 🎯 **Topic-Specific Questions**: Practice questions across popular topics including Python, SQL, HTML, JavaScript, and Data Structures.
- 🤖 **Powered by Gemini**: Uses Google's latest Gemini Flash models (`gemini-3.1-flash-lite`, `gemini-3.5-flash`, `gemini-3.8-flash`) with automatic fallback for high availability.
- 📝 **Structured Interview Feedback**: Evaluates answers with:
  1. **What Was Good**: Identifies accurate and well-explained concepts.
  2. **Areas for Improvement**: Highlights gaps, misconceptions, or areas to expand.
  3. **Sample Ideal Answer**: Provides an exemplary answer tailored for an interview setting.
- 🔒 **Secure Configuration**: Keeps API keys safe using Streamlit Secrets.

---

## 🚀 Getting Started

### Prerequisites

- Python 3.10+
- A Google Gemini API key from [Google AI Studio](https://aistudio.google.com/)

### 1. Clone the Repository

```bash
git clone https://github.com/saikumar7845/AI-interview-practice-app.git
cd AI-interview-practice-app
```

### 2. Set Up a Virtual Environment

```bash
# Windows
python -m venv venv
.\venv\Scripts\activate

# macOS / Linux
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure Your API Key

Create a `.streamlit/secrets.toml` file in the project root:

```toml
GEMINI_API_KEY = "your-gemini-api-key-here"
```

*(Note: `.streamlit/secrets.toml` is ignored by `.gitignore` to keep your credentials safe.)*

### 5. Run the Application

```bash
streamlit run app.py
```

The app will open automatically in your browser at `http://localhost:8501`.

---

## 🌐 Deploy to Streamlit Community Cloud

1. Fork or push this repository to your GitHub account.
2. Sign in to [Streamlit Community Cloud](https://share.streamlit.io/).
3. Click **New app** and select:
   - **Repository:** `saikumar7845/AI-interview-practice-app`
   - **Branch:** `main`
   - **Main file path:** `app.py`
4. Click **Advanced settings...** > **Secrets** and add:
   ```toml
   GEMINI_API_KEY = "your-gemini-api-key-here"
   ```
5. Click **Deploy!**

---

## 🛠️ Built With

- [Streamlit](https://streamlit.io/) — Interactive web UI
- [Google GenAI Python SDK](https://github.com/googleapis/python-genai) — Official Gemini API client
- Python 3
