# AI Job Recommender

A Streamlit app that analyzes a PDF resume with OpenAI and recommends jobs from LinkedIn and Naukri using Apify actors.

## Features

- Upload a resume in PDF format
- Extract resume text with PyMuPDF
- Generate a resume summary
- Identify skill gaps and missing areas
- Suggest a career roadmap
- Generate job-search keywords
- Fetch job listings from LinkedIn and Naukri

## Tech Stack

- Python
- Streamlit
- OpenAI API
- Apify API
- PyMuPDF
- python-dotenv

## Setup

This project was tested locally with Python 3.12. If your machine has multiple Python versions installed, make sure you install dependencies and run Streamlit with the same Python interpreter.

Install dependencies:

```bash
pip install -r requirements.txt
```

On Windows, if `python` points to a different Python version, use the full Python 3.12 path:

```powershell
C:\Users\sangi\AppData\Local\Programs\Python\Python312\python.exe -m pip install -r requirements.txt
```

Create a `.env` file in the project root:

```env
OPENAI_API_KEY=your_openai_api_key
APIFY_API_TOKEN=your_apify_api_token
```

Do not commit `.env` to GitHub. It is already ignored by `.gitignore`.

Run the app:

```bash
streamlit run app.py
```

On Windows, if Streamlit is installed under Python 3.12, run:

```powershell
C:\Users\sangi\AppData\Local\Programs\Python\Python312\python.exe -m streamlit run app.py --server.port 8501
```

Then open:

```text
http://localhost:8501
```

## Streamlit Cloud Deployment

When deploying to Streamlit Cloud, add these values in the app's secrets/settings instead of committing them to GitHub:

```toml
OPENAI_API_KEY = "your_openai_api_key"
APIFY_API_TOKEN = "your_apify_api_token"
```

Use `app.py` as the main file.
