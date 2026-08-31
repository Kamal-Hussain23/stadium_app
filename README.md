# Stadium Security Dashboard

A web app for tracking stadium entry logs. Built to prevent data loss during investigations.

## Quick Start

```bash
./run.sh
```

Then open `http://localhost:5000` in your browser.

## Project Structure

```
stadium_app/
├── backend/
│   ├── app.py              # Flask routes
│   └── data_layer.py       # SQLite queries
├── frontend/
│   ├── index.html           # Dashboard UI
│   └── app.js               # Fetch logic
├── SPECS/
│   ├── MISSION.md           # Why this project exists
│   ├── TECH.md              # Architecture rules
│   └── ROADMAP.md           # What's next
├── seed.sql                 # Sample data
└── run.sh                   # Start script
```

## Features

- View stadium entry logs
- Filter by gate (A, B, C, D)
- See person names and phone numbers
- Data saved in SQLite (survives crashes)
