# Remind-me-later 

A simple Django-powered API that allows users to set reminders with a custom message, date, time, and notification type (SMS or Email). While the frontend is built by JS developers, this backend API is responsible for storing reminder data securely in the database.

---

##  Features

- Accepts reminders with:
  -  Date
  -  Time
  -  Message
  - ✉ Reminder type (SMS or Email)
- Clean and RESTful API using Django REST Framework
- Easily extendable for future reminder types

---

##  Tech Stack

- Python 
- Django 
- Django REST Framework 
- SQLite (default DB, switchable to PostgreSQL or others)

---

##  API Endpoint

### `POST /api/reminders/create/`

**Request Body:**

```json
{
  "date": "2025-05-14",
  "time": "15:30:00",
  "message": "Meeting with client",
  "reminder_type": "sms"
}
