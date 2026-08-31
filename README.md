# Stadium Security Management System

A web-based security dashboard for monitoring and managing stadium gate entries, badge scans, and security alerts.

## Architecture

```
Frontend (HTML/JS)  →  Backend (Flask API)  →  Data Layer (Python)  →  SQLite (stadium.db)
```

| Layer | File | Responsibility |
|-------|------|----------------|
| Frontend | `frontend/index.html`, `frontend/app.js` | UI rendering, HTTP requests |
| Backend | `backend/app.py` | Route handling, request validation |
| Data Layer | `backend/data_layer.py` | SQL execution, parameterized queries |
| Database | `stadium.db` | Persistent storage |

## Quick Start

```bash
./run.sh
```

The server starts on `http://localhost:5000`.

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/entries` | List all stadium entries |
| GET | `/api/entries?gate=A` | Filter entries by gate |
| GET | `/api/health` | Health check |

## Project Structure

```
stadium_app/
├── backend/
│   ├── app.py              # Flask API server
│   └── data_layer.py       # SQLite data access layer
├── frontend/
│   ├── index.html           # Security Command Dashboard
│   └── app.js               # Frontend logic
├── SPECS/
│   ├── TECH.md              # Technical architecture
│   └── ROADMAP.md           # Engineering milestones
├── seed.sql                 # Database seed data
├── run.sh                   # Server startup script
└── stadium.db               # SQLite database
```

## Development

See `SPECS/ROADMAP.md` for the current development status and upcoming features.
