---
layout: default
title: 30-Day Challenge
description: Offline iOS challenge tracker with JSON-powered custom challenges.
---

# 30-Day Challenge

![30-Day Challenge App Icon](assets/images/app-icon.png)

**An offline, notebook-style iOS app for 30-day self-improvement challenges.**  
Create, import, and track fully local challenge packs with no internet required.

[View source on GitHub](#get-the-code) · [Challenge format](#challenge-package-format) · [GitHub Pages setup](#publish-with-github-pages) · [Terms of Use](./terms) · [Privacy Policy](./privacy-policy) · [Support](./support)

## Why this app stands out

- **Fully offline** — no internet, analytics, or cloud dependency
- **JSON-powered** — add new 30-day challenges without changing the app architecture
- **Notebook-style UI** — warm paper design with a focused daily journaling flow
- **Multilingual-ready** — translations and labels are driven by challenge JSON
- **Custom habit tracker** — configurable columns for any challenge type
- **Built for creators** — package and publish your own challenge libraries

## Core features

### Daily notebook workflow
Each day includes:
- Morning checklist
- Afternoon checklist
- Evening checklist
- Today’s challenge
- Reflection prompts
- Notes and progress scoring

### Local-first challenge library
Install multiple challenge packs and switch between them directly in the app.

### Import your own challenges
Users can import `.json` challenge files from Files, AirDrop, shared links, and cloud storage providers supported by iOS.

### Flexible scoring and tracking
Track values like:
- Sleep
- Focus
- Mood
- Energy

Or redefine them for any challenge, such as money, fitness, prayer, study, or productivity.

## Included challenge ideas

The current project already shows how the format can support multiple themes:

- Brain upgrade / self-improvement
- Spending tracker / money challenge
- Indonesian and English challenge packs

That means the same app structure can power many downloadable challenge products.

## Best use cases

This app can be positioned as:

- a **30-day habit challenge app**
- a **guided journal app**
- a **self-improvement tracker**
- a **money tracking challenge app**
- a **faith, reading, health, or study challenge platform**

## App architecture summary

```text
SwiftUI app
├── App/                 Entry point + Info.plist
├── Models/              Challenge, day, checklist, scoring models
├── ViewModels/          Business logic + persistence
├── Views/               Home, detail, tracker, settings, library
├── Utilities/           Design system and reusable UI helpers
└── Resources/           Challenge JSON packages + assets
```

## Challenge package format

Every challenge is a single `.json` file.

```json
{
  "id": "my-challenge-v1",
  "version": "1.0",
  "language": "en",
  "metadata": {
    "title": "My 30-Day Challenge",
    "subtitle": "A subtitle",
    "author": "Author Name",
    "description": "What this challenge is about.",
    "durationDays": 30,
    "createdDate": "2026-01-01",
    "tags": ["health"],
    "labels": {
      "morning": "Morning Checklist",
      "afternoon": "Afternoon Checklist",
      "evening": "Evening Checklist",
      "todayChallenge": "Today's Challenge",
      "reflection": "Reflection"
    }
  },
  "coreRules": ["Rule 1", "Rule 2"],
  "habitTrackerColumns": ["Sleep", "Exercise", "Reading"],
  "days": []
}
```

### What this enables

- You can launch **new 30-day products** without rebuilding the app UI
- You can localize the experience by changing JSON labels and content
- You can create downloadable packs for niches like finance, prayer, studying, fitness, or parenting

## For app creators

This project is especially useful if you want to:

1. Build one iOS app shell
2. Sell or distribute multiple challenge packs
3. Support multiple languages
4. Keep all user data local on-device

## Get the code

Place your Xcode project in the same repository or link this site to your app repository.

Suggested repo structure:

```text
your-repo/
├── docs/                 GitHub Pages website
├── ThirtyDayChallenge/   iOS source code
└── README.md
```

## Publish with GitHub Pages

GitHub Pages can publish a site from a branch or from a `/docs` folder in your repository, and Markdown works well with Jekyll.

### Recommended setup

1. Create a GitHub repository for the app
2. Add this website inside a `docs/` folder
3. Push your code to GitHub
4. In **Settings → Pages**, choose:
   - **Source:** Deploy from a branch
   - **Branch:** `main`
   - **Folder:** `/docs`
5. Save and wait for the site URL to appear

If you publish from a source branch, Jekyll builds the site by default.

## Suggested copy for the homepage hero

> Build better habits in 30 days — fully offline, beautifully simple, and customizable with your own challenge packs.


## Legal & support

For App Store review and user support pages:

- [Terms of Use](./terms)
- [Privacy Policy](./privacy-policy)
- [Support](./support)

## Roadmap ideas

- App screenshots section
- Download / TestFlight section
- Privacy policy page
- Challenge marketplace page
- Documentation for building custom JSON packs
- FAQ for import and translations

## License

MIT
