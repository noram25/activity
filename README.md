# Activity Manager for KDE

A command-line tool to manage KDE Activities with safety features.

## Quick Start

Show all activities with current activity marked by `*`:

```bash
activity --show-table
```

**Example output:**

```text
ACT  ID                                      NAME
     0c12898d-a014-41c9-8e32-303fb42e2007    1. Downloading
*    ffed83a0-84c4-4600-97a3-6d2f2c31d8a8    2. Main
     c58a85b6-5b38-4e1d-a40b-3c30b6dfcfca    3. Private
     3f729292-39ab-44a5-8d46-83b50ac9f248    4. Programming
```

Switch to an activity by name:

```bash
activity --switch-by-name "Programming"
```

Preview a destructive action (safe):

```bash
activity --dry-run --remove-activity "1. Downloading"
```

For more examples, see [Usage Examples](Usage%20Examples).

## Features

- Switch between activities by ID, name, or index
- List activities in table format
- Export activities to CSV or JSON
- Create, remove, and modify activities
- Slideshow mode to cycle through activities
- **`--dry-run`** support for all destructive operations
- Proper error handling and exit codes

## Installation

```bash
# Download to your PATH
curl -o ~/.local/bin/activity https://raw.githubusercontent.com/noram25/activity/main/activity
chmod +x ~/.local/bin/activity

# Download and install the manual page
sudo curl -o /usr/local/share/man/man1/activity.1 https://raw.githubusercontent.com/noram25/activity/main/activity.1
sudo mandb
```

## Dependencies

- KDE Plasma (Activities framework)
- `qdbus6` (usually installed with KDE)

## Getting Help

```bash
# Show all available commands
activity --functions

# Show detailed help
activity --help

# View the manual page
man activity
```

## License

MIT License — see [LICENSE](LICENSE) file for details.

## Author

Nora Moyer — [BlueSky](https://bsky.app/profile/noram25.bsky.social)
