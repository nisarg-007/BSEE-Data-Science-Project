🛢️ BSEE Offshore Well Analysis: Deep Dive into the Gulf
From Dynamic Web Scraping to Data-Driven Strategy > A Data Science Capstone Project at the University of Houston

📖 The Story Behind the Data
Living in Houston, the energy capital of the world, my team and I didn't want to just analyze a clean, pre-packaged dataset from Kaggle. We wanted to understand the real heartbeat of the industry: Offshore Drilling.

We targeted the Bureau of Safety and Environmental Enforcement (BSEE). The challenge? The data wasn't just sitting in a CSV. It was locked behind a dynamic ASP.NET portal.

This repository documents our full journey: from building a custom Selenium scraper to handle dynamic pagination, to extracting 20,000+ well records, and finally performing deep EDA to uncover trends in drilling speed and technology.

📂 Repository Contents
Team_9_Midterm_project.ipynb 🧠

The core brain of the project. Contains the custom scraping script (Selenium/BeautifulSoup), data cleaning pipeline, EDA, and all visualization code.

bsee_well_data.csv 💾

The "gold" we mined. A cleaned dataset of ~20,000 offshore wells including Spud Dates, Water Depths, Company Names, and Status codes.

project report week 1,2,3.pdf 📄

Our detailed weekly logs, outlining the project management aspect, challenges faced, and the strategic milestones achieved by the team.

💡 Key Insights Uncovered
1. Speed is Everything ⏱️
One of our biggest surprises was operational efficiency. The data revealed that over 70% of offshore wells are drilled and completed in just over a month. The industry doesn't waste time.

2. The Shift to Directional Drilling ↘️
By analyzing the difference between Measured Depth (MD) and True Vertical Depth (TVD), we visualized the industry's technological shift.

Zero Difference: Vertical Well (Old School).

Large Difference: Directional/Horizontal Well (Modern Tech).

Verdict: We found massive deviations, proving the widespread adoption of complex directional drilling to reach reservoirs miles away from the platform.

3. The Deepwater Frontier 🌊
We identified a distinct cluster of high-tech wells pushing past 1,000ft water depth, separating the "legacy" shallow-water operations from the modern "deepwater frontier."

🛠️ Tech Stack & Methodology
This wasn't just analysis; it was engineering.

Data Acquisition (The Hard Part):

Tools: Python, Selenium, BeautifulSoup.

Method: We automated a browser to navigate the BSEE ASP.NET portal, handle post-back events, and scrape data page-by-page.

Data Cleaning:

Tools: Pandas, NumPy.

Process: Handled missing values, converted dates, and engineered features like Drilling Duration and Depth Difference.

Visualization:

Tools: Matplotlib, Seaborn.

Outputs: Correlation heatmaps, geospatial (lat/long) scatter plots, and distribution histograms.

👥 The Team (Group 9)
This project was a collaborative effort under the guidance of Prof. Narges Debary for the Intro to Data Science course at the University of Houston.

Nisarg Shah (Team Manager): Web Scraping Lead & Architecture.

Omkar Koli: Data Visualization Specialist.

Parva Shah: Data Mining & Pattern Discovery.

Praveen Kumar G: Exploratory Data Analysis (EDA) & Wrangling.

Nithin Lingala: Exploratory Data Analysis (EDA) & Wrangling.

🚀 How to Run the Code
Clone this repo.

Install dependencies:

Bash

pip install pandas numpy seaborn matplotlib selenium beautifulsoup4
Note on Scraping: The scraping portion of the notebook requires a compatible chromedriver installed for your version of Chrome.

Run Team_9_Midterm_project.ipynb in Jupyter Lab or Google Colab.
