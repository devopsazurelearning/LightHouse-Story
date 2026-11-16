# Backlog for Azure Boards (Agile process)

Create these work items in Azure Boards, then link each User Story to its Feature and each Feature to the Epic.
Work in a branch per story and put `AB#<id>` in every commit message so the commit links to the work item.

## Epic

**Publish "The Lighthouse Keeper" as a readable story website**

## Feature 1: Story structure

| Type | Title | Acceptance criteria |
|---|---|---|
| User Story | As a reader, I can see the story title and a short subtitle | One `<h1>` with the title; subtitle paragraph below it |
| User Story | As a reader, I can read Chapter 2 | `<h2>` heading and two paragraphs from STORY.md, in a new `<section id="chapter-2">` |
| User Story | As a reader, I can read Chapter 3 | `<h2>` heading and two paragraphs from STORY.md, in a new `<section id="chapter-3">` |
| Task (under each chapter story) | Add the HTML section | Valid HTML, correct heading level |
| Task (under each chapter story) | Check the page in a browser | No layout errors |

## Feature 2: Typography

| Type | Title | Acceptance criteria |
|---|---|---|
| User Story | As a reader, I see headings in a storybook serif font | Heading font set for `h1` and `h2`; fallback fonts defined |
| User Story | As a reader, I see body text in a comfortable reading font | Body font, size of at least 18px, line height of at least 1.6 |
| User Story | As a reader, the text width is easy to read | Content centred, maximum width around 65 characters |

## Feature 3: Navigation and polish

| Type | Title | Acceptance criteria |
|---|---|---|
| User Story | As a reader, I can jump to any chapter from a menu | Nav links at the top that scroll to each chapter |
| User Story | As a reader, I see a footer with the author and year | Footer at the bottom of every page |
| User Story | As a reader on a phone, the page fits my screen | No horizontal scrolling at 375px width |

## Bug (seeded on purpose)

| Type | Title | Repro steps | Expected |
|---|---|---|---|
| Bug | Subtitle contains a spelling mistake | Open `index.html` and read the subtitle | "lighthouse" is spelled correctly |

## Suggested order

1. Create the Epic, the three Features and the User Stories, then link them.
2. Create Tasks under the stories you start first.
3. Fix the bug first (smallest change) to practise the full flow: work item, branch, commit with `AB#`, pull request, close.
4. Then work through Feature 1, Feature 2 and Feature 3.

## Branch and commit examples

```bash
git checkout -b feature/AB#12-chapter-2
git add index.html
git commit -m "AB#12 Add chapter 2 to the story"
git push origin feature/AB#12-chapter-2
```

Use your real work item number in place of 12.
