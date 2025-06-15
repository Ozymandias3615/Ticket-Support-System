Support Ticket System

> **Proprietary Project – All Rights Reserved**

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [Running Tests](#running-tests)
- [Deployment](#deployment)
- [License](#license)
- [Contact](#contact)

## Overview
A full-stack help-desk and knowledge-base web application for managing support tickets, user authentication, and curated articles. Access is restricted and proprietary.

## Features
- User sign-in/out (Firebase)
- Role-based access control (users, agents, admins)
- Ticket creation, commenting, file uploads
- Dynamic ticket workflows and status updates
- Automated email notifications (Gmail SMTP & Resend API)
- Knowledge base with search and category-based filtering
- Global search across tickets, services, and articles
- Admin dashboard for user, ticket, article, and service management

## Tech Stack
- Python 3.13, Flask 3.1
- SQLite with PRAGMA migrations
- Jinja2 templating
- Firebase Admin SDK, JWT
- Flask-Mail, Resend API for emails
- pytest for automated testing

## Prerequisites
- Python 3.13 or higher
- pip (Python package manager)
- A Gmail account with an App Password
- Firebase credentials

## Installation
```bash
git clone https://github.com/Ozymandias3615/Support-Ticket-System.git
cd Support-Ticket-System
python -m venv venv
source venv/bin/activate   # on Windows: venv\Scripts\activate
pip install -r requirements.txt
```

## Configuration
Create a `.env` file in the project root with the following keys:
```env
SECRET_KEY=replace-with-secure-random-key
DATABASE=tickets.db
GMAIL_APP_PASSWORD=your-gmail-app-password
FIREBASE_API_KEY=
FIREBASE_AUTH_DOMAIN=
FIREBASE_PROJECT_ID=
FIREBASE_STORAGE_BUCKET=
FIREBASE_MESSAGING_SENDER_ID=
FIREBASE_APP_ID=
RESEND_API_KEY=
```

## Usage
```bash
# Initialize the database
python init_db.py

# Run the development server
python app.py
```
Open your browser at `http://localhost:5050`.

## Running Tests
```bash
pytest
```

## Deployment
Outline your preferred hosting steps (e.g., Docker, Heroku, AWS) here.

## License
This project is proprietary. **All rights reserved.** No part of this repository may be used, copied, distributed, or modified without prior written permission from the author.

## Contact
- Author: Nanabanyin Abbiw
- Email: n.abbiw10@gmail.com
- GitHub: [Ozymandias3615](https://github.com/Ozymandias3615) 