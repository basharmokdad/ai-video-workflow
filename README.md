# AI Video Workflow

One instruction file that any AI coding agent can follow to make a finished vertical Short (1080x1920, 30-40 s): fact-checked script, voice, real screenshots, captions, music, and a mastered final.

We tested the same instructions on three AIs:

| AI | Time | Cost |
|---|---|---|
| ChatGPT (Codex) | 16 min | paid plan |
| Claude Sonnet (Claude Code) | 40 min | paid plan |
| GLM, a free model in OpenCode | ~2.5 h | $0, voice included |

The idea: build the process once with a strong model, write every decision down, and let cheaper models repeat the work. That saves tokens, and you don't need a Claude subscription.

## How to use it

1. Pick the folder for your AI: `claude-code/`, `chatgpt-codex/` or `opencode-free/`. Copy it into an empty project folder.
2. Write your own `STYLE.md` there (the template is at the bottom of `WORKFLOW.md`). This is what makes the videos look like yours.
3. Open your AI in that folder and paste the start prompt from `CLAUDE.md` / `AGENTS.md`, with your topic.

It stops after the script so you can check it before it builds. `ai-video-workflow-pack.pdf` is the same guide as a PDF.

## Needs

Node 20+, Python 3.11+, FFmpeg, and Playwright (Chromium). The free route uses Kokoro for the voice and faster-whisper for captions.

---

Made by [Web Lab](https://www.instagram.com/weblabai/). Follow @weblabai for one of these every day.
