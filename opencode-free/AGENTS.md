# Short video workflow (OpenCode, $0)

Read `WORKFLOW.md` in this folder before you do anything, and follow it step by step. It is the full process. The look comes from `STYLE.md` in this folder: follow it exactly, and if it is missing, ask me to fill it in before you build.

## This run must cost $0

- **Model:** a free model in OpenCode. We used GLM 5.3. A model that can see images (a "VL" model) is better, because it can check its own frames.
- **Voice:** Kokoro (`pip install kokoro-onnx soundfile`, plus the free model files from github.com/thewh1teagle/kokoro-onnx releases). Never use a paid voice API.
- **Captions:** faster-whisper for word timings (`pip install faster-whisper`).
- **Music:** a track you own, or none at all. Never use a paid music API.
- **Cover:** set type in HTML over a frame from your video. No image generation.

## How to work

- Use one folder per video. Keep `TIMELOG.md` up to date, with each step's start and end time and anything that failed.
- Free models are slower, so plan for 2-3 hours. Work through it one step at a time, and save after each step.
- If a step can't be done, write it in `NOTES.md` and carry on with the next step.
- Never post anything anywhere. Your job ends at the delivered files.

## Start prompt (paste this, and change the topic)
```
Read AGENTS.md, WORKFLOW.md and STYLE.md first. This run must cost $0. TOPIC: <your topic>.
Do steps 1-7 of WORKFLOW.md in order. Stop after step 2 and show me the script before you build.
```
