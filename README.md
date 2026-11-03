# telegram-to-gdrive
An interactive Google Colab tool to download Telegram files directly to Google Drive with live speed, ETA, and auto-organization.
# 📥 Telegram to Google Drive — Interactive Downloader

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]([YOUR_COLAB_LINK_HERE](https://colab.research.google.com/drive/1ZL4un43heVoqIWDYnK542d6epVJ8DS0H))

An automated, interactive tool built for Google Colab that lets you download files, videos, and albums from Telegram (public, private, or forum topics) directly into your Google Drive.

> 🤖 **Credits:** The code, UI, and architecture for this project were written and engineered in collaboration with **DeepSeek AI**.

## ✨ Features
- **📂 Auto-Organized:** Automatically saves files into subfolders named `Sender Name - YYYY-MM-DD` to keep your Drive clean.
- **⚡ Live Speedometer & ETA:** Real-time download/copy speeds, time elapsed, and estimated time remaining for every file.
- **✅ Interactive Selection:** Fetch a Telegram album, preview the files, uncheck the ones you don't want, and upload the rest.
- **🛡️ Auto-Resume:** If your Colab session disconnects, it compares file sizes and skips files already in your Drive.
- **📊 Live Dashboard:** A real-time dashboard (updates every 3 seconds) showing your total files, storage used, and recent download history.
- **🔐 Secure Session Reuse:** Saves your Telegram session safely inside your own Google Drive, so you only log in once.

---

## 🚀 How to Use

### 1. Prerequisites
- A Telegram account.
- A Google Drive account (Free tier gives 15GB).
- Telegram `API ID` and `API Hash`.

### 2. Getting Telegram API Credentials
1. Go to [my.telegram.org](https://my.telegram.org) and log in with your phone number.
2. Click on **API development tools**.
3. Fill out the form (any name/platform works) and click **Create application**.
4. Copy your **App api_id** and **App api_hash**.

### 3. Running the Notebook
1. Click the **Open in Colab** badge at the top of this page.
2. Run **⚙️ Step 0 (Setup)** to install dependencies and mount your Drive.
3. Run **🔧 Step 1 (Backend)** to initialize the background logic.
4. Run **🔑 Step 2 (Connect)**. Paste your API ID, API Hash, and phone number. Enter the login code sent to your Telegram app.
5. Run **📤 Step 3 (Upload)**. Paste a Telegram link, click **Fetch & Preview**, select your files, and click **Upload**!
6. Run **📊 Step 4 (Dashboard)** to see a live view of your files.

---

## ⚠️ Important Disclaimers & Limits
* **Google Drive Quota:** The free tier of Google Drive is limited to **15 GB**. If you hit this limit, file transfers will fail.
* **Google Colab ToS:** Colab is designed for interactive coding, not as a 24/7 bulk file-transfer server. Avoid downloading massive amounts of data in a single run to prevent your session from being flagged.
* **Private Groups:** To download from a private group or channel, your Telegram account **must** already be a member of that group.
* **Copyright:** This tool is intended for personal backups. Do not use it to mass-mirror copyrighted material. Use responsibly.

---

## 🛠️ Built With
- [Telethon](https://github.com/LonamiWebs/Telethon) — Pure Python 3 MTProto library.
- [ipywidgets](https://ipywidgets.readthedocs.io/) — Interactive HTML widgets.
- [Google Colab API](https://research.google.com/colaboratory/) — For mounting Google Drive.

## 📝 License
This project is licensed under the MIT License - feel free to use, modify, and distribute it.
