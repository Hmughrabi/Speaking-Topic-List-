# 🎓 Level 1 Speaking Exam - Topic Selection Portal

A lightweight, real-time web application built for **Dhofar University (Centre for Preparatory Studies)** to manage student final speaking exam topic selections efficiently and prevent duplicate choices.

---

## 🚀 Key Features

* **Real-Time Conflict Prevention:** Once a student selects a topic, it is instantly locked out so no other student can choose the same topic.
* **Student Verification:** Requires students to input their full name and Student ID number before picking a topic.
* **Cloud-Synced Storage:** Powered by a free Google Sheets backend via Google Apps Script, allowing students to access it from any device (phones, laptops, tablets).
* **Instant Excel Export:** Instructors can download the complete list of selections as a Microsoft Excel (`.xlsx`) file directly from Google Sheets at any time.
* **Modern Responsive UI:** Designed with a clean, professional aesthetic using Tailwind CSS.

---

## 🛠️ Tech Stack

* **Frontend:** HTML5, Vanilla JavaScript, Tailwind CSS (via CDN)
* **Backend / Database:** Google Apps Script & Google Sheets (Free cloud infrastructure)
* **Hosting:** Netlify / GitHub Pages

---

## ⚙️ Setup & Configuration Guide

### 1. Frontend Setup (`index.html`)
The main interface is contained in `index.html`. It communicates with your backend via the `SCRIPT_URL` variable located inside the script section:
```javascript
const SCRIPT_URL = "YOUR_GOOGLE_APPS_SCRIPT_WEB_APP_URL_HERE";
