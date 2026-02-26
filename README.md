# NowNews

An aggregated news platform with personalized features: favorite articles, read tracking, and comments. Built as a **university project** for Copenhagen Business School (HA(it.)), May 2023—developed in a study group to practice full-stack web development and database integration.

---

## Business Problem

Readers often juggle multiple news sources and lose track of what they’ve read or want to revisit. **NowNews** addresses this by providing a single place to browse aggregated news, save favorites, mark articles as read, and discuss them via comments. The app pulls content into a central database and surfaces it through a simple, session-based web interface so users can manage their reading in one place.

---

## Tech Stack

- **Runtime:** Node.js
- **Framework:** Express.js
- **Templating:** EJS
- **Database:** Azure SQL (via Tedious driver)
- **Auth & sessions:** express-session, bcryptjs
- **Scheduled jobs:** node-cron (e.g. article ingestion, weather updates)
- **HTTP clients:** axios, node-fetch
- **Configuration:** dotenv
- **Testing:** Mocha, Chai

**Architecture:** MVC — Models (Azure SQL/Tedious), Views (EJS), Controllers handling routes for articles, comments, favorites, categories, search, user auth, and weather.

---

## How to Run the Code

1. **Clone the repository** and open a terminal in the project root.

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Configure environment:** Copy `.env.example` to `.env` and fill in your values (Azure SQL connection and any API keys):
   - `DATABASE_URL`, `DB_NAME`, `PASSWORD`, `DATABASE`
   - `API_KEY_AI`, `API_KEY_ORG` (if using those features)

4. **Start the server:**
   ```bash
   node app.js
   ```
   The app runs at **http://localhost:4000**.

---

## Collaborators

Developed in a study group with:

- **Gustav Søgård** — [@gustavsogard](https://github.com/gustavsogard)
- **thel22ab** — [@thel22ab](https://github.com/thel22ab)
- **Troels R.** — [@TroelsPR](https://github.com/TroelsPR)
- **Amanda** — [@Aman3612](https://github.com/Aman3612)

---

*Copenhagen Business School, HA(it.), May 2023.*
