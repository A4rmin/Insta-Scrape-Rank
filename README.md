# 📸 InstaScrapeRank

> Effortlessly scrape, rank, and analyze image posts from any public Instagram profile — no API keys, no hassle.

---

## ✨ Overview

**InstaScrapeRank** is a beginner-friendly Jupyter Notebook that lets you:
- **Scrape** all image posts from any public Instagram profile
- **Rank** posts by likes
- **Download** top image posts (with captions)
- **Analyze** account performance (average likes, top hashtags, and more)

No API keys, no OAuth — just log in once and go!

---

## 🚀 Features

- ⚡ **No API keys required** (uses [Instaloader](https://instaloader.github.io/))
- 🖼️ **Image-only filtering** (skip videos)
- 📈 **Ranking** by likes
- 💾 **Download** top image posts (images + captions)
- 📊 **Bonus analytics & visualizations**: advanced account summary, hashtag stats, insights, and professional plots
- 📝 **Notebook format**: easy to use, modify, and extend
- 🔧 **Future-ready**: planned script & microservice versions

---

## 🗂️ Project Structure

```
InstaScrapeRank.ipynb      # Main notebook
.env                       # Store your login & target info
/data/
├── raw_<target>_<ts>.json         # All scraped posts
├── processed_<target>_<ts>.json   # Ranked posts
├── summary_<target>_<ts>.json     # Bonus analytics
└── top_posts_<ts>/                # Top-ranked image posts
```

---

## 📊 BONUS: Advanced Analytics & Visualizations

In addition to scraping and ranking, **InstaScrapeRank** provides a professional analytics dashboard:

- 📈 Visualizes engagement trends, posting frequency, and content performance
- 🏆 Reveals best-performing months, days, and post types
- 📝 Analyzes caption length, hashtag usage, and their impact on likes
- 🔮 Offers actionable insights and recommendations for growth
- 🎨 Generates beautiful, modern plots (matplotlib + seaborn)

All analytics are generated automatically in the notebook—no extra setup required!

---

## ⚡ Quickstart

### 1. Install requirements

```bash
pip install instaloader pandas python-dotenv
```

### 2. Log in to Instagram (one-time)

```bash
instaloader --login=your_username
```

This creates a saved session so you don’t need to log in again every time.

### 3. Set up your `.env` file

```
IG_USERNAME=your_instagram_username
IG_TARGET=target_public_profile
```

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
- 🖼️ Downloaded images of top-performing posts
- 📊 Analytics summary: total posts, average likes, hashtag frequency, and more
- 🎨 Professional visualizations and actionable insights (BONUS)

---

## 🛠️ Troubleshooting

- **Login issues?** Make sure your credentials are correct and you’ve run the login command.
- **Target not found?** Double-check the IG_TARGET value in your `.env` file.
- **Missing packages?** Re-run the install command above.

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
- ☕ [Buy me a coffee](https://buymeacoffee.com/your-link) *(replace with your actual link)*
- 🧠 Suggest features or improvements
- 🤝 Contribute! Even a typo fix is appreciated

---

## 📃 License

MIT – free to use, modify, and share.

---

## 🙏 Acknowledgments

Thanks to the amazing [Instaloader](https://instaloader.github.io/) project for making Instagram scraping so much easier.

