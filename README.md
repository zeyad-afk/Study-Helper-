# Study Desk

A weekly study tracker with adjustable topics, per-topic timers, and a Mon–Fri timetable that bridges to Apple Calendar.

## Features

- **Topics you control** — starts with four seeded topics, but you can add more (or remove old ones) any time from the "+" tile at the bottom of the topic list. Each new topic gets a randomly assigned icon from the existing set.
- **Per-topic timers** — a 10-hour weekly study countdown and a break timer that automatically pauses whichever one isn't active.
- **Session goals** — a notepad per topic for what you're aiming to get through.
- **Weekly timetable** — a Mon–Fri, 9am–7pm grid in 15-minute increments. Click any square, pick a duration (from 15 minutes up to 4 hours), and assign a topic — so a class running 4:00–5:15 fits exactly, not rounded up to a full hour.
- **Important events** — a free-text notes box on the timetable page for exam dates, assignment deadlines, anything worth remembering. Saves automatically.
- **Apple Calendar bridge (.ics)** — since a website can't get live, two-way access to the Calendar app, this uses the standard interchange format instead:
  - **Export**: downloads your timetable as a `.ics` file with repeating weekly events. Open it (or AirDrop it to your phone) and it drops straight into Apple Calendar.
  - **Import**: reads a `.ics` file exported from Apple Calendar and overlays those events onto the grid (events outside the Mon–Fri/9–6 grid are listed separately below it).
  - Neither direction is "live" — re-export or re-import whenever something changes.

## Usage

Just open `index.html` in a browser. No build step, no dependencies — it's a single self-contained file (HTML, CSS, and JS all inline).

Progress, topics, and timetable data are saved automatically using the browser's own storage (`localStorage`), or the Claude.ai artifact storage API when running inside claude.ai. Either way, everything persists between visits on the same device and browser.
