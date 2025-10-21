# 📡 NetPulse – PRTG Alerts & Visual Daily Report for Telegram

<p align="center">
  <img src="https://i.ibb.co/7tp8mpP2/Gemini-Generated-Image-ia4eiuia4eiuia4e.png" alt="NetPulse Banner" width="200" height="200">
</p>

*Illustrative diagram of workflow (replace with your own screenshot if desired)*

**NetPulse** is an **n8n workflow** to **receive PRTG alerts in real-time**, track downtime, and send a **visual daily/weekly report to Telegram**.

---

## 🌟 Features

| Feature | Description |
|---------|-------------|
| 🔔 Real-time Alerts | Color-coded messages with Emojis for outage severity: ✅ Green < 1 min, ⚠️ Yellow < 3 min, 🔴 Red ≥ 5 min |
| 📊 Downtime Tracking | All outages stored in **Global Data Store** |
| 📝 Outage Reason | Outage reason included for each sensor |
| 📆 Daily/Weekly Reports | Emoji-based visual charts and downtime summary |
| 📈 Visual Charts | Quick overview of severity and frequency |

---

## 💬 Sample Visual Report

<details>
<summary>Click to expand & copy</summary>


📊 NetPulse Daily Report

Device: Router1
- Sensor1: 🔴🔴🔴  3 outages, total Downtime: 12 min
- Sensor2: ✅  1 outage, total Downtime: 0.5 min

Device: Server2
- CPU Usage: ⚠️⚠️  2 outages, total Downtime: 4 min
- Memory: ✅  1 outage, total Downtime: 0.8 min

</details>

## ⚙️ How to Use
<details>
<summary>Click to expand & copy instructions</summary>

### 1️⃣ Import Workflow
Go to n8n → Workflows → Import from JSON and select the provided JSON file.
### 2️⃣ Telegram Setup
Replace <YOUR_TELEGRAM_CHAT_ID> in the workflow with your Telegram chat or group ID.
### 3️⃣ PRTG Webhook
Set the n8n Webhook URL in PRTG → Notifications → Webhook.
### 4️⃣ Schedule Reports
Configure the Cron Node for daily or weekly reports according to your preference.

</details>

## 📌 Tips

<details>
<summary>Click to expand & copy tips</summary>

- Enable persistent mode in n8n Global Data Store for long-term data retention.
- Emojis in reports visually indicate outage severity.
- Extend the workflow to notify Slack, Email, or Dashboard.
- Emoji charts provide a quick visual summary for network management.
- 
</details>

## 📅 Last Update

<details>
<summary>Click to expand & copy update info</summary>

- Date: October 21, 2025
- Changes:
  - Added visual emoji charts for daily reports
  - Accurate downtime tracking and reasons
  - Color-coded emojis based on downtime: ✅ <1 min, ⚠️ <3 min, 🔴 ≥5 min
  - Daily/weekly reports include emoji lines for each sensor
</details>
