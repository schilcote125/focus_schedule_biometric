Biometric Focus Schedule
A personal weekly schedule built around biometric data from Oura and Whoop, rather than arbitrary time blocks. The structure maps directly to a real heart rate pattern — protecting peak cognitive bandwidth in the morning and leaning into the natural volatility of the afternoon rather than fighting it.
What It Is
A single-file web app that runs in any browser with no dependencies, no installs, and no backend. It functions as a daily reference tool and a lightweight notes system for each time block.
The Framework
The schedule is organized around four biological zones identified from heart rate data:
Zone	Time	Logic
Deep Anchor	8:30–11:30 AM	Heart rate is most stable here. Reserved for heavy cognitive work — SQL, PowerBI, analytical reporting, coursework.
Flex & Fuel	11:30 AM–1:00 PM	Natural biological dip with movement spikes at ~10:34 and ~12:26. Dog walk + lunch + decompression.
Reactive Triage	1:00–5:30 PM	Heart rate becomes volatile (82–102 bpm). Lean into reactive mode — meetings, email, partner requests, ad-hoc work.
Physical Deactivation	5:30–6:00 PM	Natural activity spike. Dog walk, close tabs, hard stop on the workday.
Weekly Variations
Each day is structured differently to account for standing appointments and rotating focus priorities:
Monday — Therapy at 11:00 AM clips the anchor to 2.5 hours. Full afternoon for BHFS triage.
Tuesday — German lesson at 8:30 AM acts as a cognitive warmup before technical deep work. Biggest BHFS triage block of the week.
Wednesday — No fixed appointments. Full uninterrupted 3-hour Deep Anchor. Cleanest window of the week.
Thursday — Anchor flips to personal and strategic work. BHFS takes the afternoon triage window.
Friday — Anchor closes week deliverables. Back end of triage reserved for Weekly Review.
Sunday — Minimal structure. Workout, German practice, open personal time. No work.
Features
Day tabs — Switch between Monday through Friday and Sunday
Biometric HR curve — Visual approximation of the heart rate pattern that drives the schedule structure, with colored zone overlays and dip markers
Per-block notes — Each time block has a collapsible notes panel. Notes auto-save to localStorage and persist between sessions
Recovery status — Header badge reflects Whoop recovery and REM status as a daily reminder to calibrate output expectations accordingly
Fully offline — No external dependencies beyond Google Fonts. Works without an internet connection once loaded.
Usage
Open the URL in any browser. Click a day tab to view that day's block schedule. Click ✎ Notes on any block to expand the notes panel — notes save automatically after a short delay and are indicated by a blue dot on the button.
Notes are stored in the browser's localStorage tied to this URL. They persist across sessions on the same device and browser.
Stack
Plain HTML, CSS, and vanilla JavaScript. No frameworks, no build tools, no package.json. The HR curve is a generated SVG path from approximated biometric data points.
