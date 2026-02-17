#  AI Interview Practice & Resume Screening Platform

An NLP + Machine Learning based Resume-Job Matching and Candidate Screening System built for Hackathon.

This system automatically evaluates resumes against job descriptions and predicts selection probability using Natural Language Processing and Machine Learning.


##  Problem Statement

Manual resume screening is time-consuming and inefficient.

This project builds an AI-powered system that:

- Screens resumes automatically
- Matches candidates with job descriptions
- Predicts selection probability
- Calculates resume-job similarity score
- Provides decision support for recruiters


##  Project Workflow

Dataset → Data Cleaning → EDA → Feature Engineering → TF-IDF → ML Model → Evaluation → Gradio Interface


##  Features

✔ Exploratory Data Analysis (EDA)  
✔ Text Preprocessing (Cleaning + Combining Fields)  
✔ TF-IDF Vectorization  
✔ Binary Classification Model  
✔ Confusion Matrix  
✔ Classification Report  
✔ Resume-Job Similarity Score  
✔ Interactive Gradio Interface  


##  Dataset Columns Used

- career_objective  
- skills  
- skills_required  
- job_position_name  
- matched_score  

Target Variable:

selected = 1 if matched_score >= median else 0


This ensures balanced classification.


##  Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- TF-IDF Vectorizer
- Logistic Regression / Random Forest
- Gradio


##  Model Evaluation

Metrics Used:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- ROC-AUC

Example Confusion Matrix:


[[True Negative   False Positive]
 [False Negative  True Positive]]


##  Resume Screening Logic

1. Combine:
   - Career Objective
   - Skills
   - Skills Required
   - Job Position

2. Convert combined text into TF-IDF vectors

3. Model Predicts:
   - Selection Decision
   - Selection Probability

4. Calculate Similarity Score between Resume and Job Description


##  How to Run Locally

### 1️ Clone Repository


git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name


### 2️ Install Dependencies


pip install -r requirements.txt


### 3️ Run Application


python app.py


##  Deployment Options

- Google Colab (Gradio share link)
- HuggingFace Spaces
- Local Machine
- Cloud Platforms (Render / Railway)


##  Sample Output

Prediction: Strong Match - High Selection Chance  
Selection Probability: 84.25 %  
Resume-Job Similarity: 78 %


##  Hackathon Highlights

- Dynamic target creation using statistical threshold
- Balanced dataset validation
- NLP-based semantic matching
- End-to-end ML pipeline
- Interactive AI-powered screening system
- Real-world resume-job dataset


##  Future Improvements

- Deep Learning Model (BERT-based matching)
- Multi-class job category prediction
- Candidate ranking system
- Skill gap recommendation engine
- Interview question generation module
