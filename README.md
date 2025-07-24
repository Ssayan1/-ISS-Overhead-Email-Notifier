# 🌍 ISS Overhead Email Notifier

A simple Python script that sends you an **email alert** when the **International Space Station (ISS)** is flying over your location **at night**!

## ✨ Features

- Checks ISS location every 60 seconds
- Sends an email when it's above your city
- Only alerts at night using the [sunrise-sunset API](https://sunrise-sunset.org/api)

---

## ⚙️ Requirements

- Python 3.x
- Internet access
- Gmail account with **App Passwords** enabled

---
## ✅ Step 1: Project Structure

Organize your project like this:

```bash
📁 iss-email-notifier/
├── main.py           # Your ISS email notifier script
├── README.md         # Project description
├── .gitignore        # To ignore cache files, credentials
```
## 📌 How it works

- Uses [Open Notify API](http://open-notify.org/) to track ISS position
- Uses [Sunrise-Sunset API](https://sunrise-sunset.org/api) to check night time
- Sends email via Gmail SMTP when both conditions are true

---
## ✅ Step 2: Save Your Script

Filename: main.py
### Suggested Safe Change:
```bash
MY_EMAIL = "your_email@gmail.com"
MY_PASSWORD = "your_app_password"  # Use environment variables for security
```
Later, you can load them using:
```bash
import os
MY_EMAIL = os.getenv("MY_EMAIL")
MY_PASSWORD = os.getenv("MY_PASSWORD")
```
## ✅ Step 3: Create .gitignore

In the same folder, create a .gitignore file:
```bash
__pycache__/
*.pyc
.env
```
## 🛠 Setup
1. Clone the repo:
 ```bash
   git clone https://github.com/yourusername/iss-email-notifier.git
   cd iss-email-notifier
```
2. Install dependencies:
```bash
pip install requests
```
4. Edit main.py and add your:
- Gmail address
- App password
- Latitude and Longitude

## 🚀 Run the Script
```bash
python main.py
```






