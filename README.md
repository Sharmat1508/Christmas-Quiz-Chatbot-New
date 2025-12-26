# 🎄 Christmas Quiz Chatbot

A festive **Gradio** quiz app powered by **IBM watsonx.ai**.  
Pick a category, answer with A/B/C/D, and get Santa-style feedback after each question.

---

## ✨ Features
- Category-based Christmas trivia (easy to extend with more categories/questions)
- Gradio UI with a clean quiz flow (Next Challenge + answer box)
- Uses IBM watsonx.ai to generate fun, “Santa’s Verdict” explanations

- ## Demo Screenshots

![Quiz Question Screen](Screenshot%202025-12-26%20002030.png)

![Santa’s Verdict Screen](Screenshot%202025-12-26%20002038.png)


---

## 🧰 Tech Stack
- Python
- Gradio
- IBM watsonx.ai (Watsonx Runtime)
- crewai + litellm

---

## ✅ Prerequisites
- Python 3.10+ (recommended)
- An **IBM watsonx.ai project** with **watsonx.ai Runtime** associated
- Your IBM credentials:
  - `WATSONX_APIKEY`
  - `WATSONX_AI_PROJECT_ID`
  - `WATSONX_URL` (example: `https://us-south.ml.cloud.ibm.com`)

> If you see credential/project errors, open your project in watsonx → **Manage → Services & integrations** → Associate **watsonx.ai Runtime**.

---

## 🚀 Run Locally (Windows)

### 1) Create & activate a virtual environment
```bash
python -m venv .venv
.\.venv\Scripts\Activate.ps1

### 2) Install dependencies
pip install -r requirements.txt

###3) Add credentials (IMPORTANT)
This repo includes .env.example. Create your own .env file locally:
copy .env.example .env

Open .env and replace the placeholders with your real values:
WATSONX_APIKEY=PASTE_YOUR_API_KEY_HERE
WATSONX_AI_PROJECT_ID=PASTE_YOUR_PROJECT_ID_HERE
WATSONX_URL=https://us-south.ml.cloud.ibm.com

### 4) Start the app
python app.py

Open the link shown in the terminal (usually):
http://127.0.0.1:7860

Project Structure
app.py → main Gradio app
requirements.txt → dependencies
.env.example → template environment variables
.gitignore → prevents secrets / venv from being committed



