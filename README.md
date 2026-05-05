# stats-tracker

Automatically tracks coding stats across all my public GitHub repositories and LeetCode.

## What it tracks

- **Lines of Code** — across all public repos using `cloc`
- **Total Repos** — public repository count
- **Total Commits** — contributions across all repos
- **Total PRs** — pull requests authored
- **LeetCode Stats** — problems solved by difficulty + ranking

## How it works

- GitHub Action triggers daily
- Clones all public repos
- Runs cloc across all repos
- Fetches GitHub stats via API
- Fetches LeetCode stats via GraphQL
- Saves everything to stats.json
- Auto commits and pushes

## Live Data URL

https://raw.githubusercontent.com/DivakarVelagacherla/loc-tracker/main/stats.json

## Note

Only **personal public repositories** are counted. Professional work at Vanguard and Cognizant is not included.
