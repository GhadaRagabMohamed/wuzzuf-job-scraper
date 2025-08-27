# 📝 Wuzzuf Job Scraper & Data Analysis

## 📌 Project Overview
This project scrapes job listings from [Wuzzuf](https://wuzzuf.net) for the role **"Data Analyst"** using Python.  
After collecting the data, it performs **data cleaning, preprocessing, and exploratory data analysis (EDA)** to uncover job market insights such as:
- Most in-demand skills  
- Top hiring companies  
- Job level distribution (Junior / Mid / Senior)  
- Most common job locations in Egypt  

> ⚠️ Note: The dataset file (`wuzzuf_jobs_data.csv` / `wuzzuf_jobs_data.xlsx`) is **not included** in this repository.  
> You can generate the dataset by running the scraper script to fetch the latest job listings from Wuzzuf.

---

## ⚙️ Technologies Used
- **Python** 🐍  
- **Libraries**:
  - `requests` & `BeautifulSoup` → Web scraping  
  - `pandas` & `numpy` → Data handling  
  - `matplotlib` & `seaborn` → Data visualization  
  - `WordCloud` → Skill keywords visualization  

---

## 📊 Workflow

### 1. Web Scraping
- Scraped up to **50 pages** (~15 jobs per page).  
- Extracted the following fields:
  - **Job Title**  
  - **Company**  
  - **Location**  
  - **Skills / Requirements**  
  - **Job Link**  

👉 Data saved into:
- `wuzzuf_jobs_data.csv`  
- `wuzzuf_jobs_data.xlsx`

---

### 2. Data Cleaning
- Removed duplicates.  
- Extracted structured **skills** (split by `·`).  
- Parsed **City** from job location.  
- Classified **Job Level** (Junior / Mid / Senior) using Regex.  

---

### 3. Data Analysis & Visualizations
- **Top 10 In-Demand Skills** (Bar Chart)  
- **Skill WordCloud** (high-frequency keywords)  
- **Job Levels Distribution** (Junior, Mid, Senior)  
- **Top Hiring Companies**  
- **Top Cities with Most Job Listings**
