# The Web Lab faceless Short workflow

One instruction file that any AI coding agent can follow to make a finished vertical Short: Claude Code (Opus or Sonnet), ChatGPT Codex, or a free model in OpenCode.

We built this process once with Claude Opus, then wrote every decision down. The expensive model plans once, and any model repeats the work.

---

## What you get

A 30-40 second vertical video (1080x1920, 60 fps) about one topic:

- fact-checked, with every claim tied to a source;
- a narrator voice, one line at a time;
- real screenshots of the real thing, on screen as you talk about them;
- burned-in captions, music, and an end card in YOUR style;
- mastered to -14 LUFS, the loudness YouTube, TikTok and Instagram expect.

## Tools (free unless marked paid)

| Job | Tool |
|---|---|
| Animation and render | HyperFrames (`npx hyperframes`), which turns HTML into video |
| Video and audio work | FFmpeg |
| Captures of real pages | Playwright (Chromium) |
| Voice, paid | ElevenLabs v3 |
| Voice, free | Kokoro (Apache-2.0, runs on your CPU) |
| Word timings for captions | faster-whisper (free) |
| Music, paid | ElevenLabs Music |
| Music, free | any track you own a licence for, or no music |

---

## The steps (do them in this order)

### 1. Facts first
Find the official sources: the vendor's own pages and docs. Confirm every claim, and write `fact-check.md` with four columns: claim, verdict, exact quote, URL. If you can't confirm a claim, cut it. Never invent a number, a quote or a feature.

### 2. Script (30-40 s)

- Line 1 is the hook. It contradicts a belief or reveals a result ("One of these videos cost zero dollars.").
- One idea per sentence, 6-8 sentences in total.
- Every number shown on screen is also spoken.
- The last line is the call to action, then "Follow [your channel]. And remember:", so the end loops back into line 1.

### 3. Voice

- One audio file per sentence.
- Never speed the voice up. Shorten long pauses instead.
- Give each line a short fade at the end, so it doesn't cut off hard.
- Time every word (faster-whisper with word timestamps). Captions and cards are timed to these words.

### 4. Real material

- Capture the real thing: official pages in dark mode, real product screens, a real output if you can make one.
- Use Playwright at 2-3x pixel density, so text stays sharp on a phone.
- Put every capture on one contact sheet and look at it before you use any of them.
- Never generate a fake screenshot of a product.

### 5. Build (in your own style)
Your AI builds the video from the `STYLE.md` you write below, not from anyone else's look. Without one, every video looks generic.

- Frame 0 must already be moving, with the hook on screen. Never fade in from black.
- Show one idea on screen at a time, changing on the spoken word.
- Keep the captions away from anything important.
- Duck the music under the voice.

### 6. Check (never skip this)

- The file is 1080x1920 at 60 fps, and audio and video end within 0.05 s of each other.
- Loudness is -14 LUFS, with the true peak at or below -1 dB.
- There are no black frames, no frozen stretch over 1 second, and no one-frame flashes.
- Take a snapshot at every card and look at each one: nothing clipped, empty or off the frame.

### 7. Deliver
`final.mp4`, a 720p preview, a contact sheet, and a cover image. Keep a `TIMELOG.md` of when each step started and finished, and what failed.

## Your style (write this first)

Make a file called `STYLE.md` in your video folder and fill it in. This is what makes the videos yours. Add every correction you give the AI to this file.

```
# My video style
Colours:      ...
Fonts:        ...
Cards:        how screenshots and text sit on screen
Captions:     size, colour, words at a time
Pacing:       a new shot every ... seconds
Music + SFX:  style, how loud under the voice
End card:     my name / logo / call to action
Never:        ...
```

---

Made by Web Lab. Follow @weblabai for one of these every day.
The full build files (templates, tools and the brand kit) are inside Web Lab Academy.
