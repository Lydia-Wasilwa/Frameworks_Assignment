# 📊 CORD-19 Metadata Analysis  

This project analyzes the **CORD-19 dataset (metadata.csv)** to uncover publication trends, top journals, and research patterns during the COVID-19 pandemic.  

## 📂 Project Structure  
Frameworks-Assignment/
│── app.py # Streamlit app for interactive exploration
│── data_analysis.ipynb # Jupyter notebook with analysis & visualizations
│── README.md # Project overview (this file)
│── report.md # Detailed report (findings + reflection)
│── app.py # Streamlit Application 
│── .gitignore # Ignore large files (like metadata.csv)


⚠️ **Note:** The dataset (`metadata.csv`) is **not included** in this repo because it exceeds GitHub’s 100MB limit.  
You can download it directly from https://www.kaggle.com/datasets/allen-institute-for-ai/CORD-19-research-challenge?select=metadata.csv

## 🚀 How to Run  

### Clone the Repository  
```bash
git clone https://github.com/Lydia-Wasilwa/Frameworks_Assignment.git
cd Frameworks_Assignment

```
## Install dependencies
```bash
pip install pandas matplotlib seaborn streamlit wordcloud

```
## Add the Dataset
Download metadata.csv from Kaggle and place it in the project root folder.

## Run the Notebook
```bash
jupyter notebook data_analysis.ipynb

```

## Launch the Streamlit App
```bash
streamlit run app.py
```
