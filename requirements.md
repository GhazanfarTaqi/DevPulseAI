# DevPulse AI

> An AI-powered platform that analyzes real-world job market data to deliver technology trend insights, salary predictions, skill recommendations, and personalized career roadmaps for software developers.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Machine Learning Models](#machine-learning-models)
- [MVP Scope](#mvp-scope)
- [Non-Functional Requirements](#non-functional-requirements)

---

## Overview

DevPulse AI collects job postings from multiple sources through automated web scraping, processes the data using NLP and ML pipelines, and surfaces actionable insights through an intuitive dashboard — helping developers stay ahead of market trends and make informed career decisions.

---

## Features

### 🔍 Data Collection
- Scrapes job postings from multiple job portals and company career pages
- Collects: Job Title, Company, Location, Salary, Experience, Employment Type, Skills, Description, Posting Date, and URL
- Scheduled automatic scraping with deduplication and validation

### ⚙️ Data Processing
- NLP-based skill extraction from job descriptions
- Skill normalization (e.g. `ReactJS → React`, `JS → JavaScript`)
- Salary standardization across formats
- HTML cleaning, special character removal, and location normalization

### 📊 Analytics Dashboard
- Trending and in-demand skills
- Hiring trends and company hiring statistics
- Geographic demand analysis
- Experience-level and salary distribution

### 💰 Salary Prediction
- Input your skills, experience level, and location
- Get an estimated salary range powered by ML

### 🧭 Recommendation Engine
- **Skill Gap Analysis** — compare your skills against market demand
- **Learning Recommendations** — discover the next technologies to learn
- **Career Roadmap** — personalized learning paths based on your career goals

### 📄 Resume Analyzer
- Accepts PDF and DOCX resumes
- Extracts skills and experience automatically
- Generates a **Market Fit Score**
- Identifies missing skills relative to market demand

### 🎯 Job Matching
- Builds user profiles
- Matches users with relevant job postings
- Calculates a **Job Match Score** per listing

### 📈 Trend Forecasting
- Predicts future demand for specific technologies
- Identifies emerging skills before they peak
- Forecasts hiring trends over time

### 👤 User Management
- Registration, login, and profile management
- Save reports and personalized learning roadmaps

### 🛠️ Admin Panel
- Monitor and manage scraping jobs
- Track data quality metrics
- Retrain ML models
- Manage datasets

---

## Machine Learning Models

| # | Model | Purpose |
|---|-------|---------|
| 1 | Skill Extraction (NLP) | Extract skills from unstructured job descriptions |
| 2 | Salary Prediction | Estimate salary ranges from user inputs |
| 3 | Job Category Classification | Automatically classify job postings |
| 4 | Skill Recommendation System | Suggest skills to learn next |
| 5 | Job Matching | Score and rank jobs for each user |
| 6 | Trend Forecasting | Predict future technology demand |

---

## MVP Scope

The initial release focuses on the core value loop:

- [x] Job Scraping
- [x] Data Cleaning
- [x] Skill Extraction
- [x] Skill Demand Dashboard
- [x] Salary Prediction
- [x] Skill Gap Analysis
- [x] Learning Recommendations

---

## Non-Functional Requirements

| Category | Requirement |
|----------|-------------|
| **Performance** | Dashboard loads in < 3s; search results in < 1s |
| **Scalability** | Supports 100,000+ job records; modular architecture |
| **Security** | Secure auth, protected user data, API authorization |
| **Reliability** | Automated backups, scheduled scraping, logging & monitoring |
| **Usability** | Responsive UI, intuitive dashboard, clear visualizations |