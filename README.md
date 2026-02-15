
# 🛰️ Russia-Ukraine Conflict: Data Pipeline Project

This project demonstrates a complete **ETL (Extract, Transform, Load)** pipeline built using **KoboToolbox**, **Python**, **PostgreSQL**, and **Power BI** (optional). It extracts real-time data about the Russia-Ukraine conflict, cleans and transforms it using Python, and loads it into a PostgreSQL database for further analysis.

---

## 📌 Project Overview

The pipeline performs the following:

1. **Extract** data from KoboToolbox (CSV endpoint).
2. **Transform** the data using `pandas`:
   - Rename columns for consistency.
   - Calculate total casualties.
   - Parse and convert date formats.
3. **Load** the cleaned data into a PostgreSQL database.
4. *(Optional)* Use **Power BI or Tableau** for reporting and visualization.

---

## 📂 Project Structure

```bash
Russia-Ukraine-Conflict/
├── .env                     # Stores environment variables
├── .gitignore               # Git exclusions
├── pipeline.py              # Python script for the ETL pipeline
├── README.md                # Project overview and setup guide
├── requirements.txt         # Required Python libraries
````

---

## ⚙️ Technologies Used

* **Python 3.10+**
* **Pandas** – data cleaning
* **Requests** – data fetching
* **psycopg2** – PostgreSQL connection
* **PostgreSQL** – database
* **KoboToolbox** – data source
* **python-dotenv** – environment variable management

---

## 🔐 Environment Variables

Create a `.env` file in the root directory with the following structure:

```ini
KOBO_USERNAME=your_kobo_username
KOBO_PASSWORD=your_kobo_password
PG_HOST=your_postgres_host
PG_DATABASE=your_database_name
PG_USER=your_postgres_user
PG_PASSWORD=your_postgres_password
PG_PORT=5432
```

---

## 🚀 How to Run the Pipeline

1. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

2. Add your `.env` file with credentials as shown above.

3. Run the script:

   ```bash
   python pipeline.py
   ```

---

## 🧠 Key Metrics Calculated

* **Total Casualties** = Casualties + Injured + Captured
* Dates converted for time-based analysis
* Cleaned and standardized column names

---

## 📊 Dashboard

Connect the PostgreSQL database to **Power BI** to build an interactive dashboard showing:

* Total casualties over time
* Casualties by region
* Combat intensity heatmaps
* Occupied territories distribution
---

## 🤝 Contributing

If you'd like to suggest improvements or contribute, feel free to fork the repository and open a pull request.

---

## 📜 License

This project is open-source and available under the **MIT License**.

---

## 🙌 Acknowledgments

* **KoboToolbox** – for making humanitarian data collection simple
* All open-source developers whose tools made this project possible

---

## 📽️ Project By

**Michael Fongwe Tebug**

```


