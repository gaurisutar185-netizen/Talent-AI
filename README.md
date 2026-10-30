Talent-AI - Smart Resume Screening

Final Year Project - M.Sc Data Analytics (2026-27)
Pillai College of Arts, Commerce & Science, Panvel.

Under Guidance of Prof. Soly Zachariah.

Team Members:
- Gauri Sutar (Roll No: 23)
- Vishakha Pagare 
- Mansi Tambe


About Project:
In campus placement we saw recruiters take 2-3 days to shortlist resumes. So we built Talent-AI to automate it.

We tried only keyword matching first, but it was failing for synonyms like "JS" vs "JavaScript". So we added BERT.

How it Works:
1. User uploads Job Description (JD)
2. Uploads 10-50 Resumes in PDF format
3. System extracts text using PyMuPDF
4. Calculates 2 scores:
   - TF-IDF score for keyword match
   - BERT score for meaning
1. Final Score = (BERT * 0.7) + (TF-IDF * 0.3)
2. Shows ranked list with %.

Accuracy:
Tested on 50 sample resumes (Data Analyst roles). Got ~89% accuracy compared to manual shortlisting by our HOD. 


How to Run on Your Laptop:
bash
pip install -r requirements.txt
streamlit run app.py
