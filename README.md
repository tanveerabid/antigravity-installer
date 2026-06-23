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

---

## 📥 How to Download and Run the Archive
1. Go to your web browser and download the official application source files (`.tar.gz` packages).
2. Open your system **Downloads** folder (or the folder where you saved the files).
3. Right-click on any empty blank space inside that folder window and select **Open in Terminal**.
4. Run your installation commands from this specific terminal window so the script can locate your downloaded archives.

---

## 🚀 Usage Commands Reference

Run these commands directly from the terminal window you opened inside your download directory:

### 1. View Available System Options
To display the complete interactive help menu and flags, type:
```bash
antigravity-cli --help instructions** on downloading the .tar.gz files from Google and opening the terminal right there.
* **A Command Reference section** showing exactly how to use --help, --install, --update, and --remove.
