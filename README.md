# Antigravity Linux Installer & Orchestrator CLI

An advanced, atomic management tool built to seamlessly install, update, and completely isolate Google Antigravity 2.0 application files on modern desktop Linux environments (X11 & Wayland).

---

## Key Features

- 🔒 **Runtime Memory Isolation:** Configures native sandbox flags to completely eliminate multi-instance memory collisions (`SIGTRAP` errors).
- 👁️ **Hidden ASAR Icon Extraction:** Pulls application image assets directly out of compressed Electron files so system menus can render your icons perfectly.
- 📌 **Correct Window Grouping:** Automatically maps execution strings (`StartupWMClass`) to your dock launcher to avoid broken generic gear window emblems.
- 🔀 **Smart Safety Guardrails:** Restricts mismatched source files from executing over opposite runtime profiles.

---

## Prerequisites

Before launching the script, verify that your system satisfies these dependencies:

| Requirement | Details |
|---|---|
| **Operating System** | Ubuntu 20.04+, Debian 10+, Fedora 36+, Linux Mint 21+, or Arch Linux |
| **Interpreter** | `python3` — required to decode binary `.asar` filesystem logs |
| **Privileges** | Standard desktop user — the script calls `sudo` internally only when modifying `/opt` |

---

## Step 1: Install the CLI Tool

Deploy the management client onto your system using this single-line installation:

```bash
curl -sSL https://raw.githubusercontent.com/tanveerabid/antigravity-installer/main/antigravity-cli \
  -o ~/.local/bin/antigravity-cli && chmod +x ~/.local/bin/antigravity-cli
```

---

## Step 2: Download and Run an Archive

1. Go to your browser and download the official application source files (`.tar.gz` packages).
2. Open your system **Downloads** folder (or wherever you saved the files).
3. Right-click any empty space inside that folder and select **Open in Terminal**.
4. Run the installation commands from that terminal window so the script can locate your downloaded archives.

---

## Usage

Run all commands from the terminal you opened inside your downloads directory.

### Help

```bash
antigravity-cli --help
```

### Install

```bash
# Install the background Hub orchestrator engine
antigravity-cli --install --hub

# Install the workspace developer interface (IDE)
antigravity-cli --install --ide
```

### Update

```bash
# Update Hub to a newly downloaded archive version
antigravity-cli --update --hub

# Update IDE to a newly downloaded archive version
antigravity-cli --update --ide
```

### Remove

```bash
# Remove Hub application files and desktop entry
antigravity-cli --remove --hub

# Remove IDE application files and desktop entry
antigravity-cli --remove --ide
```

---

## Command Reference

| Command | Flag | Description |
|---|---|---|
| `--help` | — | Display the interactive help menu |
| `--install` | `--hub` / `--ide` | Install from a downloaded `.tar.gz` archive |
| `--update` | `--hub` / `--ide` | Update an existing installation from a new archive |
| `--remove` | `--hub` / `--ide` | Remove application files and desktop launcher |
