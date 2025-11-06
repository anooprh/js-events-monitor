# JavaScript Events Monitor

A single-page tool that listens to nearly every browser event, displays them in real time, and lets you filter, pause, and export the log. No build step or backend required—just open the page in a browser.

Available at https://anooprh.github.io/js-events-monitor

## Getting Started

### GitHub Pages
- Commit `index.html` to the branch you publish through GitHub Pages (e.g. `gh-pages` or `main`).
- Enable Pages in your repository settings and point it at that branch.
- Visit the published URL (shown in the Pages settings) to start capturing events.

### Local Usage
- Simply open `index.html` in any modern browser (double-click or drag it into a tab). Everything works over the `file://` protocol.
- Optional: run a static server if you prefer `http://` URLs. For example:
  ```bash
  npx serve .
  ```

## Features

- **Real-time Event Monitoring** – Streams new browser events to the log instantly.
- **Detailed Context** – Shows event type, target element, pointer position, key codes, modifiers, and more.
- **Powerful Filtering** – Enable or disable event categories and individual event types.
- **Pause & Clear Controls** – Pause logging to inspect entries or clear the log to start fresh.
- **Export to File** – Download the captured log as a timestamped `.txt` file.
- **Live Statistics** – Track totals, filtered counts, and pause status.

## Event Coverage

The monitor registers listeners for most standard DOM events, grouped into:
- Mouse, pointer, and wheel events
- Touch and gesture events
- Keyboard events (with left/right modifier tracking)
- Form and clipboard events
- Window lifecycle, navigation, and resize events
- Media playback events
- Drag-and-drop events

Additional events can be added in `index.html` if you need to extend the coverage.

## Customization Tips

- Update the event categories or styling directly inside `index.html`—everything is self-contained.
- Clone the layout or logic into your own project by copying the markup and script sections.
- When hosting elsewhere, ensure the page loads over HTTPS if you need secure-only browser APIs (e.g. clipboard write).

