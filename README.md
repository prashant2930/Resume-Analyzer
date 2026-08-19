# 📄 ATS Resume Analyzer

An AI-powered ATS (Applicant Tracking System) resume analyzer that evaluates resumes against job descriptions, calculates match percentages, and generates actionable feedback using Google Gemini 2.0 Flash and PyMuPDF.

---

## 🌐 Overview

Job applicants often submit resumes without knowing how effectively their qualifications align with applicant tracking systems (ATS) or specific job postings. **ATS Resume Analyzer** automates resume critique by extracting text from PDF documents, passing structured prompts to Google Gemini 2.0 Flash, and parsing match scores and recommendations.

### Key Features
* 📄 **Local PDF Text Extraction**: High-fidelity text parsing from uploaded PDF resumes using PyMuPDF (`fitz`).
* 🤖 **Gemini 2.0 Flash Integration**: Generates deep ATS compatibility analysis, missing keyword identification, and strengths/weaknesses breakdown.
* 📊 **Dynamic Match Score Parsing**: Regex extraction of match percentages rendered via Streamlit progress bars.
* 📥 **Report Export**: Instant plain-text report download functionality for offline review.

---

## 🛠️ Tech Stack

* **Frontend / UI**: Streamlit
* **AI Provider**: Google Generative AI (`gemini-2.0-flash`)
* **PDF Engine**: PyMuPDF (`pymupdf`)
* **Environment Management**: `python-dotenv`

---

## 🚀 Installation & Local Execution

### Prerequisites
* Python 3.10 or higher
* Google Gemini API Key (`GOOGLE_API_KEY`)

### Local Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/prashant2930/Resume-Analyzer.git
   cd Resume-Analyzer
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure environment**:
   Create a `.env` file in the root directory:
   ```env
   GOOGLE_API_KEY=your_gemini_api_key_here
   PROMPT=Analyze the following resume against the job description...
   ```

4. **Launch Streamlit app**:
   ```bash
   streamlit run app.py
   ```
   Open [http://localhost:8501](http://localhost:8501) in your browser.

---

## 👨‍💻 Author

**Prashant Srivastava** — Software Engineer
