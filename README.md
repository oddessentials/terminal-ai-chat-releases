# terminal-ai-chat

A terminal client for your ChatGPT web session, for Windows, Linux and macOS.
It uses your normal ChatGPT login and needs no API key. Sign-in happens in a
dedicated, sandboxed Chrome that the tool provisions privately: on Windows that
Chrome runs inside WSL, on Linux and macOS it runs directly on your machine.

This repository publishes the signed release binaries, install scripts and
checksums. See [Releases](https://github.com/oddessentials/terminal-ai-chat-releases/releases).

## Requirements

- A desktop session. Sign-in happens in a real browser window.
- Windows 10 or 11 (x86-64) with WSL and the `Ubuntu-24.04` distribution.
- Linux x86-64 on X11 or Wayland, with unprivileged user namespaces enabled.
- macOS on Apple Silicon or Intel.

## Install and update

Linux and macOS:

```sh
curl -fsSL https://github.com/oddessentials/terminal-ai-chat-releases/releases/latest/download/install.sh | sh
```

Windows (PowerShell):

```powershell
irm https://github.com/oddessentials/terminal-ai-chat-releases/releases/latest/download/install.ps1 | iex
```

Run the same command again to update. The script checks the download against
the release's `SHA256SUMS` (and, on Windows, its Authenticode signature) and
sets up the private browser runtime.

Homebrew (macOS and Linux) and WinGet:

```sh
brew install oddessentials/tap/terminal-ai-chat
```

```powershell
winget install OddEssentials.TerminalAIChat
```

These install only the program. Run `terminal-ai-chat setup` once afterwards,
and again if `terminal-ai-chat` asks for it after an upgrade.

## Run

```sh
terminal-ai-chat
```

Sign in to ChatGPT in the Chrome window that opens, return to the terminal and
press Enter. Type `/exit` when you're done.
