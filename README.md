# 🤖 AI Resume ATS Checker

AI Resume ATS Checker is an intelligent web application that analyzes a resume against a job description and simulates real-world Applicant Tracking Systems (ATS). It leverages Google Gemini AI to calculate resume-job compatibility, identify missing skills, and generate improvement suggestions to increase interview shortlisting chances.

---

## 📌 Why This Project?

Over 90% of companies use ATS software to filter resumes before a human recruiter sees them.  
This project helps job seekers understand how ATS evaluates resumes and optimize their profiles accordingly.

---

## ✨ Key Features

- Upload PDF resume
- Paste any job description
- AI-powered ATS simulation
- Resume Match Percentage Score
- Matching Skills Detection
- Missing Skills Identification
- Resume Optimization Suggestions
- Clean modern UI (Tailwind)
- Works completely locally
- No data storage

---

## 🧠 How It Works

1. User uploads resume (PDF)
2. User pastes job description
3. System extracts resume text using PyPDF2
4. Gemini AI compares resume vs JD
5. ATS-style JSON analysis is returned
6. Frontend displays results instantly

---

## 🛠 Tech Stack

| Layer | Technology |
|------|-----------|
| Frontend | HTML, Tailwind CSS, JavaScript |
| Backend | Python, Flask |
| AI Model | Google Gemini 2.5 Flash |
| PDF Reader | PyPDF2 |

---

## 📁 Repository Structure

---

## ⚙ Installation Guide

### Step 1 – Clone Repository
```bash
git clone https://github.com/yourusername/ats-checker.git
cd ats-checker
python -m venv venv
source venv/bin/activate    # Windows: venv\Scripts\activate
pip install flask PyPDF2 google-generativeai
client = Client(api_key="YOUR_GEMINI_API_KEY")
python app.py
http://localhost:2000
{
  "match_percentage": 78,
  "match_summary": "Good alignment with backend development roles.",
  "matching_skills": ["Python", "Flask", "REST APIs"],
  "missing_skills": ["Docker", "AWS"],
  "improvement_suggestions": [
    "Add cloud deployment experience",
    "Include more quantifiable achievements"
  ]
}

---

If you want, I can also generate:
- `requirements.txt`
- `.env` version with secure API key
- One-click cloud deployment version
