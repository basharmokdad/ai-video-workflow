# Short video workflow (ChatGPT Codex)

Read `WORKFLOW.md` in this folder before you do anything, and follow it step by step. It is the full process. The look comes from `STYLE.md` in this folder: follow it exactly, and if it is missing, ask me to fill it in before you build.

## How to work

- Use one folder per video. Keep `TIMELOG.md` up to date, with each step's start and end time and anything that failed.
- If a step can't be done, write it in `NOTES.md` and carry on with the next step.
- Codex runs in a sandbox. Give it permission to run `npx`, `ffmpeg` and `python` in this folder, and to reach the web for step 1 (facts) and step 4 (captures).
- Open and check every contact sheet and snapshot before you call a step done.
- Never post anything anywhere. Your job ends at the delivered files.

## Start prompt (paste this, and change the topic)
```
Read AGENTS.md, WORKFLOW.md and STYLE.md first. TOPIC: <your topic>.
Do steps 1-7 of WORKFLOW.md in order. Stop after step 2 and show me the script before you build.
```
