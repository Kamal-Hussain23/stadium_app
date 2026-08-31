# Technology & Architecture

## Stack

| Layer | Technology | File |
|-------|------------|------|
| Frontend | HTML, CSS, JavaScript | `frontend/index.html`, `frontend/app.js` |
| Backend | Flask (Python) | `backend/app.py` |
| Data Layer | Python + SQLite | `backend/data_layer.py` |
| Database | SQLite | `stadium.db` |

## Architecture

```
Frontend  →  Backend (Flask)  →  Data Layer  →  SQLite Database
```

**Rules:**
1. Frontend only makes HTTP requests. No SQL.
2. Backend only handles routes. No SQL.
3. Data Layer is the only place that talks to SQLite.
4. All SQL uses parameterized queries (never string concatenation).

## Engineering Standards

- **Walking skeleton** — build the thinnest working slice first, then grow
- **Simplicity** — prefer simple solutions over clever ones
- **DRY** — don't repeat yourself; extract shared code into functions
