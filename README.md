# AspireIQ

This Streamlit app analyzes uploaded resumes to match skills with a selected job role. It also recommends online courses for missing skills using GPT-based models. The app generates course suggestions from platforms like Udemy, Coursera, and YouTube to help users improve their skill sets.

## Features
- **Resume Analysis**: Upload a resume (PDF format) and select a job role to match the skills in the resume.
- **Skill Matching**: Compare required skills for the chosen job role with those found in the resume.
- **Course Recommendations**: If any skills are missing, the app recommends relevant courses from platforms like Udemy, Coursera, and YouTube.
- **Fuzzy Matching**: Uses fuzzy matching to identify skills, even with slight variations in the text.

## Requirements
- Python 3.x
- Streamlit
- pdfplumber
- fuzzywuzzy
- requests
- HuggingFace API key (for course recommendations)

## Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/resume-analyzer.git
    cd resume-analyzer
    ```

2. Create a virtual environment and activate it:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Create a `.env` file and add your HuggingFace API key:
    ```
    HUGGINGFACEHUB_API_TOKEN=your_api_key_here
    ```

5. Run the app:
    ```bash
    streamlit run app.py
    ```

## Usage

1. Upload a PDF resume.
2. Select a job role (e.g., Data Scientist, Web Developer).
3. Click the "Analyze Resume" button to view matched skills and missing skills.
4. The app will recommend online courses for the missing skills.


