---
layout: default
title: 30-Day Challenge
description: Offline iOS challenge tracker with customizable 30-day challenge packs.
---

<div style="text-align:center; padding: 1rem 0 0.5rem 0;">
  <img src="assets/images/app-icon.png" alt="30-Day Challenge App Icon" width="140" style="border-radius: 28px; box-shadow: 0 12px 30px rgba(0,0,0,0.12);">
</div>

<h1 style="text-align:center; margin-bottom:0.4rem;">30-Day Challenge</h1>
<p style="text-align:center; font-size:1.15rem; max-width:760px; margin:0 auto 1rem auto;">
Build better habits in 30 days — fully offline, beautifully simple, and customizable with your own challenge packs.
</p>

<p style="text-align:center; margin-bottom:1.5rem;">
  <a href="#why-it-works"><strong>Why it works</strong></a> ·
  <a href="#features"><strong>Features</strong></a> ·
  <a href="#challenge-packs"><strong>Challenge packs</strong></a> ·
  <a href="#for-creators"><strong>For creators</strong></a> ·
  <a href="./privacy-policy"><strong>Privacy</strong></a> ·
  <a href="./terms"><strong>Terms</strong></a> ·
  <a href="./support"><strong>Support</strong></a>
</p>

<div style="background: linear-gradient(180deg, #fffaf3 0%, #fff 100%); border:1px solid #f0e3cf; border-radius:20px; padding:1.4rem; margin: 1rem 0 2rem 0; box-shadow: 0 10px 25px rgba(0,0,0,0.05);">
  <h2 style="margin-top:0;">A local-first iOS app for journaling, habits, and guided 30-day programs</h2>
  <p>
    30-Day Challenge is designed for creators, coaches, and self-improvement brands that want a simple mobile app shell
    powered by reusable JSON challenge packs. Users can install challenge content, track progress, write reflections,
    and stay focused without needing an account or internet connection.
  </p>
  <p style="margin-bottom:0;">
    <strong>Best fit for:</strong> self-improvement, budgeting, prayer, studying, productivity, reading, wellness, and lifestyle programs.
  </p>
</div>

## Why it works {#why-it-works}

<table>
  <tr>
    <td><strong>100% offline</strong><br>No login, no cloud dependency, no required internet.</td>
    <td><strong>Customizable content</strong><br>Add new 30-day programs without rebuilding the app UI.</td>
  </tr>
  <tr>
    <td><strong>Notebook-style flow</strong><br>Designed for a warm, focused daily reflection experience.</td>
    <td><strong>Translation-ready</strong><br>Labels and content can be localized through JSON packs.</td>
  </tr>
</table>

## Features {#features}

### Daily experience
Each day can include:
- morning checklist
- afternoon checklist
- evening checklist
- daily challenge prompt
- notes and reflections
- progress tracking fields

### Local challenge library
Users can keep multiple challenge packs on-device and switch between them inside the app.

### Import from files
Challenge packs can be distributed as `.json` files and imported from Files, AirDrop, or other iOS-supported locations.

### Flexible tracking
The same tracker structure can support habits like sleep, focus, prayer, money, reading, exercise, gratitude, or study time.

## What the app can become

This app structure can support many product directions:

- **Habit Builder App**
- **Guided Journal App**
- **30-Day Budget Challenge App**
- **Faith and Prayer Challenge App**
- **Study Sprint App**
- **Wellness Reset App**

## Challenge packs {#challenge-packs}

The current project already shows multi-pack support, including themes like budgeting and self-improvement. That means you can turn one app into a reusable platform for multiple downloadable experiences.

### Example JSON format

```json
{
  "id": "my-challenge-v1",
  "version": "1.0",
  "language": "en",
  "metadata": {
    "title": "My 30-Day Challenge",
    "subtitle": "A subtitle",
    "author": "Growth Ideology",
    "durationDays": 30,
    "labels": {
      "morning": "Morning Checklist",
      "afternoon": "Afternoon Checklist",
      "evening": "Evening Checklist",
      "todayChallenge": "Today's Challenge",
      "reflection": "Reflection"
    }
  },
  "habitTrackerColumns": ["Sleep", "Exercise", "Reading"],
  "days": []
}
```

### Why this format matters

- launch new challenge themes faster
- localize to new languages
- sell or share niche packs without redesigning the app
- keep the same core app experience across many products

## For creators {#for-creators}

If you are building a brand around content, coaching, or education, this app gives you a flexible product format:

1. Build one iOS app shell
2. Publish multiple challenge packs
3. Translate to different languages
4. Keep user data private and local
5. Grow a product ecosystem around recurring 30-day experiences

## App architecture

```text
SwiftUI app
├── App/                 Entry point + Info.plist
├── Models/              Challenge, day, checklist, scoring models
├── ViewModels/          Business logic + persistence
├── Views/               Home, detail, tracker, settings, library
├── Utilities/           Design system and reusable UI helpers
└── Resources/           Challenge JSON packages + assets
```

## Suggested repository structure

```text
your-repo/
├── docs/                 GitHub Pages website
├── ThirtyDayChallenge/   iOS source code
└── README.md
```

## Publish with GitHub Pages

1. Put this website inside the `docs/` folder of your repository.
2. Push the repository to GitHub.
3. Open **Settings → Pages**.
4. Set **Source** to **Deploy from a branch**.
5. Select **main** and **/docs**.
6. Save and wait for GitHub Pages to publish the site.

## Need legal pages?

These are already included in this website package:

- [Terms of Use](./terms)
- [Privacy Policy](./privacy-policy)
- [Support](./support)

## Next ideas

- add real iPhone screenshots
- add TestFlight or App Store button
- add FAQ page
- add changelog page
- add challenge marketplace page
- add docs for authors creating JSON packs
