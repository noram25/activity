# Activity Manager for KDE

A command-line tool to manage KDE Activities with safety features.

## Features

- Switch between activities by ID, name, or index
- List activities in table format
- Export activities to CSV or JSON
- Create, remove, and modify activities
- Slideshow mode to cycle through activities
- **`--dry-run`** support for all destructive operations
- Proper error handling and exit codes

## Dependencies

- KDE Plasma (Activities framework)
- `qdbus6` (usually installed with KDE)

## Installation

```bash
# Download to your PATH
curl -o ~/.local/bin/activity https://raw.githubusercontent.com/noram25/activity/main/activity
chmod +x ~/.local/bin/activity

# Download and install the manual page
sudo curl -o /usr/local/share/man/man1/activity.1 https://raw.githubusercontent.com/noram25/activity/main/activity.1
sudo mandb
