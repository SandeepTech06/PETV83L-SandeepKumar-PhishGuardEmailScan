# 🛡️ PhishGuard — Phishing Email Detector WebTool

An advanced full-stack web application that helps users detect phishing, suspicious, and safe emails with real-time threat intelligence.

![PhishGuard Banner](https://via.placeholder.com/1000x300?text=PhishGuard+Phishing+Detector+WebTool) <!-- Replace with actual banner if available -->

---

## 🚀 Live Demo

> https://phishguard-email.whoisalok.tech/

---

## 📌 Features

- 📝 Paste or upload suspicious email content
- 🔍 Detect and classify as **Safe**, **Suspicious**, or **Phishing**
- 🌐 Extract & scan URLs using real-world threat intelligence APIs
- 🧠 Rule-based keyword detection
- 📊 Risk score (0–100%) + explanation
- 💡 Human-readable summaries (optional OpenAI API integration)
- 🧑‍💻 Admin panel to view total scans and stats (optional)
- 🌗 Light/Dark mode UI

---

## 🧰 Tech Stack

| Layer          | Technologies                                      |
|----------------|---------------------------------------------------|
| Frontend       | Next.js (React), Tailwind CSS                     |
| Backend        | Node.js, Express.js                               |
| Database       | MongoDB Atlas                                     |
| External APIs  | Google Safe Browsing, PhishTank, WhoisXML         |
| Optional       | OpenAI GPT API for explanations                   |

---

## 🌐 Architecture Overview

1. **User Input:** Paste/upload email content.
2. **Frontend (Next.js):** Sends data to backend.
3. **Backend (Express):**
   - Extracts URLs, scans for keywords.
   - Calls threat intelligence APIs.
   - Generates classification + risk score.
4. **Result Display:** Frontend shows result with explanation.
5. **Database (MongoDB):** Saves scans & optional user feedback.

---

## 🧪 External APIs Used

| API                  | Purpose                                  |
|----------------------|------------------------------------------|
| Google Safe Browsing | Check URLs for malware/phishing threats  |
| PhishTank API        | Detect known phishing URLs               |
| WhoisXML API         | Get domain age & sender reputation       |

---


