# EE Probation Tracker

A password-protected employee probation management tool built as a single-page React app. Track onboarding milestones, 30/60/90-day reviews, compliance tasks, and probation clearance for all new hires.

## How to Access

1. **Open the app** — Download or clone this repo, then open `index.html` in any browser (Chrome, Edge, Firefox, Safari)
2. **Enter the access code** on the login screen
3. You're in — all changes auto-save to your browser

> The login page features an interactive 3D wireframe globe. Drag to rotate, scroll to zoom.

## Features

### Views
- **Dashboard** — Summary stats, status donut chart, phase progress bars, per-hire completion, AI insights
- **Task Tracking** — Sortable table with inline status/priority dropdowns, overdue highlighting
- **Kanban Board** — Drag-and-drop cards between status columns (Not started, In progress, In review, Done)
- **Gantt / Timeline** — Full-page timeline with per-hire rows, phase-colored bars, today marker

### Employee Management
- **Add Employee** wizard — 3-step form: Employee info, Compliance status, Review & confirm
- Collects name, EE ID, job title, level (G1-G4), manager, department, team, hire date
- Asks compliance questions (E-Verify, I-9, background check, Concentra, health insurance)
- Auto-generates ~20 tasks with correct phases, due dates, and statuses based on your answers

### Email Templates
- Click any task to open the side panel — scroll to **Email Templates**
- Pre-written emails for every task type (I-9 reminders, review scheduling, probation clearance, etc.)
- Auto-filled with employee name, manager, dates, department
- **Copy body** or **Copy all** (includes subject line) to paste into your email client

### AI Assistant (Gemini)
- Floating chat button (bottom-right) for HR onboarding questions
- AI Insights on the Dashboard — analyzes overdue tasks, at-risk employees, and gives actionable recommendations
- Powered by Google Gemini API

### Data
- **Auto-save** — Every change saves instantly to browser localStorage
- **Export backup** — Download a JSON file of all tasks
- **Import backup** — Restore from a previously exported JSON
- **Import CSV/Excel** — Upload spreadsheets with auto column mapping
- **Reset to original** — Restore the initial dataset from the Excel import

## Tech Stack

- **React 18** (CDN, no build step)
- **D3.js** (wireframe globe on login page)
- **Gemini API** (AI chat & insights)
- **localStorage** (auto-save)
- Single HTML file — no server, no dependencies to install

## Running Locally

Just open the file:

```
git clone https://github.com/kimnmd/SKY.git
cd SKY
open index.html
```

Or double-click `index.html` in your file explorer. That's it — no `npm install`, no build, no server needed.
