# loc-tracker

Automatically counts lines of code across all my public GitHub repositories, excluding professional work.

## What it does

A GitHub Action runs daily, clones all public repositories, counts lines of code using `cloc`, and saves the result to `stats.json`. This file is consumed by my portfolio to display a live personal LOC count.

## How it works

- GitHub Action triggers daily
- Clones all public repos
- Runs cloc across all repos
- Saves results to stats.json
- Auto commits and pushes

## Live Data URL

https://raw.githubusercontent.com/DivakarVelagacherla/loc-tracker/main/stats.json

## Note

Only **personal public repositories** are counted. Professional work at Vanguard and Cognizant is not included.
