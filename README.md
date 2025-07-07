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
# Data Flow Diagram for Phishing Email Detector WebTool

This moderate Level-0 Data Flow Diagram (DFD) illustrates the core data flow in the Phishing Email Detector WebTool, showing how users and admins interact with the system, external APIs, and the database.

# Graph TD
    A[User] -->|Login/Register| B(Phishing Detector System)
    A -->|Submit Email| B
    A -->|View Scan History| B
    C[Admin] -->|View Statistics| B
    B -->|Extract URLs/Keywords| D[Rule-Based Analysis]
    B -->|Query Threat Data| E[External APIs]
    B -->|Store/Retrieve Data| F[(MongoDB Database)]
    D -->|Analysis Results| B
    E -->|Threat Data| B
    F -->|Scan History| B
    B -->|Result & Score| A
    B -->|Scan Statistics| C
# Explanation
- Entities:
1. User: Submits email content (paste/upload), logs in/registers, and views scan history.
2. Admin: Views scan statistics and flagged emails.
3. External APIs: Includes Google Safe Browsing, PhishTank, and WhoisXML for threat intelligence.
- Processes:
1. Phishing Detector System: Manages authentication, email analysis, API queries, and result display.
2.  Rule-Based Analysis: Extracts URLs and keywords for phishing detection.
3.  Data Store: MongoDB Database stores scan results and history.
4.  Data Flows: Email submission, analysis, API queries, data storage, and result/statistics display.

---


