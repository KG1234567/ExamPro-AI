# 🤖 ExamPro AI – AI Powered Quiz Generation System
## 📌 Project Overview

ExamPro AI is an AI-powered web application that dynamically generates quizzes using Generative AI and Large Language Models (LLMs). The system allows users to create customized quizzes based on a selected topic, difficulty level, and number of questions.

The platform is designed to help students preparing for competitive examinations like UPSC and PCS by providing instant practice questions and immediate feedback.

Unlike traditional static question banks, ExamPro AI generates unique questions on demand, enabling unlimited practice and faster learning cycles.

# 🎯 Objectives
The main objectives of this project are:

1. To build an AI-based quiz generation system

2. To automate the creation of practice questions

3. To provide instant feedback and scoring

4. To demonstrate the application of Generative AI in education

5. To create an interactive learning platform for exam preparation

# 🧠 Key Features
1. 📝 Dynamic Quiz Generation using AI

2. 🎯 Topic-based question generation

3. 📊 Difficulty levels (Easy, Medium, Hard)

4. ❓ Supports MCQ and Fill in the Blank questions

5. ⚡ Low latency question generation

6. 📈 Instant scoring and detailed explanations

7. 📁 Export quiz results to CSV

8. 🖥️ Interactive web interface using Streamlit

# 🏗️ System Architecture
The application follows a two-tier architecture:

```
User (Browser)
       │
       ▼
Streamlit Application (Python)
       │
       ▼
Groq API (LLM Model)
```

The system converts user input into prompts, sends them to the AI model, and returns structured quiz questions.

# ⚙️ Technology Stack
```
| Technology    | Purpose                   |
| ------------- | ------------------------- |
| Python        | Core programming language |
| Streamlit     | Web application interface |
| Groq API      | AI model inference        |
| LangChain     | LLM integration           |
| Pydantic      | Data validation           |
| Pandas        | Data analysis & export    |
| python-dotenv | Secure API key management |
```

# 📂 Project Structure
```
ExamPro-AI
│
├── app.py                # Main Streamlit application
├── utils.py              # Quiz generation logic
├── requirements.txt      # Project dependencies
├── .env                  # API keys (not uploaded to GitHub)
│
├── results/
│   └── results.csv       # Quiz result exports
│
├── screenshots/
│   ├── dashboard.png
│   ├── quiz_interface.png
│   └── results_page.png
│
└── README.md
```

# 🚀 How to Run the Project
## 1️⃣ Clone the repository
```
git clone https://github.com/KG1234567/ExamPro-AI.git
cd ExamPro-AI
```

## 2️⃣ Create a virtual environment
``` python -m venv .venv ```
Activate Environment
Windows:
``` .venv\Scripts\activate  ```

## 3️⃣ Install dependencies
``` pip install -r requirements.txt ```

## 4️⃣ Add Groq API Key
Create a .env file and add:
``` GROQ_API_KEY=your_api_key_here ```

## 5️⃣ Run the application
``` streamlit run app.py ```
The application will run in your browser.

# 📊 Application Workflow
1️⃣ User enters topic, difficulty, and number of questions

2️⃣ Application sends prompt to Groq LLM

3️⃣ AI generates quiz questions

4️⃣ Questions are validated using Pydantic schemas

5️⃣ User attempts the quiz

6️⃣ System calculates score and displays explanations

7️⃣ Results can be exported as CSV

# 🧪 Testing
The system was tested for:

1. Question generation accuracy

2. API response handling

3. UI interaction

4. Result calculation

Average question generation time:

~1.4 seconds for 5 questions

# ⚠️ Limitations
1. Requires internet connection

2. Dependent on external AI API

3. Possible AI hallucinations in rare cases

4. No user login or database storage yet

# 🔮 Future Enhancements
1. Adaptive learning system

2. User accounts and progress tracking

3. Multilingual quiz generation

4. Cloud database integration

5. Mobile application support

# 📚 References
1. Groq API Documentation

2. Streamlit Documentation

3. LangChain Documentation

4. Pydantic Documentation



