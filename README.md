# Cooking Animation Skill

Makes Anime cooking ASMR short films from a recipe, following the workflow proven in the Basque burnt cheesecake test film (October 2026).

## What it does

- Locks one Anime style, one character sheet and one kitchen set for the whole film.
- Builds the film in phases, with an approval gate at the end of every phase. Never advance without approval.
- Phase 2: chronological scene breakdown, 8 scenes x 10 seconds.
- Phase 3: one image prompt per scene, in its own JSON block.
- Phase 4: one video motion prompt per scene, in its own JSON block.
- Poster (Step 4): one master poster prompt, 4-layer parallax, 9:16.
- SEO (Step 5): Vietnamese, Mobile First, 5 items, each in its own code block.
- Render: Muse first within the weekly token allowance; Google Flow as fallback (see `references/render-rules.md`).

## Files

- `SKILL.md` — the operating instructions. Muse reads this first.
- `skill.yaml` — name, title, description and category.
- `references/` — character sheet, phases, the Basque example, Phase 3 and Phase 4 prompts, poster rules, SEO rules, render rules and short commands.

## Load it

After the files are on GitHub as a Public repository, load the whole package with one command in a new chat:

```
Nạp Skill này (<link zip>) và cùng làm việc bạn nhé!
```

Replace `<link zip>` with the real zip link of the Public repository, in the form `https://github.com/<account>/<repo>/archive/refs/heads/main.zip`. Do not use a guessed link. Check first that the downloaded zip contains `SKILL.md`, `skill.yaml` and `references/`.

## Version

- v1.0 — draft, 31/10/2026 — packaged from the side-chat Basque workflow, awaiting the owner's approval before GitHub upload.
- This skill shares the workflow only. It does not include the Basque test video, and it does not publish any film.
