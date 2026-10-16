---
name: micro-drama
description: Start or continue the user's serialized micro-drama workflow in VideoExpress. Trigger when the user says “Start Micro Drama,” asks to begin a micro-drama project, or resumes one; load the user's canonical GitHub system prompts first. Keep VideoExpress as the video production app.
---

# Micro Drama Startup

Use this skill when the user says **Start Micro Drama** (including capitalization or punctuation variations), or clearly asks to start/resume the user's micro-drama workflow.

## Load the canonical rules

1. Read the latest `SYSTEM_PROMPT.md` and `VIDEO_EDITING_SYSTEM_PROMPT.md` from `https://github.com/akinluyigithub/micro-drama-system-prompt` before starting a new project. Prefer the local clone at `C:\Users\ak\OneDrive\Documents\1 - VideoExpress\micro-drama-system-prompt` and fast-forward it from `origin/main`; if unavailable, fetch/read the two raw GitHub files.
2. Follow those prompts as the source of truth. Continue without asking what the trigger means.
3. Use only VideoExpress for video animation, editing, captions, audio, timeline, and export. The still-image generation route is selected per project as specified in the system prompt.

## Start the project

- If the user supplies a story with the trigger, use it. Otherwise, offer up to three concise original concepts, recommend one, and finish with an easy numbered option for **“I have my own story.”** Help shape a rough story idea without a long questionnaire.
- Once the title is established, create a dedicated folder named after the project inside the current workspace. Keep that project's scripts, assets, prompt book, and continuity notes there. Reuse it when continuing the same project; don't overwrite unrelated project folders.
- Follow the system prompt's two checkpoints: concept, then consolidated brief including the image-generation route. Keep answers and follow-up questions easy to respond to with numbered choices.
- Once an episode package is approved, follow the standing authorization and complete routine production in VideoExpress without per-asset approval requests. Ask only for a genuine blocker or material change.
