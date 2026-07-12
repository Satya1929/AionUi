@AGENTS.md

<!-- SYNC:BEGIN brain -->
## Second brain (hub-and-spoke)
- Before researching any fact, decision, client detail, or playbook: run
  python "C:\Users\ASUS\Desktop\Satya\Projects\Fable5\brain\brain.py" find "<question>"
  It deterministically searches THIS project's BRAIN_INDEX.md, the Fable5 hub, and all sibling
  projects — and returns one section of evidence (~400 tokens, zero model calls). Only fall back
  to Grep/Read sweeps after it prints NOT FOUND, and then store what you learned:
  python "C:\Users\ASUS\Desktop\Satya\Projects\Fable5\brain\brain.py" remember <slug> "<one-liner>" --type knowledge --body "<fact>"
- After adding or moving docs in this project, refresh its spoke index:
  python "C:\Users\ASUS\Desktop\Satya\Projects\Fable5\brain\brain.py" index "<this project root>"
- Master doctrine (routing, verification, standing rules): Fable5/brain/FABLE_MODE.md.
- Full refresh (all spokes + lint + map): python "C:\Users\ASUS\Desktop\Satya\Projects\Fable5\brain\update.py"
<!-- SYNC:END brain -->
