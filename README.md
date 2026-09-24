# 🦈 SHARKFLIX — From Data to Screen

> **"Two countries. Some of the world's most beautiful beaches. And thousands of shark attacks."**

---

## 🎬 Project Overview & Premise

**SHARKFLIX** is a data-driven documentary series concept designed as a high-octane pitch for global streaming platforms. Created by **Blue Fang Studios**, this project bridges data science and investigative media production by transforming raw global shark attack archives into a compelling 7-episode true-crime style narrative structure.

While marine biologists agree that sharks generally avoid humans, thousands of attacks have been recorded over the last 25 years. SHARKFLIX investigates the environmental triggers, human activity factors, and localized anomalies behind these dangerous encounters—proving that behind every statistic is a human story.

---

## 🛠️ Data Pipeline & Methodology

Using Python and the Pandas library, we processed decades of unrefined data from the Global Shark Attack File to extract meaningful patterns, seasonal trends, and geographic hotspots.

```
 RAW DATA  ──>  CLEAN  ──>  GROUP  ──>  ANALYSE  ──>  PATTERNS  ──>  STORY
```

### Core Data Cleaning Steps:
1. **Data Cleaning & Filtering:** Handled missing/null values across key fields (`Fatal (Y/N)`, `Location`, `Date`, `Activity`).
2. **Standardization:** Normalized messy strings in state/country columns and formatted temporal data.
3. **Aggregation & Grouping:** Grouped incidents by geography, year, time of day, and severity using Pandas methods such as `df.groupby()` and `value_counts()`.
4. **Export:** Exported the cleaned, ready-to-analyze dataset into `sharkflix_clean.csv`.

---

## 📊 Key Findings & Dangerous Figures

* **The Global Scale:** **~3,000 recorded cases** and **100+ fatalities** analyzed over the last 25 years.
* **The 80%+ Rule:** Over 80% of all recorded incidents in the dataset occur across two primary countries: **USA** and **Australia**.
* **Overall Trend:** Annual reported incidents peaked in **2015 (76 cases)** and showed a decrease toward recent years (**19 recorded cases**). However, human risk and severity remain critical.
* **Volume vs. Fatality Paradox:**
  * **Most Volume:** Florida, USA (**699 attacks**) leads in sheer number of incidents, followed by New South Wales, AUS (**191**) and Hawaii, USA (**178**).
  * **Most Fatal:** Western Australia exhibits a staggering **15.9% fatality rate per attack**.
  * *Key Insight:* **The place with the most attacks isn't necessarily the most fatal.**
* **The 2020 Pandemic Anomaly:** Despite a sharp decline in beachgoers during global lockdowns, 2020 experienced an unexpected spike in human fatalities, serving as the focal point for Episode 7.

---

## 📁 Repository Structure

```
data-cleaning-pandas/
├── shark_attack.ipynb        # Main Jupyter Notebook containing all data cleaning & analysis code
├── sharkflix_clean.csv       # Cleaned dataset exported from the notebook
└── README.md                 # Project documentation and presentation link
```

---

## 🚀 How to Run the Code

### Prerequisites
You only need **Python 3**, **Pandas**, and either **VS Code** (with the Jupyter extension) or **Jupyter Notebook** installed.

### Step 1: Clone the Repository
Clone this repo to your local machine using terminal or git:
```bash
git clone https://github.com/YOUR_USERNAME/data-cleaning-pandas.git
```

### Step 2: Open in VS Code or Jupyter Notebook
* **If using VS Code:**
  1. Open VS Code.
  2. Go to `File > Open Folder...` and select the cloned `data-cleaning-pandas` folder.
  3. Open `shark_attack.ipynb`.
  4. Ensure your Python kernel is selected and run the cells sequentially!

* **If using Jupyter Notebook:**
  1. Open your terminal/command prompt.
  2. Navigate to the folder: `cd data-cleaning-pandas`
  3. Launch Jupyter: `jupyter notebook`
  4. Click on `shark_attack.ipynb` in your browser and run the cells.

*Note: The notebook reads `sharkflix_clean.csv` directly from the same root folder, so no file paths need to be changed.*

---

## 🧰 Technologies Used

* **Language:** Python 3
* **Data Manipulation:** Pandas
* **Environment / Tools:** Jupyter Notebook / Visual Studio Code (VS Code)

---

## 🔗 Presentation Slides

📺 **Presentation Deck (SharkFlix_Project_Unit2):**  
👉 [**Click Here to View Google Slides Presentation**](https://docs.google.com/presentation/d/YOUR_GOOGLE_SLIDES_SHARE_LINK_HERE/edit?usp=sharing)

*(Note: Ensure your Google Slides sharing settings are set to "Anyone with the link can view")*

---

## 👥 Team & Authors — Blue Fang Studios

* **Presenter 1:** Creative & Narrative Lead
* **Presenter 2:** Data & Analytics Lead
* **Presenter 3:** Production & Showrunner

*Produced for the Data Analytics Project Presentation.*