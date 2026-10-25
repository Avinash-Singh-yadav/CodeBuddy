# CodeBuddy — AI Code Reviewer

CodeBuddy is a beginner-friendly AI-powered code review tool built with Python, Streamlit, and Google's Gemini API. It helps developers understand their code, identify potential bugs, improve code quality, and learn better programming practices.

## Features

- **AI-powered code reviews** using Google's Gemini API.
- **Multiple programming languages** — currently Java and Python.
- **Review focus selection** to guide the feedback.
- **Potential bug detection** with explanations of possible issues.
- **Code quality feedback** covering readability, naming, and maintainability.
- **Suggested improvements** with corrected code when useful.
- **Beginner-friendly learning takeaways**.
- **Simple web interface** powered by Streamlit.

## Tech Stack

- Python
- Streamlit
- Google Gen AI Python SDK
- Google Gemini API

## Project Structure

```text
codebuddy/
├── .streamlit/
│   └── secrets.toml
├── .gitignore
├── app.py
├── requirements.txt
└── README.md
```

The `secrets.toml` file stores the local API key and must not be committed to GitHub.

## Getting Started

### Prerequisites

- Python 3.10 or a compatible newer version
- pip
- A Google AI Studio API key

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd codebuddy
```

Replace `YOUR_GITHUB_REPOSITORY_URL` with your actual repository URL.

### 2. Create a virtual environment

On Windows PowerShell:

```powershell
py -m venv .venv
```

Activate it:

```powershell
.\.venv\Scripts\Activate.ps1
```

### 3. Install dependencies

```powershell
python -m pip install -r requirements.txt
```

### 4. Configure the API key

Create a file at `.streamlit/secrets.toml` with the following content:

```toml
GOOGLE_API_KEY = "YOUR_GOOGLE_GEMINI_API_KEY"
```

Replace the placeholder with your own API key. Never publish your real key in source code, screenshots, or public repositories.

You can obtain an API key through [Google AI Studio](https://aistudio.google.com/).

### 5. Run CodeBuddy

```powershell
python -m streamlit run app.py
```

Open the local URL printed in the terminal, normally `http://localhost:8501`.

## How to Use

1. Open CodeBuddy in your browser.
2. Choose a programming language.
3. Enter your code or load an example.
4. Select the review focus.
5. Click **Review My Code**.
6. Read the summary, potential bugs, code quality feedback, suggested improvements, and learning takeaway.

## Important Notes

- AI-generated reviews can be incorrect or incomplete. Verify suggestions before applying them.
- CodeBuddy analyzes submitted code; it does not execute the submitted program.
- API availability, rate limits, and usage charges depend on Google's current API terms and account configuration.
- Never submit passwords, API keys, private credentials, or confidential source code.

## Future Improvements

- More programming languages
- Severity levels for identified issues
- Line-specific feedback
- Review history
- Improved error handling and response times
- Automated tests and deployment

## Author

Built as a personal learning project to explore Python, AI integration, API usage, and software development.

**CodeBuddy — Understand your code. Improve your skills.**