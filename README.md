# Resume Optimizer 🚀

An NLP-powered tool to analyze job descriptions and optimize resumes for ATS compatibility using keyword matching and actionable suggestions.

## Features ✨
- **JD Keyword Extraction**: Identifies top skills/requirements from job descriptions using TF-IDF.
- **Resume Gap Analysis**: Highlights missing keywords in your resume.
- **Smart Suggestions**: Recommends improvements to boost ATS scores.
- **Match Score**: Quantifies resume-JD compatibility with cosine similarity.

## Tech Stack 🛠️
- **NLP**: `spaCy`, `scikit-learn` (TF-IDF)
- **Backend**: Python, Pandas
- 
## Installation 📦
1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/resume-optimizer.git
   cd resume-optimizer

2. Install dependencies:
   pip install -r requirements.txt

3. Download spaCy model:
   python -m spacy download en_core_web_sm


Usage 🖥️
1. Add your resume as resume.pdf in the /data folder.

2. Add job descriptions as job_descriptions.csv (columns: job_title, job_description).

3. Run the optimizer:
   streamlit run app.py


**Code Structure 📂**

resume-optimizer/
├── data/               # Sample resumes/JDs
├── nlp/                # TF-IDF and spaCy scripts
│   ├── keyword_extractor.py
│   └── resume_parser.py
├── app.py              # Streamlit app
├── requirements.txt
└── README.md


**Example Output 📄**

✅ Match Score: 78%  
🔍 Missing Keywords: pytorch, aws, airflow  
💡 Suggestions:  
   - Add "Built PyTorch models for computer vision tasks"  
   - Include "AWS (S3, EC2)" in Skills  
   - Mention "Automated pipelines with Apache Airflow"



