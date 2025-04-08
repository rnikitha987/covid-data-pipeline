**🦠 COVID-19 Data Pipeline**

This project pulls real-time COVID-19 data from the [disease.sh API](https://disease.sh/docs/), cleans it using Python and Pandas, and visualizes the top 10 countries by total cases.

**📌 Features**
- Fetches live COVID-19 data from an open API
- Cleans and transforms data with Pandas
- Converts timestamps to readable format
- Creates a bar chart for visualization
- Saves output as a downloadable CSV

**🛠 Tech Stack**
- Python (Requests, Pandas, Matplotlib)
- Google Colab

**📊 Visualization**
top_10 = df_clean.sort_values(by='cases', ascending=False).head(10)

plt.figure(figsize=(10,6))
plt.bar(top_10['country'], top_10['cases'])
plt.xticks(rotation=45)
plt.title("Top 10 Countries by COVID-19 Cases")
plt.ylabel("Total Cases")
plt.tight_layout()
plt.show()


🚀** How to Run**
1. Open the project in Google Colab
2. Run each cell step by step
3. Download the CSV file if needed

** 📁 Data Source**
[disease.sh COVID-19 API](https://disease.sh/docs/)

💡 Future Ideas
- Store data in a cloud database like AWS S3 or SQLite
- Schedule automatic runs using Airflow or cron
- Create a dashboard using Power BI or Tableau

** 🙋‍♀️ Author**
Nikitha R

