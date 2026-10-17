---
name: micro-drama
description: Start or continue the user's serialized micro-drama workflow in VideoExpress. Trigger when the user says “StartMicroDrama,” asks to begin a micro-drama project, or resumes one; load the user's canonical GitHub system prompts first. Keep VideoExpress as the video production app.
---

# Micro Drama Startup

Use this skill when the user says **StartMicroDrama** (including capitalization or punctuation variations; internal whitespace is significant), or clearly asks to start/resume the user's micro-drama workflow.

## Load the canonical rules

1. Read the latest `SYSTEM_PROMPT.md` and `VIDEO_EDITING_SYSTEM_PROMPT.md` from `https://github.com/akinluyigithub/micro-drama-system-prompt` before starting a new project. Prefer the local clone at `C:\Users\ak\OneDrive\Documents\1 - VideoExpress\micro-drama-system-prompt` and fast-forward it from `origin/main`; if unavailable, fetch/read the two raw GitHub files.
2. Follow those prompts as the source of truth. Continue without asking what the trigger means.
3. Use only VideoExpress for video animation, editing, captions, audio, timeline, and export. The still-image generation route is selected per project as specified in the system prompt.
4. For every video prompt, use the same ordered, fully populated section format specified in `VIDEO_EDITING_SYSTEM_PROMPT.md`; retain all headings and mark inapplicable sections explicitly.

## Start the project

- Make the browser action an actual tool call, not just an instruction: immediately after reading the prompt, use `mcp__cua_repl.js` with `cua.getTab({ url: "https://app.videoexpress.ai/" }, { browser: "iab" })`. If there is no matching tab, call `cua.createBrowserTab("iab", "https://app.videoexpress.ai/", { visible: true })`. Do this before waiting for search results; dispatch research agents first if used, then focus the browser while they work. Verify the URL, loaded app UI, and signed-in account indicator. Never close the VideoExpress tab as cleanup; leave it open across turns and after project completion, and reuse it later. Reopen it if missing. The tab cannot persist beyond a user-closed Codex/browser session. If CUA is unavailable, use Codex `open_in_codex` with this exact browser URL. Stop and report any login/access gate; do not generate before approval.
- Before any concept recommendation or refinement, run the system prompt's live trend scan. Search at least three accessible areas, prioritizing TikTok, YouTube Shorts, and Instagram Reels; target 60–90 seconds and stop by two minutes. Cite sources, separate observed signals from interpretation, and disclose access gaps. Use up to two agents only if they improve coverage/speed; otherwise browse directly. Then preserve a user-supplied story or provide the structured recommendation menu; never invent viral metrics.
- Keep the concept choice interactive across turns: if the user selects a genre alternative, create a full story concept in that style and ask for the next easy choice; if they ask for “something else,” offer A another premise in the same style, B a different style, C their own story. Never stop at an alternative list or require a restart. Continue until a concrete premise is approved, their own story is supplied, or they explicitly stop.
- Once the title is established, create a dedicated folder named after the project inside the current workspace. Keep that project's scripts, assets, prompt book, and continuity notes there. Reuse it when continuing the same project; don't overwrite unrelated project folders.
- Follow the system prompt's two checkpoints: concept, then consolidated brief including the image-generation route. Keep answers and follow-up questions easy to respond to with numbered choices.
- Once an episode package is approved, follow the standing authorization and complete routine production in VideoExpress without per-asset approval requests. Ask only for a genuine blocker or material change.
