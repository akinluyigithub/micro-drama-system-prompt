# Micro Drama System Prompt

A Video Express AI only workflow for original serialized micro-dramas.

## What this repository contains
- `SYSTEM_PROMPT.md`: reusable showrunner and production instructions for planning and producing original serialized micro-dramas entirely in Video Express AI.
- `VIDEO_EDITING_SYSTEM_PROMPT.md`: Video Express-only instructions for editing, English regional voice direction, captions, title cards, audio, and delivery.
- `audio-library/`: reusable original WAV music tracks stored with Git LFS, plus a track index with provisional filename-based cues.
- This README: setup and operating notes.

## Start a new series
1. Give the agent a story seed, or ask it to recommend a drama tradition, title, and premise.
2. Confirm or revise the premise.
3. Review and approve one consolidated project brief (cast, visual treatment, language, episode batch and cliffhangers).
4. Review each episode's complete text package before image/video generation.
5. Approve the episode text package. For this user, that approval authorizes end-to-end production in Video Express AI: all needed portrait references and clips, timeline assembly, save, export, and download when requested. No per-asset check-ins are required.
6. The agent completes the approved episode in Video Express and reports the export status.

## Production principles
- Video Express AI is the only image, video, speech, audio, timeline, and export application in this workflow. Do not use CloneVoice, external image/video generators, APIs, or other editing services.
- Use vertical 9:16 for all episode references, storyboard images, clips, timeline, and final exports unless the user explicitly changes that preference. Verify dimensions in the app or file metadata.
- Do not publish or share a video unless explicitly requested.
- Verify controls and limits from the live Video Express interface. Do not assume source-repository settings still match the current application.
- Keep story canon, approved references, episode state and prompt book together so later episodes preserve continuity.
- Do not claim an asset was generated, saved, reviewed, or exported unless the app confirms it.

## Source playbooks studied
- [Historical documentary workflow](https://github.com/ai-playbooks/historical-documentary-video-workflow)
- [Slow English learning videos workflow](https://github.com/ai-playbooks/slow_english_learning_videos)

These are references for browser-based Video Express workflows. Their CloneVoice dependency and their specific historical/children's-video formats are intentionally excluded from this project.
