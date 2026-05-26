# JobSuite AI — Backend

> FastAPI backend powering JobSuite AI — resume analysis, cover letter generation, and job description matching using Groq LLM.

![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=flat&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-0.111-009688?style=flat&logo=fastapi&logoColor=white)
![Groq](https://img.shields.io/badge/LLM-Groq_Llama_3-orange?style=flat)
![Deployed on Render](https://img.shields.io/badge/Deployed_on-Render-46E3B7?style=flat&logo=render&logoColor=white)

**Live API:** coming soon  
**Frontend Repo:** [jobsuite-ai](https://github.com/Yusufcommit/jobsuite-ai)  
**API Docs:** /docs (Swagger UI)

---

## What It Does

Three AI-powered endpoints that help job seekers optimize their applications:

- **Resume Analyzer** — scores a resume and returns strengths, weaknesses, and improvements
- **Cover Letter Generator** — generates a tailored cover letter from a resume and job description
- **JD Matcher** — calculates match score, detects skill gaps, and returns AI tips

---

## API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| `GET` | `/` | Health check |
| `POST` | `/analyze-resume` | Analyze and score a resume |
| `POST` | `/generate-cover-letter` | Generate a tailored cover letter |
| `POST` | `/match-job` | Match resume to job description |

---

## Tech Stack

| Layer | Technology |
|---|---|
| Framework | FastAPI |
| Language | Python 3.11 |
| LLM | Groq — Llama 3.3 70B |
| Similarity | TF-IDF + cosine similarity |
| Resume Parsing | pdfplumber + python-docx |
| Deployment | Render |

---

## Run Locally

```bash
# 1. Clone the repo
git clone https://github.com/Yusufcommit/jobsuite-backend.git
cd jobsuite-backend

# 2. Create virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Add your Groq API key
echo "GROQ_API_KEY=your_key_here" > .env

# 5. Start the server
uvicorn main:app --reload
```

API runs at `http://localhost:8000`  
Swagger docs at `http://localhost:8000/docs`

---

## Roadmap

- [x] Resume analysis with LLM scoring
- [x] Cover letter generation with tone options
- [x] JD matching with skill gap detection
- [x] AI tips per job application
- [ ] PostgreSQL session storage
- [ ] JWT authentication
- [ ] Docker + CI/CD pipeline
- [ ] API versioning

---

## Related

- **Frontend:** [jobsuite-ai](https://github.com/Yusufcommit/jobsuite-ai)
- **HireLens AI:** [hirelens-ai](https://github.com/Yusufcommit/hirelens-ai)

---

## Built by Yusuf

**Yusuf Abdirashid** — AI Full Stack Developer  
Building polished AI-powered tools for hiring and job applications.

[![GitHub](https://img.shields.io/badge/GitHub-Yusufcommit-181717?style=flat&logo=github)](https://github.com/Yusufcommit)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Yusuf_Abdirashid-0A66C2?style=flat&logo=linkedin)](https://tr.linkedin.com/in/yusuf-abdirashid)
[![Email](https://img.shields.io/badge/Email-yusufabdirashid100@gmail.com-EA4335?style=flat&logo=gmail)](mailto:yusufabdirashid100@gmail.com)