# face_rec

A face-recognition service. The dependencies suggest a FastAPI backend with a
FaceNet/Keras recognition pipeline and a SQL database (Alembic migrations).

> **Note:** source code has not been committed yet — this repo currently holds
> the project scaffolding (dependencies, ignore rules). Application code goes in
> this folder.

## Getting started

This project uses Python 3.8. Create and activate a virtual environment, then
install the dependencies.

### Windows (PowerShell)

```powershell
python -m venv .
.\Scripts\Activate.ps1
pip install -r requirements.txt
```

### macOS / Linux

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## Notable dependencies

- **FastAPI / Uvicorn** — web API
- **keras-facenet, TensorFlow/Keras** — face embedding & recognition
- **SQLAlchemy, Alembic, asyncmy** — database layer and migrations
- **bcrypt, python-jose/ecdsa, cryptography** — auth / security

See [requirements.txt](requirements.txt) for the full pinned list.

## Project layout

```
.
├── .gitignore
├── requirements.txt
└── README.md
```

The virtual environment (`Include/`, `Lib/`, `Scripts/`, `pyvenv.cfg`) is
intentionally **not** tracked — recreate it from `requirements.txt`.
