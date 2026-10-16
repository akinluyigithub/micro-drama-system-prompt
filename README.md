# Micro Drama System Prompt

A reusable workflow for original serialized micro-dramas, with all video generation and production performed in VideoExpress AI.

## What this repository contains
- `SYSTEM_PROMPT.md`: reusable showrunner and production instructions, including the per-project still-image route choice.
- `VIDEO_EDITING_SYSTEM_PROMPT.md`: VideoExpress editing instructions for English regional voice direction, captions, title cards, audio, and delivery.
- `audio-library/`: reusable original WAV music tracks stored with Git LFS, plus a track index with provisional filename-based cues.
- This README: setup and operating notes.

## Start a new series
1. In a new chat, type **Start Micro Drama**. The installed Codex skill loads the latest prompts from this repository and starts the workflow. At the same time as the trend scan begins, it opens or focuses `https://app.videoexpress.ai/` in Codex's built-in browser and verifies the app is loaded. On a device without the skill, load `SYSTEM_PROMPT.md` and `VIDEO_EDITING_SYSTEM_PROMPT.md` first.
2. Before recommending a story, the agent performs a time-boxed live scan of at least three accessible trend sources, prioritizing TikTok, YouTube Shorts, and Instagram Reels, then cites observed signals and access gaps. The scan targets 60–90 seconds and stops by two minutes. If you have not supplied a story, the agent presents one detailed lead recommendation, lettered alternatives, and a numbered choice board ending with **I have my own story**. A rough story seed is enough.
3. Confirm or revise the premise.
4. Review and approve one consolidated project brief (cast, visual treatment, language, image-generation route, episode batch and cliffhangers).
5. Review each episode's complete text package before image/video generation.
6. Approve the episode text package. For this user, that approval authorizes end-to-end production in VideoExpress: all needed portrait references and clips, timeline assembly, save, export, and download when requested. No per-asset check-ins are required.
7. The agent completes the approved episode in VideoExpress and reports the export status.

## Production principles
- VideoExpress AI is always used for video animation, editing, speech/audio, timeline, and export. For still images, the user chooses ChatGPT Advanced Image Model or Video Express AI once per project. No other image/video generators or external editing services are used.
- Use vertical 9:16 for all episode references, storyboard images, clips, timeline, and final exports unless the user explicitly changes that preference. Verify dimensions in the app or file metadata.
- Do not publish or share a video unless explicitly requested.
- Verify controls and limits from the live Video Express interface. Do not assume source-repository settings still match the current application.
- Create a separate project folder in the current workspace named after each approved project title. Keep story canon, approved references, episode state and prompt book there so later episodes preserve continuity.
- Do not claim an asset was generated, saved, reviewed, or exported unless the app confirms it.

## Source playbooks studied
- [Historical documentary workflow](https://github.com/ai-playbooks/historical-documentary-video-workflow)
- [Slow English learning videos workflow](https://github.com/ai-playbooks/slow_english_learning_videos)

These are references for browser-based Video Express workflows. Their CloneVoice dependency and their specific historical/children's-video formats are intentionally excluded from this project.
