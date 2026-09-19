# System Design Roadmap

A 26-week, day-by-day plan (in Russian) for system design fundamentals, the Azure Solutions Architect Expert and AWS Solutions Architect Associate certifications, and interview preparation for EU/UK/US roles.

- **Plan:** [plan.md](plan.md)
- **Web page with progress tracking:** https://alexander-shamray.github.io/system-design-plan/

The page renders `plan.md` and adds a checkbox to every day. Progress is stored in your browser's `localStorage`, so it stays on that device and browser only.

To move progress between devices, use the header buttons:

- **⤓ Export** downloads `sd-roadmap-progress-YYYY-MM-DD.json`.
- **⤒ Import** merges a file into the current progress. Days checked in either place stay checked. Import never unchecks a day, so to uncheck one, do it on every device.

## Run locally

```sh
python -m http.server 8000
# open http://localhost:8000
```

Opening `index.html` straight from disk does not work, because the page fetches `plan.md`.
