# StudyFlow

A polished, local-first student timetable and study planner made for a hackathon demo. It is a dependency-free static web app: all data lives in the browser's `localStorage`.

## Run locally

1. Download or clone this repository.
2. Open `index.html` in a modern browser, or serve it from the project folder:

   ```bash
   python -m http.server 8000
   ```

3. Visit `http://localhost:8000`.

No install, API key, login, or backend is required.

## Features

- Monday–Sunday timetable from 8:00 AM–8:00 PM, with colour-coded class blocks
- Add, edit, and delete classes; required-field, time-range, and overlap validation
- Today dashboard with next-class countdown, schedule, and weekly task progress
- Assignments/exams with priority, completion state, due dates, and editing
- Rule-based study-plan generator that turns available hours into a day-by-day checklist
- Persistent dark/light theme and data through `localStorage`
- Sample demo data, reset control, responsive mobile layout, keyboard-friendly controls, and optional browser notifications

## demo script (about 90 seconds)

1. Open **Today** and point out the live next-class status plus the weekly progress card.
2. Scroll to **Your timetable**. Click a coloured class block to show editing, then add a new class (try an overlap to demonstrate friendly validation).
3. Open **Assignments & exams**, check off a task, and show the progress percentage update.
4. In **Study-plan generator**, select “Midterm: Calculus II,” enter 6 hours, and build a paced checklist.
5. Toggle dark mode; refresh the browser to demonstrate that the chosen theme and data persist.
6. Use **Reset demo data** to return to the clean demo state.

## Project structure

- `index.html` — accessible app markup and dialogs
- `styles.css` — responsive visual system and themes
- `app.js` — local state, validation, rendering, and planner logic
