# 🚀 SpaceX Launch Dashboard

An interactive and data-rich dashboard that visualizes **SpaceX's mission history** using Plotly Dash. From launch sites and payloads to mission outcomes and booster performance — this dashboard is your personal launch control center! 🛰️📊

---

## App Link

🔗 Visit the deployed app:  
**[https://spacex-falcon-9.onrender.com](https://spacex-falcon-9.onrender.com/)** 

## 🌟 Features

✨ **Dynamic Dropdown** — Select any launch site or view all launches at once.  
📈 **Success Rate Pie Chart** — Instantly compare success vs. failure by site.  
🎯 **Payload Range Slider** — Filter launches based on payload weight in kilograms.  
🚀 **Scatter Plot** — Understand how payload and booster version affect launch success.  
⚡ **Fast & Responsive** — Powered by Plotly Dash, works beautifully in your browser.

---

## 🧠 What You'll Learn

- Which launch site has the **highest success rate**?
- Does **payload size** affect mission success?
- How do **booster versions** compare in performance?
- Are SpaceX launches consistent over time?

All answers are just a few clicks away.

---

## 📁 Dataset Overview

The dashboard is powered by the `spacex_launch_geo.csv` dataset, which includes:

| Column Name           | Description |
|-----------------------|-------------|
| `Flight Number`       | Sequential ID for each launch |
| `Date` + `Time (UTC)` | Launch datetime in UTC |
| `Booster Version`     | Type and ID of the booster (e.g., F9 v1.1 B1003) |
| `Launch Site`         | Launch location (e.g., CCAFS LC-40) |
| `Payload Mass (kg)`   | Mass of the payload |
| `Orbit`               | Orbit type (e.g., LEO, GTO) |
| `Customer`            | Organization requesting the launch |
| `Mission Outcome`     | Human-readable outcome of the mission |
| `Landing Outcome`     | Booster landing status |
| `class`               | 1 for success, 0 for failure (used for modeling)

---

## 🚀 Try It Yourself (Locally)

### 1. Clone this repo
```bash
git clone https://github.com/yourusername/spacex-dash-app.git
cd spacex-dash-app
