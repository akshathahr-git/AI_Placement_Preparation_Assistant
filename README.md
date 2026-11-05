# 🚀 AI Placement Preparation Assistant

An AI-powered web application designed to help students and job seekers prepare for technical interviews. Built using **LangChain**, **Streamlit**, and **OpenRouter**, this tool generates customized interview questions, detailed model answers, and practical examples based on the user's target job role, experience level, and difficulty preference.

## ✨ Features

- **Role-Based Generation:** Select from roles like Python Developer, AI Engineer, Data Scientist, and more.
- **Experience & Difficulty Control:** Tailor questions based on your experience level (Fresher to 5+ Years) and preferred difficulty (Easy, Medium, Hard).
- **Comprehensive Answers:** For every question, the AI provides:
  - 📝 A detailed, interview-ready model answer.
  - 💡 A simple, conversational explanation to understand the core concept.
  - 💻 A practical real-world or code example.
  - 🔑 Important technical keywords to remember.
  - 🎤 A follow-up question an interviewer might ask next.
- **Interactive UI:** A clean, responsive user interface built with Streamlit.

## 🛠️ Tech Stack

- **Frontend:** Streamlit
- **AI Framework:** LangChain
- **LLM Provider:** OpenRouter (Defaults to `openai/gpt-4o-mini` for reliable structured output)
- **Data Validation:** Pydantic
- **Environment Management:** python-dotenv

## 🚀 Getting Started

Follow these steps to run the project locally on your machine.

### 1. Prerequisites
- Python 3.9 or higher installed.
- An [OpenRouter API Key](https://openrouter.ai/keys).

### 2. Clone the Repository
git clone https://github.com/akshathahr-git/AI_Placement_Preparation_Assistant.git
cd AI_Placement_Preparation_Assistant

### 3. Create a Virtual Environment
For Windows:
python -m venv venv
venv\Scripts\activate

For macOS/Linux:
python3 -m venv venv
source venv/bin/activate

### 4. Install Dependencies
pip install -r requirements.txt

### 5. Configure Environment Variables
Create a file named `.env` in the root directory of the project and add your OpenRouter API key:
OPENROUTER_API_KEY=your_openrouter_api_key_here
MODEL_NAME=openai/gpt-4o-mini

(Note: You can change `MODEL_NAME` to any valid model ID available on OpenRouter, such as `anthropic/claude-3.5-sonnet`).

### 6. Run the Application
streamlit run app.py

The app will open in your default web browser at `http://localhost:8501`.

## 📂 Project Structure

AI_Placement_Preparation_Assistant/
│
├── app.py                # Main Streamlit UI and application logic
├── generator.py          # LangChain setup, LLM initialization, and generation logic
├── prompts.py            # LangChain prompt templates and output parsers
├── schemas.py            # Pydantic models for structured output validation
├── requirements.txt      # Project dependencies
├── .env                  # API keys (git-ignored)
└── README.md             # Project documentation

