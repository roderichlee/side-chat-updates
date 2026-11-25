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
  <img alt="Apple Silicon and Intel" src="https://img.shields.io/badge/Apple%20Silicon%20%26%20Intel-native-1f1e1d">
</p>

---

Have you ever been deep in a long conversation with Claude or ChatGPT, hit one line you didn't quite understand, and had to choose between derailing the whole chat with a side question or opening a new chat that knows nothing about what you were discussing?

**Side Chat lets you highlight any part of an answer, press a hotkey, and ask about it in a small pop-up that already knows the whole conversation.** Get your answer, press <kbd>Esc</kbd>, and you're right back where you were. Your main chat stays clean.

## How it works

1. **Highlight** a sentence, equation or block of code, in Claude or any other app.
2. **Press <kbd>⌃</kbd> <kbd>⇧</kbd> <kbd>Space</kbd>.** You can change the hotkey. A small chat opens next to your cursor.
3. **Ask**, tap a quick action (**Explain It · Example · Define terms · Quiz me · Check it**), or type <kbd>/</kbd> for a command.

Side Chat sends the AI what it needs to answer well:
- **What you highlighted.** Math in it shows as real math, not raw LaTeX.
- **A screenshot** of the window you were reading.
- **The whole conversation.** From the Claude app, or from claude.ai, chatgpt.com or gemini.google.com in your browser. This includes the parts scrolled out of view, so its answers connect to what you discussed earlier.
- **Files you uploaded to the chat**, such as a homework PDF, when your copy is on this Mac.

## Features

Every feature can be switched off, and every shortcut can be changed, in **Settings → Features**.

### Asking

- **Knows the whole chat.** It reads the full conversation, not just what's on screen.
- **Reads the files you uploaded.** Uploaded a PDF, Word or text file to the chat? If your copy is on this Mac (Downloads, Desktop, Documents or iCloud Drive), Side Chat reads it too, so answers use the whole file, not just what's visible. A chip shows each file; click its × to leave it out. Long files send only the pages around your highlight. Only files actually uploaded to the chat count, not file names that are merely mentioned. The first time, Side Chat explains this before macOS asks for access to the folder.
- **Commands.** Type <kbd>/</kbd> in the text box for a list that narrows as you type: `/model` (pick any connected model for this side chat), `/fast`, `/strong`, `/compare`, `/clear`, `/pin`, `/area`, `/history`, `/copy`, `/save`, `/flashcards`, `/send`, `/read`, `/theme`, `/settings`, plus one for each quick action.
- **Quick actions.** One-tap questions above the text box (<kbd>⌘</kbd><kbd>1</kbd>–<kbd>⌘</kbd><kbd>9</kbd>). Add, edit, reorder or remove them in Settings.
- **Select an area.** Drag over part of the screen and ask about just that part, such as a graph or a diagram. Works from any app (<kbd>⌥</kbd> + your hotkey).
- **Fast or strong model.** Answers stream from a fast model. Press <kbd>⌘</kbd><kbd>M</kbd> to switch to a stronger one.
- **Compare two models** (<kbd>⌘</kbd><kbd>K</kbd>). Ask two models at once, side by side, and keep the better answer.
- **Pin** (<kbd>⌘</kbd><kbd>P</kbd>). Keeps the pop-up open. Each hotkey press adds the new highlight to the same side chat.
- **Branch.** Highlight part of a Side Chat answer and ask about just that part.
- **Dictation** (<kbd>⌘</kbd><kbd>D</kbd>). Talk instead of typing, with macOS Dictation.
- **Claude Code sessions.** When the Claude app shows a Claude Code session, Side Chat reads that session's transcript.

### Answers

- **Readable answers.** Markdown, highlighted code, and real math symbols (LaTeX).
- **Send to chat** (<kbd>⌘</kbd><kbd>⇧</kbd><kbd>↩</kbd>). Pastes the answer, or a drafted follow-up, into your main chat. It never presses Return for you.
- **Read aloud** (<kbd>⌘</kbd><kbd>R</kbd>). Speaks the latest answer. Press again to stop.
- **Save as notes or flashcards** (<kbd>⌘</kbd><kbd>S</kbd>). Save the side chat as a Markdown file, or as flashcards you can import into Anki.
- **Copy** (<kbd>⌘</kbd><kbd>⇧</kbd><kbd>C</kbd>). Copies the whole side chat as Markdown.
- **Cost and a monthly cap.** With an API key, each answer shows its estimated price, and you can set a monthly spending cap.

### History

- **History** (<kbd>⌘</kbd><kbd>Y</kbd>, or the clock button). Search, reread, copy and delete past side chats. Saving is **off** until you turn it on, and saved chats stay on this Mac.
- **History from any app.** Give it a shortcut to open the pop-up straight to History.

### The app

- **Works with your account.** Sign in with ChatGPT to use your Plus or Pro plan with no API key, sign in with OpenRouter, or use an Anthropic, OpenAI or Google Gemini key.
- **Looks at home next to Claude.** A see-through glass background like the Claude app's sidebar, light or dark mode, and your choice of answer font, text size and menu bar icon.
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

Needs macOS 13 or later, on an Apple Silicon or Intel Mac.

## Privacy

- **No account, no analytics.** Side Chat has no account of its own and collects no analytics.
- **Only when you ask.** Your highlight, the screenshot, the conversation and any uploaded file go to the AI provider you picked, and only when you press the hotkey and ask.
- **History is off by default.** Turn it on and finished side chats are saved on this Mac only. The text of uploaded files is never saved.
- **Chat sites only.** In a browser it reads only claude.ai, chatgpt.com and gemini.google.com. Other websites are never read.
- **Files: only what was uploaded.** Side Chat looks only for files uploaded in the chat, only inside your home folder, and never in app data, hidden folders or the Trash. You can switch this off.
- **Keys stay local.** API keys and sign-ins stay in your macOS Keychain and go only to their own provider.

## Updates

Side Chat checks this page for new versions about every 6 hours. You can also choose **Check for Updates…** from its menu bar menu.

Every update is signed. Side Chat refuses any download that isn't signed with the developer's key.

---

<p align="center"><sub>This repository hosts the app downloads. Side Chat isn't affiliated with Anthropic, OpenAI or Google.</sub></p>
