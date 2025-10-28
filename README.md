# ================================================================================================

# Paranoid Stash

# ================================================================================================

Is a web app for password managing.
All passwords are stored in encrypted files on the server.
Decryption, reading and encryption are performed on users machine only.

## ================================================================================================

## Architecture

## ================================================================================================

Frontent - React + Vite, TS

Backend - FastAPI + PostgreSQL

## ================================================================================================

## Run Frontend

## ================================================================================================

- DEV

```bash
npm run dev
```

- Build

```bash
npm run build
```

## ================================================================================================

## Run Backend server

## ================================================================================================

- DEV

```bash
uvicorn --host 0.0.0.0 --port 8000 --workers 4 main:app --reload
```

- PROD

```bash
uvicorn --host 0.0.0.0 --port 8000 --workers 4 main:app
```

## ================================================================================================

### Restore deleted file from remote repo.

## ================================================================================================

git restore --source=origin/main -- LICENSE

## ================================================================================================

## CODEOWNERS Template

## ================================================================================================

📂 Possible pathes to store CODEOWNERS file

1️⃣ .github/CODEOWNERS .github/CODEOWNERS 🔥 Highest priority
2️⃣ CODEOWNERS в корне /CODEOWNERS Second
3️⃣ docs/CODEOWNERS /docs/CODEOWNERS Third

```
# Comments start with #
# The main OWNER of the whole repo:
* @user1 @org/team-a

# Specified file:
README.md @user2

# Folder (and all its content):
/src/ @org/frontend-team

# Subfolder in every place:
docs/** @org/tech-writers

# All .js files in the root folder:
*.js @user3

# All Python files in all places:
**/*.py @org/backend-team

# Several owners for the same path template:
/infra/ @org/devops @user4
```
