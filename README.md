# AI Powered Resume Screener

An NLP-based tool that analyzes how well a resume matches a job description, identifies missing keywords, and generates intelligent feedback using Google Gemini AI.

## What it does
- Takes any resume and job description as input
- Calculates a match score using TF-IDF vectorization and Cosine Similarity
- Identifies missing skills and keywords from the job description
- Generates actionable AI feedback using Google Gemini API

## Tech Stack
Python, NLTK, Scikit-learn, Google Gemini API, Jupyter Notebook

## NLP Pipeline
1. Text Preprocessing — Lowercasing, punctuation removal, stopword removal, lemmatization
2. TF-IDF Vectorization — Converts text documents into numerical vectors
3. Cosine Similarity — Measures match score between resume and job description
4. Keyword Gap Analysis — Identifies skills present in JD but missing from resume
5. LLM Integration — Gemini AI generates human-like feedback and recommendations

## Sample Output
MATCH SCORE: 14.73%

MISSING KEYWORDS:
  - tensorflow
  - pytorch
  - aws
  - azure
  - nlp
  - tableau

AI FEEDBACK:
Your foundational Python and SQL experience is a good start. However, this role requires deep learning frameworks (TensorFlow, PyTorch) and cloud platform experience (AWS/Azure) which are currently missing from your resume.

## How to Run
1. Clone the repo
2. Install dependencies: pip install nltk scikit-learn google-generativeai
3. Add your Gemini API key in Cell 12
4. Run all cells in resume_screener.ipynb
5. Paste your resume and job description when prompted
