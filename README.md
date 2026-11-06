# Speaking Test Simulator

A full practice Speaking test: Part 1, Part 2 and Part 3 in order, with the questions read aloud and your answers recorded.

Part of the [IELTS Study Suite](https://github.com/Apurba94/ielts-study-suite): 100 free study apps for IELTS. This one is for the IELTS Academic and General Training test. It works offline, as a Windows program or in the browser.

## Download and run

- **Windows:** download `Speaking Test Simulator.exe` from the [latest release](https://github.com/Apurba94/ielts-speaking-test/releases/latest) and open it. Nothing to install. It opens in its own window and saves your progress in your user folder.
- **Browser:** open it online in the suite's web edition at https://ielts-study-suite.vercel.app/apps/ielts-speaking-test/ . Progress stays in that browser.
- **From source:** `python launcher.py` (Python 3.10 or later, no packages needed).

## What it does

A full practice Speaking test in the real order: Part 1 questions about yourself (four to five minutes), a Part 2 long turn with one minute to prepare and up to two minutes to speak, then Part 3 discussion questions linked to Part 2 (four to five minutes). In all, it takes 11 to 14 minutes. Every answer is recorded on this device so you can listen back or share it with a teacher.

Sections: Test, Recordings, Progress, About.

## How to use it

1. Find a quiet room and allow 15 minutes. Allow the microphone when asked.
2. Press **Start the test** and answer each question as the computer reads it.
3. At the end, listen to your recordings and rate them in the Speaking Self-Check app.

## Good to know

- All questions, passages, recordings and definitions were written for this suite. None are official IELTS questions. For official practice, use the materials on ielts.org and from the test partners.
- It follows IELTS as delivered on computer in 2026. Formats change, so check ielts.org before your test.
- Listening uses the voices installed on your computer, which sound less natural than real test recordings.
- Feedback on writing and speaking counts what a program can count honestly, such as length and linking words. It is not an IELTS band score. Band conversions for Listening and Reading are approximate.
- Not endorsed by or affiliated with the British Council, IDP or Cambridge University Press & Assessment. IELTS is a registered trademark of its owners.

## For developers

The app is plain HTML and JavaScript in `web/`, run by a small Python launcher that serves it on 127.0.0.1 only and needs a secret token for saving. Tests: `node --test "tests/*.test.js"` (29 tests) and `python -m unittest discover -s tests`. Build the .exe with `python build_exe.py`.

Built with AI assistance (Claude Code). MIT licence. By JANIN A APURBA.
