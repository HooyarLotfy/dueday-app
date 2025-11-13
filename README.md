# DueDay 💻

A tiny webapp that helps adults quickly add bills or subscriptions and never forget a payment with reminders via email and notifications.

## 📜 Idea in a Sentence
Add, track, and get reminded of bills/subscriptions so nothing slips through the cracks.

---

## ⭐ Key Features

- Add a bill/subscription: name, amount (optional), due date.  
- Dashboard showing upcoming due bills.  
- Mark bills as paid.  
- Email reminders (optional, via free-tier SMTP like SendGrid or Gmail).  
- Simple stats: total bills due this month.  
- Google OAuth login (optional for mini MVP).  
- Landing page exactly as designed.  
- Interactive dashboard: add/edit subscriptions with popups.

---

## 🖥 Frontend Tech

- Blade templates (`.blade.php`)  
- TailwindCSS or Bootstrap  
- Vanilla JS / Alpine.js for interactivity  

---

## ⚙️ Backend Tech

- Laravel (latest stable)  
- Laravel Mail + free-tier SMTP (SendGrid / Gmail)  
- Laravel Scheduler for daily reminders  

---

## 🛠 Libraries / Extras

- Alpine.js — lightweight reactive frontend  
- Carbon (Laravel) — date formatting & reminders  

---

## 📂 Database

**MySQL** — simple table structure:

| Column   | Type         |
|----------|-------------|
| id       | int (PK)     |
| name     | varchar      |
| due_date | date         |
| amount   | decimal      |
| status   | enum (paid/unpaid) |
| user_id  | int (FK)     |

---

## 🚀 Deployment

- Shared hosting via cPanel  
- Laravel deployed via subfolder or subdomain  
- Cron job for daily reminders  

---

## ⚡ Complexity Level

Very Low / Mini MVP — can be built by one developer in 1 day.  
Google OAuth optional for demo purposes.

---

## 📌 Notes

- Focus on simplicity: dashboard, add/edit cards, basic stats.  
- Email notifications optional but recommended for full experience.  
- Keep frontend minimal but functional.  
