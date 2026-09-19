# IITP Exam Lookup

A lightweight, client-side exam timetable portal for IIT Patna students.

Search a roll number to find registered courses, exam dates, morning/evening slots, and room allocations. The portal also supports multi-user comparison by grouping students who share the same date, slot, and room.

## Features

- Single roll-number search
- Multi-user search with addable roll-number fields
- Grouping by exam date, slot, and room
- Course-wise registration lookup
- Room allocation support for labels such as `LT001`, `LT101`, and `LT102`
- Clickable course details showing all courses in the same room
- Single-user `.ics` calendar export
- Multi-user PNG download and print layout
- Responsive desktop, tablet, and mobile layout
- No backend or database required

## Data source

The portal fetches the published Google Sheets data directly in the browser:

- Timetable and room allocation
- Course-wise registered roll numbers

## Run locally

```bash
python3 -m http.server 4173
```

Open:

```text
http://localhost:4173
```

## Notes

The Google Sheet must remain publicly viewable for live browser-side fetching to work. The portal does not store roll numbers or timetable data.
