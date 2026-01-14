# Stroll Athens Patch Pack (Locked Build)

This pack is designed specifically for your locked baseline: `stroll-settings-memories-truefix.zip`.

## What it contains
- `routes.json` (updated): your existing routes plus 5 new Athens routes (A–E)
- `scripts/` (new files only): narration text files for every Athens stop

## How to apply (Git repo)
From your Stroll repo root:

```bash
unzip stroll-athens-patch-pack.zip -d /tmp/athens_patch
cp /tmp/athens_patch/routes.json ./routes.json
cp -R /tmp/athens_patch/scripts ./scripts

git add routes.json scripts
git commit -m "Add Athens (Tours A–E) content"
git push
```

## How to apply (if you only have the ZIP build)
1) Unzip your locked build somewhere
2) Copy `routes.json` to the root
3) Copy the new `scripts/*.txt` into the existing `scripts/` folder
4) Re-zip for distribution (optional)

Notes:
- No runtime JS/CSS changes are required. The app auto-builds the city list from `route.city`.
- Athens will appear automatically in the City selector.
