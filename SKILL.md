# Cooking Animation Skill

## When this skill applies

- Use this skill when the user asks to make an Anime cooking ASMR short film, in 9:16, from a recipe and a main character.
- Work in Vietnamese with the user. Keep technical prompts, JSON fields and style locks in English, exactly as in the references.
- This skill is a workflow only. It does not publish a film, does not post to YouTube, Facebook or TikTok, and does not share a video file outside the user's own workspace unless the user explicitly asks for that step.

## Style lock — never change mid-film

Paste this exact lock into every image and every shot, and never mix it with another style in the same film:

```
STYLE LOCK: anime style, large expressive eyes, strong emotional acting, cinematic colours, clean outlines. Keep this exact style in every image and every shot. No 3D, no Pixar look, no photorealism.
```

- 3D Pixar Style is excluded. Do not use it.
- Do not mix hyper-realistic food photography with Anime in one film. If the source master prompt is hyper-realistic, adapt it to Anime first, before any render.
- One kitchen set for the whole film: warm morning kitchen, dark oak wooden table, stable warm light. One pan or bowl where the recipe allows, so the dish stays continuous.

## Character lock

- Read `references/character-sheet.md` before proposing any scene.
- If the user has an existing character from an older channel, compare the sheet with that character first. If fur, hat or apron differ, stop and ask the user to correct the sheet before rendering. Never render scenes with a wrong sheet.
- Character continuity across video scenes: chain by last frame. Once a last frame exists, do not add a separate close-up face reference for that character.
- If a rendered frame drifts (wrong face, wrong outfit, wrong dish or packaging), do not deliver the drifted version. Re-render that scene.

## Phases and approval gates

Work in this order, and stop at the end of every phase for approval. Never advance without approval.

### Phase 1 — Recipe and format lock

- Confirm: recipe, one pan or dish, channel, format 8 scenes x 10 seconds = 80 seconds, 9:16, Anime, ASMR first.
- Dialogue for a pure ASMR film stays minimal: 1 opening line + 1 closing line, in Vietnamese. Cooking sounds dominate. If the user wants full dialogue throughout, that is a cooking story film, not pure ASMR — confirm the change before writing the script.

### Phase 2 — Scene breakdown

- Write 8 chronological scenes that follow the real cooking order. Do not force a step the recipe does not have.
- Example structure, from the Basque film in `references/basque-example.md`: line the pan, beat, pour, sift and stir, pour into the pan, put in the oven, reveal the baked dish, slice and taste.
- For each scene give: time range, action, and the ASMR sound of that action (paper rustling, pouring, whisking, tapping the pan, oven door, slicing, spoon scooping).

### Phase 3 — Image prompts

- Read `references/phase3-image-prompts.md` for the format.
- One scene = one separate JSON block, fields: `scene_number`, `shot_type`, `subject`, `background`, `aesthetic`, `aspect_ratio: "9:16"`.
- Make the character sheet first, with 4 views, before the 8 scene prompts.

### Phase 4 — Video motion prompts

- Read `references/phase4-video-prompts.md` for the format.
- One scene = one separate JSON block, fields: `camera_motion`, `action`, `motion_style`, `style`.
- Camera: static overhead or gentle micro-zoom only, one camera move per shot. Motion must be gravity-driven and continuous: pouring, whisking, sifting, tapping, jiggling, slicing. No floating objects, no morphing.

### Poster — Step 4

- Read `references/poster-step4.md`.
- Output exactly one master poster prompt, in one code block, 9:16.
- 4-layer parallax, title as a physical 3D event in the top mobile safe zone, subtitle beneath it. No real paper currency in posters.
- Single Reference Lock: `@` references appear only once each, only in the `[INPUT ASSETS & CHARACTER BINDING]` block. The rest of the prompt uses pure names only.
- Present the poster for approval before rendering scenes.

### SEO — Step 5

- Read `references/seo-step5.md`.
- Pure Vietnamese, Mobile First. Title under 42 characters including `#Shorts`, exactly one hashtag `#Shorts`, no series labelling such as "Tập 1/Tập 2".
- Package with exactly 5 items, each in its own separate code block: (1) SEO video filenames, (2) 3 title options, (3) SEO description with AI transparency, (4) core channel keywords, (5) pinned comment.
- Export the Word file named `05_SEO_Phat_Hanh_[Ten_Phim_Khong_Dau].docx` when the user asks for the file version.

## Render rules

Read `references/render-rules.md` in full before rendering anything.

- Muse first, only within the weekly token allowance. If Muse video returns a region restriction (for example 403 `video_not_available`), stop using that tool for the film. Do not retry it, and do not create an account or pay for a workaround.
- Google Flow fallback: render 360p, download upscaled to 720p. Render scenes in order, one at a time. Verify the real downloaded file exists, is about 10 seconds and 720x1280, before starting the next scene. If Flow credit runs out, report to the user for another account.
- Final assembly, when the user asks for it: pad each scene to exactly 10.000 seconds, concatenate, and re-encode Android-safe: `-vf format=yuv420p -c:v libx264 -profile:v high -level 4.0` plus `-c:a aac -b:a 128k -ar 48000 -ac 2 -movflags +faststart`. Verify with ffprobe (duration, 720x1280 or 1080x1920 as agreed, yuv420p, AAC stereo 48kHz, faststart) before delivering. Give every new final version a new filename.
- A test clip is not a final film. If the user only asks for a test, do not assemble the full film, do not upload it, and do not post it.

## Short commands

Read `references/bo-lenh-ngan.md` before proposing anything. Build every output from those commands, and name the command used.

## Verification before sharing

- Run the skill once in a brand-new chat on a real recipe. Compare the result with the Basque example.
- Checklist: skill runs all phases without asking again for what is already locked; result matches the locked style, character and kitchen; short commands work; no error repeats on a second consecutive run.
- Do not share the skill until the test run passes. Record the version and date on every change, and keep one original copy only.
- Never put a password or token inside a skill file. A GitHub token, if ever needed for upload, is used once and deleted immediately, and never pasted into the skill or sent to anyone else.
