# Short video workflow (Claude Code, Opus or Sonnet)

Read `WORKFLOW.md` in this folder before you do anything, and follow it step by step. It is the full process. The look comes from `STYLE.md` in this folder: follow it exactly, and if it is missing, ask me to fill it in before you build.

## How to work

- Use one folder per video. Keep `TIMELOG.md` up to date, with each step's start and end time and anything that failed.
- If a step can't be done, write it in `NOTES.md` and carry on with the next step.
- Run long renders in the foreground and wait for them to finish. Never leave a render running in the background and end your turn.
- Look at every contact sheet and snapshot yourself before you call a step done.
- Never post anything anywhere. Your job ends at the delivered files.

## Model tip
Sonnet is a good fit for the repeat work. Use Opus for the first run of a new format, or when a judgment call matters, like which facts to keep or which shot to use.

## Start prompt (paste this, and change the topic)
```
Read CLAUDE.md, WORKFLOW.md and STYLE.md first. TOPIC: <your topic>.
Do steps 1-7 of WORKFLOW.md in order. Stop after step 2 and show me the script before you build.
```
