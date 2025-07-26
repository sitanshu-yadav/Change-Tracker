# Web Page Change Tracker

Web Page Change Tracker is a Chrome extension that monitors a selected area or the full page of any website for visual changes and provides an audio alert when a change is detected.

## Features

- Select a specific area of a web page to monitor for changes.
- Option to track the entire visible page.
- Customizable alert phrase (spoken using Chrome's Text-to-Speech).
- Adjustable check interval (in seconds).
- Simple and intuitive popup UI.

## Installation

1. Clone or download this repository.
2. Open Chrome and go to `chrome://extensions/`.
3. Enable "Developer mode" (top right).
4. Click "Load unpacked" and select the project directory.

## Usage

1. Click the extension icon to open the popup.
2. (Optional) Click **Select Area to Track** and drag to select a region on the page.
3. Or, check **Track Full Page** to monitor the entire visible page.
4. Enter your desired **Alert Phrase** and **Check Interval** (in seconds).
5. Click **Start Tracking**.
6. When a change is detected, the alert phrase will be spoken.
7. Click **Stop Tracking** to end monitoring.

## Files

- [`background.js`](background.js): Handles background logic, periodic checks, and alerts.
- [`content.js`](content.js): Manages area selection and image comparison in the web page.
- [`popup.html`](popup.html): Popup UI for user interaction.
- [`popup.js`](popup.js): Logic for the popup UI.
- [`popup.css`](popup.css): Styles for the popup.
- [`manifest.json`](manifest.json): Chrome extension manifest.
- `icon.png`: Extension icon.

## Permissions

- `storage`: Save user settings and image data.
- `activeTab`, `scripting`: Interact with the current tab.
- `tts`: Use Chrome's Text-to-Speech for alerts.
- `declarativeContent`: Required for extension action.

## License

MIT License
