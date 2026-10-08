# Fernlight Advice — KiwiSaver projection check (portfolio demo)

A one-page KiwiSaver check for New Zealanders. Visitors pick a goal (first home or retirement) and answer one question per screen, with a three-question helper if they don't know their fund type. The projection then unlocks behind an opt-in screen: a balance chart, a settings check, five-year return ranges for their fund type, what-if sliders and a mock booking calendar, followed by a simulated AI-callback notice.

Live demo: https://historfic.github.io/fernlight-advice-kiwisaver/

## About this project

Fernlight Advice is a fictional brand, and this page is a portfolio piece. It is not a real business and does not give financial advice.

- **No backend.** The site is one static `index.html` with inline CSS and JavaScript. The projection is worked out in the browser. The only outside resource it loads is Google Fonts.
- **Nothing is collected or sent.** The form checks what you type, then discards it. No requests are made, nothing is stored, and no cookies are set. A Content-Security-Policy blocks network calls and form submission.
- **The booking calendar is a mock.** It shows sample times, and picking one books nothing.
- **The AI phone call is simulated.** No call is placed.
- **The phone numbers are fictional** and use the 555-01xx range.
- The projection uses published 2026 KiwiSaver settings (contribution rates, the government contribution, ESCT bands and the FMA's prescribed return assumptions) and is for illustration only. The page is not affiliated with IRD, the FMA or any KiwiSaver provider.

## Run locally

Any static file server works. For example:

```bash
python -m http.server 8000
```

Then open http://localhost:8000.
