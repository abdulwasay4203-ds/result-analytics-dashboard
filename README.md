# Result Analytics Dashboard

An interactive academic-performance dashboard built as **Module 4** of the **Technify University ERP** team project (Data Science Team 1).

The dashboard reads live data from a Supabase PostgreSQL database and turns exam results into KPIs, filters and charts for departments, semesters and exam types.

> This repository contains my module only. The full ERP system is a team project: https://github.com/qurban72/University-ERP-System-

## Features

- **KPI cards:** total students, average CGPA, average score, pass rate, fail rate and top scorers (80% and above)
- **Filters:** department, semester and exam type
- **Charts:**
  - Average CGPA by department
  - Pass vs fail rate
  - Semester-wise average score with a 50% pass line
  - Department pass rate
  - Grade distribution (A to F)
  - Top 10 students by CGPA
  - CGPA trend by department across semesters

## Tech stack

Python, Streamlit, Pandas, Plotly, PostgreSQL (Supabase), psycopg2

## Run locally

1. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

2. Create `.streamlit/secrets.toml` using `secrets.toml.example` as a template and add your own database credentials.

3. Start the app:

   ```bash
   streamlit run app.py
   ```

The database must contain the tables `results`, `students`, `departments`, `programs`, `enrollments` and `exams`.

## Author

Abdul Wasay, Software Engineering student, University of Sindh.
GitHub: [abdulwasay4203-ds](https://github.com/abdulwasay4203-ds) · LinkedIn: [abdul-wasay-datascientist](https://www.linkedin.com/in/abdul-wasay-datascientist/)
