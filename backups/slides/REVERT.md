# Slide Backup Revert Protocol

Backups live under `backups/slides/[slide-id]/`. Full-deck snapshots live under `backups/full/`.

## Naming

Slide backups use `YYYYMMDD-HHMMSS-pre-[description].html`. Each backup starts with an HTML comment containing timestamp, slide id, and short description.

## Manifest

`backups/slides/_index.json` maps each slide id to backup rows:

```json
{
  "cs-frontier-iconic": [
    {"timestamp": "20260514-140530", "description": "pre-exploration", "file": "backups/slides/cs-frontier-iconic/20260514-140530-pre-exploration.html"}
  ]
}
```

## Manual Revert Recipe

1. Save the current slide first using the same backup protocol.
2. Open the desired backup file.
3. Ignore the first HTML comment line.
4. In `GnR_deck.html`, replace the full `<div class="casey-slide" id="[slide-id]">...</div>` block with the backup block.
5. Copy `GnR_deck.html` to the deploy mirror as both `GnR_deck.html` and `index.html`.
6. Commit and push from the deploy mirror.
