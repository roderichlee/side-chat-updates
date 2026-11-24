<p align="center">
  <img src="icon.png" width="128" height="128" alt="Side Chat icon">
</p>

<h1 align="center">Side Chat</h1>

<p align="center">
  <b>Ask a quick side question about any AI answer, without derailing your main chat.</b><br>
  For Claude, ChatGPT and Gemini on macOS.
</p>

<p align="center">
  <a href="https://github.com/roderichlee/side-chat-updates/releases/latest"><img alt="Latest release" src="https://img.shields.io/github/v/release/roderichlee/side-chat-updates?label=download&color=1f1e1d"></a>
  <img alt="macOS 13+" src="https://img.shields.io/badge/macOS-13%2B-1f1e1d">
  <img alt="Apple Silicon" src="https://img.shields.io/badge/Apple%20Silicon-native-1f1e1d">
</p>

---

Have you ever been deep in a long conversation with Claude or ChatGPT, hit one line you didn't quite understand, and had to choose between derailing the whole chat with a side question or opening a new chat that knows nothing about what you were discussing?

**Side Chat lets you highlight any part of an answer, press a hotkey, and ask about it in a small pop-up that already knows the whole conversation.** Get your answer, press <kbd>Esc</kbd>, and you're right back where you were. Your main chat stays clean.

## How it works

1. **Highlight** a sentence, equation or block of code, in Claude or any other app.
2. **Press <kbd>⌃</kbd> <kbd>⇧</kbd> <kbd>Space</kbd>.** You can change the hotkey. A small chat opens next to your cursor.
3. **Ask**, or tap a quick action: **Explain It · Example · Define terms · Quiz me · Check it**.

Side Chat sends the AI three things:
- **What you highlighted.**
- **A screenshot** of the window you were reading.
- **The whole conversation.** From the Claude app, or from claude.ai, chatgpt.com or gemini.google.com in your browser. This includes the parts scrolled out of view, so its answers connect to what you discussed earlier.

## Features

- **Knows the whole chat.** It reads the full conversation, not just what's on screen.
- **Works with your account.** Sign in with ChatGPT to use your Plus or Pro plan with no API key, sign in with OpenRouter, or use an Anthropic, OpenAI or Google Gemini key.
- **Fast by default.** Answers stream from a fast model. Press <kbd>⌘</kbd><kbd>M</kbd> to switch to a stronger one.
- **Readable answers.** Markdown, highlighted code, and real math symbols (LaTeX).
- **Looks at home next to Claude.** It follows light or dark mode, and you can choose the answer font, text size and menu bar icon.
- **Stays out of the way.** It lives in the menu bar. <kbd>Esc</kbd> hides it and sends you back to the app you were in.
- **Updates itself.** Every update is signed and checked before it installs.

## Install

In Terminal. This way gives no security warning:

```bash
curl -fsSL https://github.com/roderichlee/side-chat-updates/releases/latest/download/install.sh | bash
```

Or download the **.dmg** from the [latest release](https://github.com/roderichlee/side-chat-updates/releases/latest) and drag Side Chat into Applications. Since the app isn't notarized by Apple yet, allow it once in **System Settings → Privacy & Security → Open Anyway**.

On first launch, a short guide walks you through:
- the two macOS permissions,
- connecting an AI,
- choosing your hotkey.

Needs macOS 13 or later on an Apple Silicon Mac.

## Privacy

- **No history.** Side Chat keeps no history, no analytics and no account of its own.
- **Only when you ask.** Your highlight, the screenshot and the conversation go to the AI provider you picked, and only when you press the hotkey and ask. They're thrown away when the pop-up closes.
- **Chat sites only.** In a browser it reads only claude.ai, chatgpt.com and gemini.google.com. Other websites are never read.
- **Keys stay local.** API keys and sign-ins stay in your macOS Keychain and go only to their own provider.

## Updates

Side Chat checks this page for new versions about every 6 hours. You can also choose **Check for Updates…** from its menu bar menu.

Every update is signed. Side Chat refuses any download that isn't signed with the developer's key.

---

<p align="center"><sub>This repository hosts the app downloads. Side Chat isn't affiliated with Anthropic, OpenAI or Google.</sub></p>
