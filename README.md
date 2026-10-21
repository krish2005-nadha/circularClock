# <Your product name>

> Fill this top section from your Examate project card on Day 1. Replace every line in angle brackets.

## Problem
RBI keeps replacing and amending its Master Directions, and old PDFs stay on staff laptops. Compliance officers waste hours checking whether a paragraph they remember is still valid, and branch staff sometimes follow withdrawn rules.

## Who it is for
User type: Compliance officer at a mid-sized gold-loan NBFC in Coimbatore who needs to monitor RBI updates and ensure the branch follows the latest applicable regulations.

## Signature feature
Time-travel' date picker: ask any question as of a past date and see the answer that was legally correct then.

## Hardest problem (my interview story)

 	
Versioning: latest valid version. Each paragraph is stored with valid-from and valid-to dates, so a question 'as on 1 April 2025' and 'as on today' can give different, correctly cited answers. A side-by-side diff shows exactly which lines changed between two versions.

## Dataset
| Source | Link | Documents | Pages | Licence / terms |
|---|---|---|---|---|
| <name> | <url> | <n> | <n> | <licence> |

## 10 real questions
See [docs/QUESTIONS.md](docs/QUESTIONS.md).

## Run it
```bash
python -m venv .venv && source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements-dev.txt
cp .env.example .env                                 # Windows: copy .env.example .env
uvicorn app.main:app --reload
curl localhost:8000/health
```

## Live link
<Added in Week 2>
