# OOP-Ex2-Teaching-Tool
Simple, extensible web app for classroom management: attendance and other tools like comments and polls.
# OOP-Ex2-Teaching-Tool
Simple, extensible web app for classroom management: attendance and other tools like comments and polls.

## Problem
Existing online teaching tools are complicated: they require logins, installation or training, and take valuable time away from the lesson. They also make little use of AI (lecture summaries, homework feedback), and attendance is still often taken manually, which is slow and easy to fake. We want a single, simple tool that opens in the browser of a phone: lecturers get attendance and polls in seconds, students get feedback and their attendance history, and the structure can grow with additional small tools.

## Features
1. **Attendance (core).** Students check in from their phones; the lecturer gets an online/offline spreadsheet; students see their own attendance history.
2. **Comments & suggestions.** Real-time during class, or asynchronously for the lecturer to answer later. Students can choose to comment anonymously.
3. **Polls.** Lecturers create quick on-the-spot polls on the current material. Polls are anonymous for now.
4. **Lecture summary.** Lecturer pastes a transcript; an LLM returns a summary. *The demo uses pasted text.*
5. **Homework review.** Students submit homework as files in a public Git repository; an LLM gives feedback and the student's relative position in the class. *Git submission is part of the design only. The demo uses pasted text instead.*

## Scope
**In:** students check in, send comments, and answer quick polls; lecturers get attendance reports and lecture summaries; students get homework feedback.
**Out:** Moodle integration, Zoom integration, integration with external personal-data systems (only a name/ID per student is stored).

## Assumptions
- The class is physical (not on Zoom).
- The demo uses one course; the data model supports multiple courses.
- Students have smartphones with internet access in class.
- In the demo, the lecture transcript and homework are pasted as text.
- Students have GitHub accounts and submit to a public repository (design only).

## Open Questions
- How do we prevent attendance fraud (a student checking in for a friend)? Options to evaluate: a rotating QR code on the classroom screen, a short-lived check-in link, or a combination.
- What counts as "relative position" in the homework comparison? Options to evaluate: a verbal description (e.g., "your approach is common in the class") or a numeric ranking.

## Future Work
- Transcript file upload / auto-transcription

## lecturer code
for demo - 4644

