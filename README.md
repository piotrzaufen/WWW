# 🔐 Signal Bot Prototype

This project contains an early-stage prototype of a Signal bot for interacting with groups, sending auto-responses, and performing basic moderation tasks.

> ⚠️ **Note:** This is not a production-ready implementation. The code here is for experimental and research purposes only.

---

## 🚀 Features

- Automated message handling
- Keyword-based auto-responses
- Basic anti-spam detection (frequency + keyword patterns)
- User join/leave logging
- Scheduled message posting (via cron)

---

## 🧰 Technologies Used

- Python 3.10
- signal-cli (Signal command-line interface wrapper)
- `subprocess` & `re` for system-level automation
- SQLite for lightweight storage
- Cron for task scheduling

---

## 🗂️ Structure
signal-bot/ ├── bot.py ├── config/ │ └── settings.yaml ├── scripts/ │ └── install_signal_cli.sh ├── data/ │ └── group_ids.db ├── logs/ │ └── bot.log ├── media/ │ ├── banner.png │ ├── screenshot1.png │ └── signal_debug_photos/ │ ├── img1.jpg │ ├── img2.jpg │ └── img3.jpg └── README.md


---

## ⚙️ Setup

1. Install dependencies
   ```bash
   pip install -r requirements.txt

2. Install signal-cli (Linux/macOS):
./scripts/install_signal_cli.sh

3. Configure your account:
   Edit config/settings.yaml with your Signal phone number and target group ID.

4. python bot.py
