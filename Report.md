
# Report on CORD-19 Metadata Analysis
---

## 🔎 Findings  

1. **Publications by Year**  
   - The dataset spans multiple years, but the majority of publications are concentrated around **2020** (the start of the COVID-19 pandemic).  
   - A sharp increase is observed in 2020 compared to earlier years, confirming the surge of global research output triggered by the outbreak.  

   📊 *Chart: Publications by Year*  

2. **Top Journals**  
   - The **Top 10 journals** with the highest number of papers include well-known biomedical and medical journals.  
   - Journals such as *PLoS One*, *bioRxiv*, *int J Environ Res Public Health*, and *BMJ* appear among the most frequent publishers.  
   - This reflects the role of both traditional academic journals and medical publishers in disseminating COVID-19-related findings.  

   📊 *Chart: Top 10 Journals Publishing COVID-19 Research*  

3. **Word Frequency in Titles**  
   - The **Word Cloud of paper titles** shows frequent words such as *COVID-19*, *SARS-CoV-2*, *infection*, *disease*, *coronavirus*, and *health*.  
   - This highlights the main themes and focus areas of the research during the pandemic.  

   ☁️ *Visualization: Most Frequent Words in Titles*  

4. **Top Publication Sources**  
   - By analyzing `source_x`, the most common sources include **bWHO**, **meldine;PMC**, and **meldine**.
  
   📊 *Chart: Top 10 Sources*  

---

## 🛠 Challenges  

1. **Large Dataset**  
   - The `metadata.csv` file was very large (hundreds of thousands of rows).  
   - Required filtering and careful selection of columns to keep processing efficient.  

2. **Missing & Inconsistent Data**  
   - Many records had missing `journal`, `abstract`, or `publish_time` values.  
   - The `doi` field was inconsistent or absent for several entries, limiting traceability of papers.  

3. **Pandas Warnings**  
   - Encountered `SettingWithCopyWarning` when transforming columns (`publish_time`, `year`, `abstract_word_count`).  
   - Fixed using `.loc[]` to safely assign values to DataFrame subsets.  

4. **Visualization Libraries**  
   - The project required installation of extra libraries like **WordCloud**, which was not included by default.  
   - Alternative approaches (e.g., `Counter` + bar plots) can be used if WordCloud is unavailable.  

---

## 📚 Learning & Skills Gained  

1. **Pandas for Data Cleaning**  
   - Learned to manage missing values with `dropna()` and `fillna()`.  
   - Converted date strings into datetime objects and extracted `year`.  
   - Created derived metrics like `abstract_word_count`.  

2. **Data Visualization**  
   - Used **Matplotlib** and **Seaborn** to create bar plots for trends and journal counts.  
   - Built a **Word Cloud** to visualize the most frequent keywords in research titles.  

3. **Working with Real-World Datasets**  
   - Understood the challenges of cleaning and analyzing **large, messy datasets**.  
   - Experienced how preprint repositories (*bioRxiv*, *medRxiv*) influenced COVID-19 research dissemination.  

4. **Critical Analysis**  
   - Translated raw dataset trends into meaningful insights about scientific response to COVID-19.  

---

## ✅ Reflection  

This project provided hands-on experience with **data cleaning, visualization, and exploratory data analysis** using a globally important dataset.  

- The **surge of publications in 2020** clearly demonstrates how the scientific community rapidly mobilized in response to COVID-19.  
- The presence of preprint servers in the top sources highlighted how urgent findings were prioritized over traditional peer-review timelines.  
- Despite challenges with missing data and large file size, pandas and visualization tools proved effective in uncovering insights.  

Overall, this project strengthened my ability to **handle real-world data, apply data science tools, and derive insights that connect data to real events**.  
