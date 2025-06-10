# 📸 InstaScrapeRank

Effortlessly scrape, rank, and analyze image posts from any public Instagram profile — no API keys, no hassle.

---

## ✨ Overview

**InstaScrapeRank** is a Jupyter Notebook and helper script that lets you:
- **Scrape** all image posts from any public Instagram profile
- **Rank** posts by likes
- **Download** top image posts (with captions)
- **Analyze** account performance (average likes, top hashtags, and more)
- **Visualize** trends and get actionable insights

No API keys, no OAuth — just a one-time login using your browser session or Instaloader's built-in login.

---

## 🚀 Features

- ⚡ **No API keys required** (uses [Instaloader](https://instaloader.github.io/))
- 🦊 **Firefox session import**: Use your existing Firefox Instagram login with `login.py` (no password needed)
- 🖼️ **Image-only filtering** (skip videos)
- 📈 **Ranking** by likes
- 💾 **Download** top image posts (images + captions)
- 📊 **Bonus analytics & visualizations**: advanced account summary, hashtag stats, insights, and professional plots
- 📝 **Notebook format**: easy to use, modify, and extend
- 🔧 **Future-ready**: planned script & microservice versions

---

## 🗂️ Project Structure

```
InstaScrapeRank.ipynb      # Main notebook (full workflow & analytics)
login.py                   # Helper: import Firefox Instagram session
.env                       # Store your login & target info
requirements.txt           # All dependencies
/data/
├── raw_<target>_<ts>.json         # All scraped posts
├── processed_<target>_<ts>.json   # Ranked posts
└── top_posts_<ts>/                # Top-ranked image posts (images + captions)
```

---

## 🔐 Login & Session Management

You have two ways to authenticate:

### 1. Instaloader's Built-in Login (Simple)
- Run: `instaloader --login=your_username`
- This creates a saved session file for future use.

### 2. Firefox Session Import (No Password Needed)
- Log in to Instagram in Firefox (stay logged in).
- Run: `python login.py -u your_username`
- This script finds your Firefox cookies and creates a session file for Instaloader.
- Useful if you have 2FA or want to avoid entering your password in the terminal.

> **Tip:** The notebook loads your session automatically if you use either method.

---

## ⚡ Quickstart

### 1. Install requirements

```zsh
pip install -r requirements.txt
```

### 2. Set up your `.env` file

```
IG_USERNAME=your_instagram_username
IG_TARGET=target_public_profile
```

### 3. Log in (choose one method)
- **Option A:** `instaloader --login=your_username`
- **Option B:** `python login.py -u your_username`

### 4. Run the notebook

Open `InstaScrapeRank.ipynb` and run the cells in order. The notebook will:
- Scrape all image posts
- Save raw and processed data
- Rank posts by likes
- Download top X image posts
- Provide a summary, analytics, and bonus visualizations

---

## 📂 Output Overview

- 📄 JSON files for raw and ranked data
- 🖼️ Downloaded images of top-performing posts (with captions)
- 📊 Analytics summary: total posts, average likes, hashtag frequency, and more
- 🎨 Professional visualizations and actionable insights (BONUS)

---

## 📊 Advanced Analytics & Visualizations

**InstaScrapeRank** provides a professional analytics dashboard:

- 📈 Visualizes engagement trends, posting frequency, and content performance
- 🏆 Reveals best-performing months, days, and post types
- 📝 Analyzes caption length, hashtag usage, and their impact on likes
- 🔮 Offers actionable insights and recommendations for growth
- 🎨 Generates beautiful, modern plots (matplotlib + seaborn)

All analytics are generated automatically in the notebook—no extra setup required!

---

## 🛠️ Troubleshooting

- **Login issues?**
  - If using Instaloader login: make sure your credentials are correct and you’ve run the login command.
  - If using Firefox session: ensure you are logged in to Instagram in Firefox and run `python login.py -u your_username`.
- **Target not found?** Double-check the IG_TARGET value in your `.env` file.
- **Missing packages?** Re-run the install command above.
- **Session not loading?** Delete old session files and re-run the login step.

---

## 💡 Future Plans

- 🐍 Python script version
- ☁️ Microservice/API
- ⌨️ CLI support
- 📈 Visual dashboards, Excel export
- 🔍 Filtering by date or hashtags

---

## 🤝 Contributing

Contributions, feedback, and feature requests are welcome! Feel free to open an issue or submit a pull request.

---

## 💖 Like It? Show Some Love!

- 🌟 Star the repo
- ☕ [Buy me a coffee](https://www.coffeebede.com/a4rmin)
- 🧠 Suggest features or improvements
- 🤝 Contribute! Even a typo fix is appreciated

---

## 📃 License

MIT – free to use, modify, and share.

---

## 🙏 Acknowledgments

Thanks to the amazing [Instaloader](https://instaloader.github.io/) project for making Instagram scraping so much easier.

Special thanks to the open-source community for tools like pandas, matplotlib, seaborn, and Jupyter.

