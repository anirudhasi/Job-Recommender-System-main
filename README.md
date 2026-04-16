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

Install dependencies:

```bash
pip install -r requirements.txt
```

Create a `.env` file in the project root:

```env
OPENAI_API_KEY=your_openai_api_key
APIFY_API_TOKEN=your_apify_api_token
```

Run the app:

```bash
streamlit run app.py
```

## Streamlit Cloud Deployment

When deploying to Streamlit Cloud, add these values in the app's secrets/settings instead of committing them to GitHub:

```env
OPENAI_API_KEY=your_openai_api_key
APIFY_API_TOKEN=your_apify_api_token
```

Use `app.py` as the main file.
