# GitHub Setup

## Before release

This repository includes an unpublished research handbook. Keep the repository **private at first** and confirm with the supervisor what may be shared publicly. If the handbook should not be shared, remove `docs/source/CAVE_EoT_Research_Handbook.pdf` and replace it with a public-safe overview.

## Create the remote repository

1. Extract this archive.
2. Create an empty GitHub repository named `cave-eot-literature-review`. Do not initialize it with an additional README.
3. In a terminal opened in the extracted folder, review files before committing:

```bash
git init -b main
git status
git add README.md docs literature .gitignore
git status
git commit -m "Add CAVE-EoT literature review and research design"
git remote add origin https://github.com/Oussam-beep/cave-eot-literature-review.git
git push -u origin main
```

4. Check the repository after pushing. Verify Markdown preview, relative links, CSV rendering and PDF access.
5. Only switch to public after supervisor approval and a final disclosure review.

## What this repository intentionally does not claim

It does not claim a running CAVE-EoT implementation, completed experiments or performance results. Those belong in later commits once the work has actually been implemented and evaluated.
