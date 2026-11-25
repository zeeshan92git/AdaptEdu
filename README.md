# AdaptEd

An adaptive learning dashboard that rearranges its widgets based on learner behaviour, explains each change, and lets the learner lock, undo or reset it. Final-year HCI course project.

**Stack:** React (Vite), Node.js + Express, MongoDB Atlas (Mongoose).
**Status:** planning and analysis documents are in `docs/`. Application code is generated phase by phase (see `docs/prompts/`).

## Folder structure

| Folder | What it holds |
|---|---|
| `client/` | React front end (Vite) |
| `server/` | Express API, Mongoose models, seed script |
| `server/seed/` | `topics.json`, `resources.json`, `questions.json` (placeholders for now) |
| `docs/research-and-analysis/` | Research findings, observation protocol, empathy maps, personas, journey map, task analysis |
| `docs/prompts/` | Prompts used with the coding agent |
| `docs/design/` | Figma links and design exports |
| `docs/private/` | Local-only material (for example the textbook PDF). Ignored by Git. |

## Setup (once the code exists)

1. Install Node.js (current LTS) and Git.
2. Create a free MongoDB Atlas cluster and a database user limited to one database.
3. Copy `server/.env.example` to `server/.env` and fill in the real values. **Never commit `.env`.**
4. Install dependencies in `server/` and `client/`, seed the database, then start both apps. Exact commands will be added here when Phase 8 is complete.

## Pushing to GitHub

```bash
git init
git add .
git status          # check that .env does NOT appear in the list
git commit -m "ADAPT-1: initial project structure"
git branch -M main
git remote add origin <YOUR_REPO_URL>
git push -u origin main
```

Start commit messages with the Jira key, for example `ADAPT-6: add rule engine`.

## Content and licence notes

Study resources are linked, not copied, and each card shows its source and licence. The reference textbook is *Introduction to Human-Computer Interaction* (Hornbaek, Kristensson, Oulasvirta, OUP 2025, CC BY-NC-ND 4.0). Questions are written in our own words, and the PDF is not stored in this repository.
