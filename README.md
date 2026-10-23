# UniFlow

A responsive, local-first student planner built with plain HTML, CSS, and JavaScript. There is no build step, account, backend, cloud sync, or AI feature. The app stores data in this browser's `localStorage`.

## Run locally

From the project folder, start a local server:

```powershell
python -m http.server 8000
```

Open [http://localhost:8000](http://localhost:8000). Stop the server with `Ctrl+C`. No package installation is required.

## Included

- Dashboard with today's classes, upcoming events, exam countdown, and semester progress.
- An 08:00–18:00 weekly timetable with recurring classes bounded by semester dates, single-occurrence moves/cancellations, manual break periods, and visible conflict markers.
- A separate calendar for independently created one-off events; recurring classes are not copied into it.
- Courses, exams, classes, and personal calendar events.
- Configurable focus timer, recorded focus sessions, progress statistics, and JSON backup export/import.

Existing local data is retained when loaded, including older course records and note data. Notes are no longer shown in the interface. New installs start empty.

## Limitations

- Breaks and holidays are configured manually; there is no external holiday calendar.
- Recurring classes repeat weekly on one weekday. A specific occurrence can be moved to another date/time or cancelled without changing the series.
- The focus timer records a study session on completion, but does not send system notifications.
- Browser data is local to this device and browser. Export a backup before changing devices or clearing site data.

