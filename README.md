# 🤖 IntelliView – AI-Powered Interview Coach

Welcome to **IntelliView**, a smart, AI-powered resume analyzer and interview preparation platform built using **Streamlit**, **Google Gemini API**, and **ngrok**. It helps job seekers evaluate their resumes, get real-time insights, and practice mock interviews powered by **Generative AI**.

---

## 📌 Table of Contents

- [🚀 Live on Google Colab](#-live-on-google-colab)
- [📄 Project Overview](#-project-overview)
- [🧠 Features](#-features)
- [🛠️ Tech Stack](#️-tech-stack)
- [⚙️ Setup Instructions](#️-setup-instructions)
- [🔐 API Keys & Tokens](#-api-keys--tokens)
  - [Gemini API Key (Google AI Studio)](#1-gemini-api-key-google-ai-studio)
  - [ngrok AuthToken](#2-ngrok-authtoken)
- [💡 Usage Flow](#-usage-flow)
- [🧪 Sample Run](#-sample-run)
- [🙌 Contributions](#-contributions)
- [📃 License](#-license)

---

## 🚀 Live on Google Colab

Launch and explore the notebook directly from Google Colab:

👉 [**Open in Google Colab**](https://colab.research.google.com/github/HimeshBhattacharjee/IntelliView/blob/main/IntelliView_AI_Powered_Interview_Coach.ipynb)

---

## 📄 Project Overview

**IntelliView** is designed for students, professionals, and job seekers to:

- Upload their **PDF resume**
- Analyze it for **ATS compatibility**
- Get **strengths**, **weaknesses**, and **tailored recommendations**
- Simulate **AI-powered mock interviews**
- View a **detailed report dashboard**

It leverages **Google’s Gemini 1.5 Flash Model** for deep NLP analysis and integrates interactive elements via **Streamlit**.

---

## 🧠 Features

- 📥 Resume Upload and Live PDF Preview  
- ⚙️ ATS Score Calculation  
- ✅ Strengths & ⚠️ Weakness Analysis  
- 📝 AI-Generated Recommendations  
- 🎤 Interview Simulation & Practice  
- 📊 Interactive Feedback Reports  
- 🔒 Environment Secure via `.env` file  

---

## 🛠️ Tech Stack

| Technology     | Purpose                          |
|----------------|----------------------------------|
| Python         | Core logic                       |
| Streamlit      | UI/UX frontend                   |
| Google Gemini  | Resume analysis & QA generation  |
| PyMuPDF (fitz) | PDF parsing                      |
| Plotly         | Graphical feedback               |
| ngrok          | Expose localhost to public URL   |
| dotenv         | Securely manage API keys         |

---

## ⚙️ Setup Instructions

Clone the repository:

```bash
git clone https://github.com/HimeshBhattacharjee/IntelliView.git
cd IntelliView
````

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch the app using Streamlit (after setting up `.env`):

```bash
streamlit run app.py
```

> To use it from Google Colab, open the notebook and follow the provided cells step-by-step.

---

## 🔐 API Keys & Tokens

You need two secure credentials:

### 1. Gemini API Key (Google AI Studio)

> Required for resume analysis and question generation.

#### 📝 Steps:

1. Go to [Google AI Studio](https://aistudio.google.com/app/apikey)
2. Click **"Create API Key"**
3. Copy the key
4. In your `.env` file (create one if not present):

```env
GEMINI_API_KEY=your_generated_key_here
```

📌 You must have a Google account. Basic usage is free with usage limits.

---

### 2. ngrok AuthToken

> Required to expose your Streamlit app running locally to the internet from Colab.

#### 📝 Steps:

1. Visit [https://dashboard.ngrok.com/get-started/setup](https://dashboard.ngrok.com/get-started/setup)
2. Sign up and login
3. Copy your **AuthToken**
4. In your `.env` file:

```env
NGROK_AUTH_TOKEN=your_ngrok_token_here
```

💡 You can also run this in Colab to authenticate:

```python
!ngrok config add-authtoken YOUR_NGROK_TOKEN
```

---

## 💡 Usage Flow

1. 🔑 Add API keys in `.env`
2. 🔃 Run the app (`streamlit run app.py`) or follow the Colab notebook
3. 📄 Upload a resume (PDF)
4. 🧠 Analyze resume → ATS Score, Strengths/Weaknesses
5. 🎤 Mock interview starts based on your resume + job role
6. 📊 Dashboard report displayed

---

## 🙌 Contributions

Contributions are welcome! Please open an issue or submit a pull request.

---

> Created with ❤️ by **[Himesh Bhattacharjee](https://github.com/HimeshBhattacharjee)**
