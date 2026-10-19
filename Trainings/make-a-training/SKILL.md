---
name: make-a-training
description: Turn a routine into a training the team follows the same way every time. Use when the owner asks to teach the team a procedure.
---
1. Only when the owner asked for this in this session. Never in a shift.
2. Ask the owner which routine, or read the `How We Work/` note they name.
3. Write it as short numbered steps: what to read, what to write, what never to do. Drafts only; nothing is sent.
4. Pick a name: lowercase words joined by dashes, 40 letters at most, never the name of a built-in training (CLAUDE.md lists them). Write a one-sentence description of when to use it, starting with a letter or number, with no colon and none of these marks: { } [ ] & * ! | > % @ ` #.
5. Write a task note in `Team/Tasks/` with `status: Needs you`, `kind: training`, `name`, `title` (the description) and the steps in the body.
6. Show the owner the whole training exactly as it will be saved, say whether it is new or replaces one, and ask "Add this training?" Wait for the answer. The saved text is exactly:
   ```
   ---
   name: <name>
   description: <description>
   ---
   <the numbered steps>
   ```
   Nothing else goes in the top block, and the steps never use an exclamation mark right before a backtick.
7. If the owner says yes, write that exact text with the Write tool, as a whole file, first to `Trainings/<name>/SKILL.md` (the copy the owner reads) and then to `.claude/skills/<name>/SKILL.md` (the copy the team uses). Claude asks the owner to approve each file.
8. If the owner says no or denies a file, stop. Read back both places, tell the owner exactly which copy was saved and which was not (the training works only once the team's copy is saved), save (Saving in CLAUDE.md), and leave the task note as `status: Needs you`.
9. When both copies are saved: save (Saving in CLAUDE.md), set the task note to `status: Done`, use the training once, and show the owner the result.
