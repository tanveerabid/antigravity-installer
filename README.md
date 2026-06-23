# Antigravity Linux Installer & Orchestrator CLI

An advanced, atomic management tool built to seamlessly install, update, and completely isolate Google Antigravity 2.0 application files on modern desktop Linux environments (X11 & Wayland).

## Key Features
* 🔒 **Runtime Memory Isolation:** Configures native sandbox flags to completely eliminate multi-instance memory collisions (`SIGTRAP` errors).
* 👁️ **Hidden ASAR Icon Extraction:** Pulls application image assets directly out of compressed Electron files so system menus can render your icons perfectly.
* 📌 **Correct Window Grouping:** Automatically maps execution strings (`StartupWMClass`) to your dock launcher to avoid broken generic gear window emblems.
* 🔀 **Smart Safety Guardrails:** Restricts mismatched source files from executing over opposite runtime profiles.

## Prerequisites
Before launching the script, verify that your system architecture satisfies these minor dependencies:
* **Operating System:** Ubuntu 20.04+, Debian 10+, Fedora 36+, Linux Mint 21+, or Arch Linux.
* **Interpreter:** `python3` (required to decode the binary `.asar` filesystem logs).
* **Privileges:** Standard desktop user configuration (the script calls `sudo` internally *only* when modifying `/opt`).

---

## 🛠️ Step 1: Install the CLI Tool
Deploy the stable management client directly onto your system using this isolated single line installation:

```bash
curl -sSL [https://raw.githubusercontent.com/tanveerabid/antigravity-installer/main/antigravity-cli](https://raw.githubusercontent.com/tanveerabid/antigravity-installer/main/antigravity-cli) -o ~/.local/bin/antigravity-cli && chmod +x ~/.local/bin/antigravity-cli
