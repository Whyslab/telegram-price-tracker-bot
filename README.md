# 🤖 Telegram Price & Content Tracker Bot

![Python](https://img.shields.io/badge/Python-3.9%2B-blue?style=flat-square&logo=python)
![Aiogram](https://img.shields.io/badge/Aiogram-3.x-blue?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)

An asynchronous Telegram bot that monitors webpages for price changes, restocks, or content updates and instantly notifies you via Telegram.

Perfect for tracking product prices, marketplace deals, competitor pricing, limited releases, or any website that changes over time.

---

## 🚀 Features

- ⚡ **Asynchronous Monitoring** — Fast, non-blocking requests powered by `httpx`.
- 🎯 **CSS Selector Support** — Monitor any specific HTML element using CSS selectors.
- 🔔 **Instant Telegram Notifications** — Receive alerts immediately after a detected change.
- 📄 **HTML Parsing** — Powered by `BeautifulSoup4` for reliable extraction.
- 🛡️ **Robust Error Handling** — Automatically recovers from temporary network failures.
- 🔄 **Continuous Monitoring** — Runs 24/7 with configurable polling intervals.
- 🐳 **VPS Friendly** — Uses less than 30 MB RAM, making it ideal for inexpensive VPS hosting.
- ⚙️ **Easy Configuration** — Simply edit a few variables to monitor a new website.

---

## 🛠️ Tech Stack

- Python 3.9+
- Aiogram 3.x
- httpx
- BeautifulSoup4

---

## 📦 Installation

Clone the repository:

```bash
git clone https://github.com/Whyslab/telegram-tracker-bot.git
cd telegram-tracker-bot
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ⚙️ Configuration

1. Create a Telegram bot using **@BotFather** and copy the bot token.

2. Obtain your Telegram **Chat ID** using **@userinfobot**.

3. Open `bot.py` and configure the following variables:

```python
BOT_TOKEN = "your_bot_token"
CHAT_ID = 123456789
TARGET_URL = "https://example.com/product"
CSS_SELECTOR = ".current-price"
```

---

## ▶️ Run

```bash
python bot.py
```

The bot will continuously monitor the selected element and send a Telegram notification whenever its content changes.

---

## 💡 JavaScript-Based Websites

Some websites built with React, Vue, Angular, or other JavaScript frameworks don't return the final HTML when requested through `httpx`.

In those cases, replace the HTTP client with **Playwright** (or another headless browser) to render the page before extracting the target element.

---

## 📂 Example Use Cases

- 💰 Price tracking
- 📦 Product restock notifications
- 🎟️ Ticket availability monitoring
- 📰 Website content updates
- 🏪 Marketplace listings
- 📈 Competitor price monitoring
- 🚀 Limited product drops

---

## 📄 License

This project is released under the **MIT License**.

You are free to use, modify, and distribute it for personal or commercial purposes.

---

## ⭐ Support

If you find this project useful, consider giving it a ⭐ on GitHub.

Contributions, issues, and feature requests are always welcome.
