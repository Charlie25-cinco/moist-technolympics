# MOIST Technolympics

A browser-based Technolympics and exhibit prize-draw experience, presented with a cyber-casino visual theme for an event setting. The interface includes game-style prize activities, a participant roster, prize inventory controls, and a winner ledger.

> **Note:** This repository's main page is a client-side event application. Its saved roster, prizes, and winner records use the browser's local storage; the inspected source does not show a server-side database or account system. Use it as a local event tool, not as a real-money gambling platform.

## Features

- **Game lobby and activities** — the lobby lists Cyber Reels, Lucky Wheel, Cyber Cards, Quantum Scatter, Plinko Drop, Dice Roll, Mystery Box, Coin Flip, Number Ball Draw, Scratch Card, Treasure Chest, and Lucky Envelope.
- **Participant roster** — register a student individually or in bulk, assign an educational level (JHS, SHS, College, or Other), search/select a participant, and manage the directory.
- **Prize inventory** — add, edit, and delete prize entries; configure stock, draw chance, tier, and an image or image URL.
- **Prize draw results** — display the result and inspect available result-pattern details.
- **Winner ledger** — review recorded results and export the ledger as a CSV file.
- **Event-friendly presentation** — responsive layout, navigation between game and management views, sound effects/music controls, and confetti effects.

The available activities and their behavior are implemented in the single-page interface; exact game behavior can vary by selected activity.

## Technologies

- **HTML5** for the page structure
- **CSS** for custom styling and effects
- **JavaScript (vanilla)** for game interactions, roster and inventory management, and result logging
- **Tailwind CSS** loaded from its CDN
- **Font Awesome 6.4.0** for icons
- **Google Fonts** (JetBrains Mono, Space Grotesk, and Plus Jakarta Sans)
- **canvas-confetti 1.6.0** for confetti effects
- **Browser Local Storage** for persistent client-side data

This repository currently uses a standalone `index.html` entry page; no `package.json` or build-tool configuration was found during inspection.

## Getting Started

### Run locally

1. Clone or download this repository.
2. Open `index.html` in a modern browser.

For the most reliable experience, serve the folder through a simple local HTTP server instead of opening the file directly, particularly if browser restrictions affect any features.

### Internet connection

The page loads Tailwind CSS, Font Awesome, Google Fonts, the confetti library, and some images from external URLs. An internet connection is therefore needed for all externally hosted assets to load. Core page code is stored in `index.html`.

## Data and Limitations

- Roster entries, educational levels, prize inventory, winner records, and some interface state are saved in the current browser's local storage.
- This is **browser-local storage**, not a shared database. Data is not automatically synchronized across devices or different browsers.
- Clearing the browser's site data may remove saved application data. Export the winner ledger when you need a separate CSV copy.
- The page does not show a server-side login or permission system in the inspected source. Anyone with access to the running page and its browser can potentially interact with its management controls.
- External assets may be unavailable if their hosting URLs change or the device is offline.
- The application is intended for event-style simulated prize activities. It does not provide a backend for real-money betting or cash-out.

## Repository Structure

```text
moist-technolympics/
└── index.html   # Main page, styles, and client-side application logic
```

## License

No license file was identified during the repository inspection. Unless a license is added, do not assume that the project is available for unrestricted reuse or redistribution.
