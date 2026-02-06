Features

Fetches channel-level and video-level statistics using YouTube Data API

Processes data using Pandas

Stores structured data in CSV / SQLite

Handles API errors and missing values gracefully

Designed with scalability in mind for future cloud integration

🛠️ Tech Stack

Python 3

YouTube Data API v3

Pandas

Requests

SQLite (current storage)

Snowflake (planned integration)

🧠 Challenges Faced

Handling empty or inconsistent API responses

Managing API limits and timeouts

Deciding between cloud (Snowflake) vs local storage due to auth constraints

Ensuring clean, reusable pipeline logic

🔮 Future Enhancements

Snowflake / BigQuery integration

Automated data refresh using schedulers

Dashboard creation (Tableau / Power BI)

Multi-channel comparison

Sentiment analysis on comments

📂 Must-Have Files for GitHub (Highly Recommended)
1️⃣ requirements.txt
pandas
requests
python-dotenv

2️⃣ .gitignore
__pycache__/
*.env
*.csv
*.db
.vscode/

3️⃣ run_pipeline.py
from scripts.fetch_youtube_data import fetch_youtube_data

if __name__ == "__main__":
    fetch_youtube_data()

4️⃣ .env (DO NOT COMMIT)
YOUTUBE_API_KEY=your_api_key_here
CHANNEL_ID=channel_id_here

5️⃣ exploratory_analysis.ipynb (Optional but Powerful)

Top videos by views

Like-to-view ratio

Upload frequency trend

Recruiters love seeing analysis notebooks.

6️⃣ PROJECT_NOTES.md (🔥 underrated but impressive)
  Project Learnings
- API-based data ingestion
- Debugging real-world data issues
- Designing flexible pipelines
- Making tool trade-offs under constraints
