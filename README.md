# Block Notes x Reminder

Block Notes x Reminder is a lightweight desktop notes app for Windows and Linux. It lets you write notes, save them locally, and assign reminders to any note using a simple right-click workflow.

## Features

- Create, edit, and delete notes
- Save notes locally as JSON files
- View a list of notes in the main window
- Set a reminder on a note with date and time
- Receive a notification when the reminder expires
- Cross-platform design using Python and Tkinter
- No heavy dependencies

## Product idea

This app is designed like a small personal note vault: the user can keep routine notes, important ideas, and short reminders in one place. It is oriented toward a simple workflow:

- open a note
- write or paste text
- right-click the note in the list
- choose “Imposta reminder”
- set the date and time
- wait for the reminder notification to appear

This is a practical base for a future Obsidian-like app with richer features such as tag management, note grouping, and search.

## Project structure

- `main.py` — application entry point
- `data/` — folder where notes are stored
- `README.md` — project documentation
- `requirements.txt` — dependency listing
- `.gitignore` — excludes local runtime artifacts
- `LICENSE` — MIT license

## Requirements

### Windows

- Python 3.10 or newer
- Tkinter is included with the standard Python installer on Windows

### Linux

- Python 3.10 or newer
- Tkinter package installed

Example on Ubuntu/Debian:

```bash
sudo apt update
sudo apt install python3 python3-tk
```

## Installation

1. Clone the repository:

```bash
git clone https://github.com/Blingutufdu37373/block-notes-x-reminder.git
cd block-notes-x-reminder
```

2. Create and activate a virtual environment (recommended):

```bash
python -m venv .venv
source .venv/bin/activate
```

On Windows PowerShell:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Launch the app:

```bash
python main.py
```

## How to use reminders

1. Create a new note or select an existing one.
2. Write the text for your note.
3. Right-click the note in the list.
4. Choose “Imposta reminder”.
5. Select the date and time.
6. When the reminder time is reached, the app shows a notification with the note title and content.

Example:

- Title: “Spesa”
- Reminder: 2026-11-20 18:30
- At 18:30, the app displays a notification

## Notes for development

The version in this repository is a functional 1.0 alpha, focused on a reliable note-taking and reminder workflow with minimal dependencies and easy testing.

It is designed to be improved with:

- note search
- note categories/tags
- note folders and grouping
- native OS notifications
- export to Markdown
- future Obsidian-like features

## Release workflow

To publish a GitHub release, create a tag such as `v1.0.0` in the GitHub UI and attach the packaged files for your target platform.

This repository is prepared for a simple first public release, but the final publishing step must be done through the GitHub Releases page because release creation is not available through the current chat tools.

## License

This project is distributed under the MIT License.
