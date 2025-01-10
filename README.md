# Resume Optimization and Job Market Analysis

## Overview
This project focuses on optimizing resumes based on job role requirements and analyzing the job market trends. It uses AI-powered tools and APIs, including Cohere API for language processing and Indeed API for job scraping, to provide suggestions for resume improvements and predict job market trends.

The project consists of two main components:
1. **Resume Optimization**: Optimizes a user's resume by detecting mistakes and suggesting missing skills based on the job role.
2. **Job Market Analysis**: Scrapes job listings from various websites (primarily Indeed) to analyze the job market and predict the demand for specific skills.

## Files Description

- **Resume Optimization**:
  - **cohere_api_integration.py**: Implements Cohere API to analyze the content of resumes, checking for common mistakes and missing skills relevant to the job role.
  - **pdf_extractor.py**: Parses resume PDFs to extract content for analysis.
  - **resume_suggestions.py**: Generates suggestions for resume improvement by comparing the extracted resume content with job requirements.

- **Job Market Analysis**:
  - **indeed_api_scraper.py**: Uses the Indeed API to scrape job listings and identify the most in-demand skills for specific roles.
  - **job_market_trends.py**: Analyzes job listings data to predict the demand for specific skills in the job market.
  - **data_cleaning.py**: Cleans and preprocesses the scraped job market data.
  
- **AI Model**:
  - **job_skill_predictor.py**: Uses an AI model to predict the skills required for a job role based on job listings.
  - **skill_demand_model.py**: A machine learning model that analyzes job market data to forecast future trends in skill demand.

## Data Collection

1. **Resume Data**:
   - Resumes are parsed using **pdf_extractor.py** to extract textual content from PDF resumes.
   - The extracted content is analyzed using the **Cohere API** to detect errors and missing skills related to the desired job role.

2. **Job Market Data**:
   - The project scrapes job listings from **Indeed** using the **Indeed API**. These listings provide valuable insights into job roles, required skills, salaries, and locations.
   - The job listings are cleaned and preprocessed using **data_cleaning.py** for further analysis and model prediction.

## Features

### Resume Optimization:
- **Resume Parsing**: Parse resumes from PDF format and extract key information.
- **Mistake Detection**: Identify and suggest fixes for common resume mistakes, such as spelling errors, formatting issues, or lack of relevant experience.
- **Skill Gap Analysis**: Based on the user's desired job role, suggest missing skills and keywords that could enhance the resume for better job compatibility.
  
### Job Market Analysis:
- **Job Trend Analysis**: Scrape job listings to track the most in-demand skills in various job roles.
- **Predict Skill Demand**: Using the machine learning model (**skill_demand_model.py**), predict which skills will be in demand in the future based on current job listings.

## How It Works

1. **Resume Optimization**:
   - The user uploads their resume (in PDF format).
   - The resume content is parsed and analyzed using Cohere's API to identify mistakes, missing skills, and suggest improvements tailored to the job role.
   - Based on the job role input by the user, the system compares the resume against job listings and suggests improvements to match industry standards.

2. **Job Market Analysis**:
   - The system scrapes job listings from Indeed using the Indeed API, extracting relevant information such as job titles, required skills, and locations.
   - The data is cleaned and analyzed to forecast trends in skill demand, providing insights into which skills are most sought after in specific job roles.
   - A machine learning model is trained to predict future skill demand, helping users understand which skills will be valuable in the job market.

## Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/Resume-Optimization-and-Job-Market-Analysis.git
   ```

2. **Install Dependencies**:
   Make sure to install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Resume Optimization**:
   To optimize a resume, run the script:
   ```bash
   python resume_suggestions.py --resume path_to_resume.pdf --role "Data Scientist"
   ```

4. **Run Job Market Analysis**:
   To analyze the job market trends, run:
   ```bash
   python job_market_trends.py --role "Data Scientist"
   ```

## Tools & APIs Used
- **Cohere API**: For natural language processing tasks like resume analysis, skill matching, and mistake detection.
- **Indeed API**: For scraping job listings data to analyze job trends and skills demand.
- **PDF Extractor**: For extracting text from resumes in PDF format.
- **Machine Learning Models**: To predict skill demand and job market trends.
