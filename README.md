# Yello

A Trello-style kanban app in a single HTML file. No server, no build step, no account. Open `index.html` in a browser and start organizing. Your data stays in your browser.

**Version 1.2**

## Features

- **Boards, lists and cards** with drag and drop (mouse and touch), archive, copy and move
- **Card details**: markdown descriptions, labels, members, checklists, comments, attachments, covers, start and due dates
- **Views**: Board, Timeline (start to due dates) and Calendar, with drag to reschedule
- **Search and filters** across cards
- **Undo and redo** for every change
- **Automatic backups**: rolling snapshots kept in the browser, plus a reminder to export
- **Export and import** as JSON for one board or everything, and import of Trello JSON exports
- **Light and dark themes**, board backgrounds, emoji icons
- **Mobile friendly**: long-press to drag on touch screens

## Getting started

1. Download `index.html`.
2. Open it in any modern browser (Chrome, Edge, Firefox, Safari).
3. Create a board and go.

Or host it as a static page, for example with GitHub Pages (Settings, Pages, deploy from the `main` branch root).

## Your data

Everything is saved in your browser's local storage and IndexedDB on the device you use. Nothing is sent anywhere. Because browser storage can be cleared, use the export button (💾) now and then to download a JSON backup. Import it on any device to restore.

## Security

Yello was reviewed for hostile imported data in v1.2:

- All user text is HTML-escaped; imported colors, backgrounds, cover images, links and dates are validated
- A Content Security Policy blocks all network access and outside scripts, and no referrer is sent
- Imports are size-limited and processed in linear time

Anyone with access to your browser profile can read your boards; data is not encrypted.

## Keyboard and tips

- Press the card title to open details; use the quick-edit pencil on a card for fast changes
- Click outside a composer to close it

## License

MIT
