# Codex Parallel Deck Workflow

1. Run many new Codex sessions only in Worktree mode.
2. Paste `prompts/CODEX_PARALLEL_DECK_TASK_PROMPT.txt` into each session.
3. Add the exact edit request at the bottom.
4. Each session must produce a `deck/[task]` branch and commit.
5. Later, one Local integration session merges completed branches and mirrors `GnR_deck.html` to `index.html`.

Never run multiple Local edit sessions at once.

Do not edit the old `pitch_visuals` copy during parallel work.

Do not push until integration/publish.
