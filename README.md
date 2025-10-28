# Paranoid Stash

Is a web app for password managing.

## Architecture

Frontent - React + Vite, TS

Backend - FastAPI + PostgreSQL

## Run Frontend

- DEV

```bash
npm run dev
```

- Build

```bash
npm run build
```

## Run Backend server

- DEV

```bash
uvicorn --host 0.0.0.0 --port 8000 --workers 4 main:app --reload
```

- PROD

```bash
uvicorn --host 0.0.0.0 --port 8000 --workers 4 main:app
```

### Restore deleted file from remote repo.

git restore --source=origin/main -- LICENSE
