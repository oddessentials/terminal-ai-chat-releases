# terminal-ai-chat

Chat with ChatGPT in your terminal, using your normal ChatGPT login. No API key needed.

## Install

**macOS and Linux**

```sh
curl -fsSL https://github.com/oddessentials/terminal-ai-chat-releases/releases/latest/download/install.sh | sh
```

**Windows** (needs [WSL](https://learn.microsoft.com/windows/wsl/install) with Ubuntu 24.04)

```powershell
irm https://github.com/oddessentials/terminal-ai-chat-releases/releases/latest/download/install.ps1 | iex
```

To update, run the same command again.
Check it's installed with `terminal-ai-chat --version`.

Prefer a package manager? Use `brew install oddessentials/tap/terminal-ai-chat` or
`winget install OddEssentials.TerminalAIChat`, then run `terminal-ai-chat setup` once.

## Use

```sh
terminal-ai-chat
```

Sign in to ChatGPT in the browser window that opens, then press **Enter** in the terminal and start chatting.
Type `/exit` to quit.
