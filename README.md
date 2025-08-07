
# 🇬🇧 UK Job Listings Analysis — Live Data from Reed.co.uk

This project fetches and analyzes **real-time job listings** from the [Reed.co.uk API](https://www.reed.co.uk/developer), supporting **any job role** such as **Data Analyst**, **Web Developer**, **UI/UX Designer**, **Database Administrator**, and more. It performs cleaning, feature engineering, and exploratory data analysis to generate insights that benefit **both job seekers and recruiters**.

---

## 🔍 What This Project Does

- Scrapes live job postings using the Reed.co.uk API
- Filters and cleans noisy or missing data
- Derives new metrics like job age and average salary
- Visualizes trends in:
  - Salary vs location / employer
  - Applications vs salary / job age
  - Posting freshness
  - Hidden gems (high pay, low competition)
- Supports dynamic job keyword targeting (e.g. "data analyst", "ML engineer")

---

## 🛠 Requirements

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/maqeel019/reed-job-UK-analysis.git
cd job-market-analysis

# 2. Set your Reed API key
export REED_API_KEY="your-own-api-key"   # or use a .env file

# 3. Open and run the notebook
jupyter notebook job_analysis.ipynb
```

---

## 📊 Analyses Included

- 📈 Salary Distribution (Filtered)
- 🏙️ Salary by Location (Top 15 Cities)
- 🏢 Salary by Employer (Top 15)
- 📉 Job Age vs Applications
- 🔍 Correlation Matrix (Salary, Applications, Job Age)
- 🎯 High Salary + Low Application Jobs (Hidden Opportunities)
- 🏆 Top Employers by Job Count
- 🧭 Remote / Hybrid Breakdown
- 📅 Job Posting Age Distribution
- ⚖️ Applications per Job Average

---

## 🔐 API Key Security

This project uses the Reed.co.uk API. You must obtain your own API key from their [developer portal](https://www.reed.co.uk/developer).

**Important:**

- Do **not** share your key publicly
- Do **not** push it to GitHub or leave it in notebooks

Instead, securely load it:

```python
import os
reed_key = os.getenv("REED_API_KEY")
```

Use a `.env` file locally (optional):

```env
REED_API_KEY=your-key-here
```

Add `.env` to your `.gitignore` file to avoid uploading it.

---

## 📁 Folder Structure

```
job-market-analysis/
├── job_analysis.ipynb        # 🔍 All-in-one notebook
├── requirements.txt          # 📦 Libraries used
├── .env                      # 🔐 Your secret API key (not committed)
├── .gitignore                # ❌ Prevents leaking secrets
└── README.md                 # 📘 You're reading it!
```

---

## 🧠 Author

**Muhammad Aqeel**
🔗 [LinkedIn](https://www.linkedin.com/in/aqeelkhan09/)  
📧 <mailto:maqeelcs09@gmail.com>

---
