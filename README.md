# Paranoid Stash

Is a web app for password managing.
All passwords are stored in encrypted files on the server.
Decryption, reading and encryption are performed on users machine only.

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

## CODEOWNERS Template

```
# Комментарии начинаются с #
# Общий владелец для всего репозитория:
* @user1 @org/team-a

# Конкретный файл:
README.md @user2

# Папка (все содержимое):
/src/ @org/frontend-team

# Подпапка где-то в любом месте:
docs/** @org/tech-writers

# Все JS файлы в корне:
*.js @user3

# Все Python файлы в любом месте:
**/*.py @org/backend-team

# Несколько владельцев для одного пути:
/infra/ @org/devops @user4
```
