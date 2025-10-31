# Surgical Video Summarizer Frontend

This project provides a desktop-style web interface for uploading surgical procedure recordings, simulating AI processing, and previewing an auto-generated highlight reel. The UI is implemented with vanilla HTML, CSS, and JavaScript, so no build tooling is required.

## Prerequisites

- Any modern web browser (Chrome, Firefox, Safari, Edge)
- A local static file server (optional but recommended). Python is preinstalled on most systems and includes a simple HTTP server.

## Getting Started

You can open `index.html` directly in your browser, or serve the project over HTTP to enable full functionality such as local video playback security policies.

### Option A: Open the file directly
1. Clone or download this repository.
2. Double-click `index.html` (or open it via your browser's **File → Open File…** menu).

### Option B: Serve with a local HTTP server (recommended)
Serving the files removes browser restrictions around local file access and ensures media playback works as expected.

1. Clone or download this repository.
2. Open a terminal in the project directory.
3. Start a static server. Examples:
   - **Python 3:** `python -m http.server 8000`
   - **Node.js (http-server):** `npx http-server -p 8000`
4. Visit `http://localhost:8000` in your browser.

## Usage

1. Click **Upload Surgical Video** to select a video file from your computer.
2. Review the extracted metadata and enter optional procedure notes.
3. Press **Generate Summary** to simulate the AI workflow. The interface will display progress, highlight cards, and a condensed playback preview.
4. Use the export controls to simulate downloading the highlight reel or copying timestamps for documentation.

## Project Structure

- `index.html` – Layout markup and component structure for the desktop UI.
- `styles.css` – Visual design, theming, and layout rules.
- `script.js` – Client-side logic for handling uploads, simulating processing, updating the UI, and managing playback interactions.

## Troubleshooting

- If video playback does not start, ensure you are accessing the site via `http://` or `https://` rather than the `file://` protocol.
- Large video files may take longer to load in the browser; try smaller samples during testing.
- Clear your browser cache if you make local changes to the frontend files and do not see them reflected immediately.

## License

This project is provided as-is for demonstration purposes. Adapt it freely to match your production environment and compliance requirements.
