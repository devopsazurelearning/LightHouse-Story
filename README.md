# The Lighthouse Keeper

A small static website that tells a short story. It is a practice project for Azure Boards, Azure Pipelines and GitHub.

## Files

- `index.html`: the story page (starts with only Chapter 1)
- `styles.css`: minimal starter styles
- `STORY.md`: text for Chapters 2 and 3
- `BACKLOG.md`: the Epic, Features, User Stories and Bug to create in Azure Boards

## Run it locally

Open `index.html` in your browser. No build step is needed.

## Push to GitHub

1. Create an empty repository on GitHub named `lighthouse-story` (no README, no .gitignore).
2. In this folder run:

```bash
git init
git add .
git commit -m "Initial commit: starter story page"
git branch -M main
git remote add origin https://github.com/<your-user>/lighthouse-story.git
git push -u origin main
```

## Connect to Azure DevOps

1. In your Azure DevOps project, go to Project settings > GitHub connections and connect this repository, so commits with `AB#<id>` link to work items.
2. Create the work items from `BACKLOG.md`.
3. Make changes on a branch, commit with `AB#<id>`, open a pull request on GitHub, and check that the work item shows the commit and pull request under Development.
