
# 📺 YouTube Data Harvesting and Visualization

This project focuses on harvesting data from YouTube using the YouTube Data API, storing it in a NoSQL database (MongoDB), migrating it to a structured SQL database (PostgreSQL), and finally visualizing the data using Streamlit.

---

## 🚀 Features

- 🔍 Fetch detailed data from YouTube channels and videos using the YouTube Data API
- 🗃️ Store raw JSON data in **MongoDB**
- 🔄 Transform and migrate structured data to **PostgreSQL**
- 📊 Visualize key metrics and insights in an interactive **Streamlit** dashboard

---

## 📌 Tech Stack

| Component        | Technology         |
|------------------|--------------------|
| Data Source      | YouTube Data API v3 |
| NoSQL Database   | MongoDB            |
| SQL Database     | PostgreSQL         |
| Backend          | Python (pymongo, psycopg2/SQLAlchemy) |
| Frontend / UI    | Streamlit          |

---

## 🧱 Project Structure

```
youtube-data-harvesting/
├── api/                      # YouTube API scripts
│   └── fetch_data.py
├── mongo/                    # MongoDB storage scripts
│   └── store_to_mongo.py
├── postgres/                 # PostgreSQL migration scripts
│   └── migrate_to_postgres.py
├── streamlit_app/            # Streamlit dashboard
│   └── app.py
├── utils/                    # Utility/helper functions
├── requirements.txt
└── README.md
```

---

## 📥 Data Collected

- **Channel Information**
  - Channel ID, Name, Subscribers, Description, etc.

- **Video Details**
  - Video ID, Title, Description, Published Date, Views, Likes, Comments Count

- **(Optional) Comments**
  - Author, Text, Published Time

---

## 📈 Dashboard Features

- Select channels and filter by upload date or views
- View top 10 videos by views or likes
- Visualize video publishing trends over time
- Interactive table with all video details
- Optional: Word cloud of comments (if enabled)

---

## 🛠️ Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/youtube-data-harvesting.git
   cd youtube-data-harvesting
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure API Keys and DB Connections**
   - Add your YouTube API key in `fetch_data.py`
   - Configure MongoDB URI and PostgreSQL credentials in `.env` or config files

4. **Run the data pipeline**
   ```bash
   python api/fetch_data.py
   python mongo/store_to_mongo.py
   python postgres/migrate_to_postgres.py
   ```

5. **Launch Streamlit app**
   ```bash
   streamlit run streamlit_app/app.py
   ```

---

## 📌 Future Improvements

- Add automatic scheduling using cron/APS
- Include sentiment analysis for comments
- Add user authentication for dashboard access
- Export data as CSV/Excel from dashboard

---

## 🤝 Contributions

Pull requests are welcome! If you find a bug or want to suggest an enhancement, feel free to open an issue.

---
