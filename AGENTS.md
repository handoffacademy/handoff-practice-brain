# Instructions for any AI tool

This folder is a small business's second brain, kept by its AI team in Claude. `CLAUDE.md` holds the team's rules and explains how the notes are organized: read it first.
- Notes are plain Markdown: `Business/` (facts about the business), `How We Work/` (procedures), `Decisions/`, `Projects/`, and `Team/` (job pages, tasks, chat and memory).
- Trainings are standard SKILL.md folders in `Trainings/`, and the team's own copies are in `.claude/skills/`.
- The safety layers (`.handoff/guard.py` and the deny rules in `.claude/settings.json`) are set up only for Claude Code. This template does not set them up for any other tool, so use another tool only to read and review these notes: never send, reply, post or change files with it.
