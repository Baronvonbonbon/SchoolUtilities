[README.md](https://github.com/user-attachments/files/21723866/README.md)
# Common Core Standards Checklist & Evidence Tracker

This project provides an **interactive, offline-capable checklist** for tracking Common Core State Standards (CCSS) mastery, with the ability to attach and organize **evidence files** for each standard.

The HTML file includes:
- Full Common Core standards organized **by grade** and **strand**
- A grouped **College & Career Readiness (CCR) Anchor Standards** section
- Search, expand/collapse all, and filter controls
- **Attach evidence** (local storage or save to disk)
- Export/import checklist state **with evidence files embedded**
- **ZIP export** of evidence (all or per-grade)
- On-disk folder browsing and file deletion (File System Access API)
- Light/Dark theme toggle
- Runs fully offline in any modern browser

## Features

- **Checkbox tracking**: mark standards complete; progress auto-saves in your browser
- **Evidence uploads**: attach supporting documents, images, or PDFs to each standard
- **Local storage & disk sync**: store files locally in your browser or export to a real folder
- **ZIP exports**: download all or per-grade evidence as organized ZIP archives
- **On-disk browsing**: view your chosen evidence folder in a collapsible tree
- **Filters**: show all, only with evidence, or only without evidence
- **Responsive design**: works on desktop, tablet, and phone
- **Cross-platform**: works on Windows, macOS, Linux

## Installation

No installation required — just download the HTML file and open it in your browser.

For full functionality (on-disk evidence management, folder browsing, file deletion), **serve locally** using the provided helper scripts to allow the browser to grant file system access permissions.

### Running Locally (recommended)

#### Option 1: Python (cross-platform)
```bash
python3 run_local_server.py
```
Open the printed `http://localhost:8000` link in your browser.

#### Option 2: Windows
Double-click `start_server.bat`.

#### Option 3: macOS
1. Make `start_server.command` executable (only once):
   ```bash
   chmod +x start_server.command
   ```
2. Double-click `start_server.command`.

The server will serve files from the current folder at `http://localhost:8000`.

## Usage

1. **Open the HTML file** in your browser.
2. Use **search**, **expand/collapse**, and **filters** to navigate standards.
3. Click the 📎 icon to **attach evidence** to a standard.
4. Export/import checklist state with evidence via the toolbar.
5. Use the **Choose evidence folder** option to store files on disk in a structured folder tree:
   - Grade → Strand → Standard ID
6. Browse or delete evidence in the right-hand Evidence panel.
7. Use the **ZIP export** buttons for backups or sharing.

## Classroom & Homeschool Management

- **Classroom**: Teachers can maintain a master checklist per class, attach scanned student work as evidence, and export/import progress between devices.
- **Homeschool**: Parents can track mastery for each child, store portfolio evidence, and print/export for evaluation or reporting.
- Use **per-grade ZIP exports** for annual reporting.
- **Filters** allow focusing on incomplete standards or reviewing completed ones with evidence.

## Requirements

- Modern browser (Chrome, Edge, Brave recommended for full file system features)
- Python 3 (optional, for local server)
- No internet required after download

## License

This project is provided as-is for educational use. No warranty or guarantee of accuracy is provided.


## Acknowledgements

This project incorporates and adapts ideas and techniques from open-source resources.

Special thanks to [Phil Ngo](https://gist.github.com/philngo) for providing the original [JavaScript ZIP creation gist](https://gist.github.com/philngo/2735248c98c3e0cd7814), 
which informed parts of the evidence ZIP export functionality. Licensed under the terms provided in the original gist.

