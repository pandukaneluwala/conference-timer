# Session Timer (Web)

A large-screen presentation timer designed for conferences, university sessions, 3MT-style events, and judging panels.

It supports:
- Speaker phase → Judges/Changeover phase → Auto next speaker
- Warning bell at a configurable remaining time (e.g., 30s remaining)
- End-of-speech double bell
- Large, projector-friendly display
- “Up Next” queue (configurable number of names)
- Excel-friendly paste (column/row/multi-cell) in Settings
- Offline-friendly after first load (static HTML/JS)

Developed by **Panduka Neluwala**.

## Live
Once GitHub Pages is enabled:
- Settings: `https://pandukaneluwala.github.io/tea/settings.html`
- Timer: `https://pandukaneluwala.github.io/tea/timer.html`

## How to use (fast)
1. Open **Settings**
2. Paste participant names (from Excel or text)
3. Set durations (Speaker, Judges, Warning time)
4. Click **Save & Open Timer**
5. On timer screen: click **START SESSION** (enables audio)

### Keyboard shortcuts
- Space: Pause/Resume
- → : Next speaker (with bell)
- ← : Previous speaker
- R : Reset current phase
- S : Go back to Settings

## Notes
- Settings are stored in the browser using **LocalStorage** (no server, no uploads).
- If browser storage is cleared, settings will reset.
- Audio requires a user click (“START SESSION”) due to browser security policies.

## Contributing / Improving
Contributions are welcome (PRs or issues). Some ideas:
- Add a **Full-screen** toggle button
- Add **Export/Import settings** (JSON) for portability between devices
- Add **Session saving** (multiple lists, multiple rounds)
- Add a **remote control** page (phone controls tablet) using WebSockets (requires backend)
- Add **PWA install** support for offline install on Android/desktop
- Add accessibility improvements (high-contrast mode, dyslexia-friendly font)

### Design principles for contributors
- Timer screen must remain **distraction-free**
- No pop-ups/ads on the timer screen
- Changes should work on a projector and on tablets
- Keep it lightweight: plain HTML/CSS/JS preferred

## License
MIT (recommended for open sharing and reuse).
