# What I Did Today
Referenced the claude slash command /what-i-did-today

02/08/26 (last checked 21:21):
- **macros**: Added Comet window focusing to website hotkeys and switched tab switching to use RShift modifier.
- **slash commands**: Created `/update-skill` command that reviews session corrections and bakes them into skill prompts, including capturing verification prompts as signals for missing validation steps. Refined it to list identified skills/commands first for confirmation, and to distinguish between skills and commands that may live in different directories. Updated `/what-i-did-today` to use a `scan-repos.sh` script (bypassing Claude Code's shell-operator permission limitation), added last-checked timestamps to avoid re-fetching old commits, and made bullet descriptions more detailed for repos with many changes.
- **rec-system-folder**: Connected repo to GitHub remote, pushed initial commit, and created an AHK script for RShift+Arrow browser tab reordering in Comet.

02/07/26:
- **yc_application**: Built the full YC application from scratch — initial draft, refined answers, added Sidequest details, wrote a pitch script with market stats and role assignments.
- **rec-system-folder**: Initialized the repo with a recommendation.md technical plan and .gitignore.
- **career-search**: Reorganized files into ultralearning folder and updated Phase 1-2 project plans with concrete rec sys tasks (Goodreads-10K, Two-Tower model, FastAPI demo, etc.).
- **macros**: Modularized AutoHotkey scripts into separate files with a main.ahk launcher, extracted the Explorer hotkey into its own script, built a triple-p "commit and push" macro and triple-l "git pull origin main" macro, moved scripts into a scripts/ subfolder, and configured Claude Code permissions for auto-allowed commands.
- **slash commands**: Updated /what-i-did-today to output one bullet per repo instead of a single sentence, check for existing date sections before adding duplicates, and insert newest entries at the top.
- **lunar-lander-file-folder**: Wrote the entire project README, then fixed GitHub display — discovered GitHub's blob viewer doesn't render MP4 files, uploaded the training video as an issue attachment for inline playback, moved the README to the repo root so GitHub displays it, and cleaned up loose files (removed duplicate video, moved sweep log to logs/, deleted empty test1.py).
- **macros**: Added Shift+Arrow Comet browser tab switching, text expansion hotstrings, smart copy, #SingleInstance Force, faster Explorer navigation, renamed notion-hotkeys to website-hotkeys with Win+6 for GitHub repos.
- **northeastern_university_folder**: Edited Project 5 VSD analysis with anti-AI-detection tone guidelines. Solved MetaCTF 3 challenges (Barry's Web Application directory traversal, Back to the Future User-Agent/cookie bypass) with runnable scripts and writeups; updated meta_ctf skill with tone enforcement section, script workflow rules, backtick ban, and logical completeness verification; added 3 new tone guidelines (discovery order, no technical justifications, broadened First/Second/Third rule); updated /update-tone-style-guidelines command to require completing all identified patterns; created ~/.claude/CLAUDE.md to disable co-author in commits.
