# Changelog

All notable changes to the **Antigravity Remote Control** extension will be documented in this file.

## [1.2.6] - 2026-03-05

### ✨ New

- **Custom CSS Setting** — Override chat styles from IDE Settings Panel and mobile dashboard. IDE CSS + Dashboard CSS, dual source with priority
- **Settings Panel CSS Card** — Custom CSS textarea added to the extension's WebView Settings Panel (alongside PIN, Tunnel, etc.)
- **All Settings Registered** — `tunnelMode`, `tunnelName`, `customCSS` all visible in VS Code Settings UI

### 🐛 Fixed

- **Tunnel Restart Hang** — Force-kills stale `cloudflared` processes before starting new tunnel (Windows `taskkill` + macOS/Linux `pkill`)
- **Empty Div Whitespace** — Strips virtual scroller placeholder `<div></div>` that caused large gaps in chat
- **SIGKILL Fallback** — Tunnel `stop()` uses SIGTERM → waits 2s → SIGKILL if process still alive

## [1.2.0] - 2026-03-04

### 🐛 Fixed

- **Chat History Lost** — Chat accumulation fix: old messages preserved during streaming updates
- **Block Fingerprinting** — More resilient tag-based fingerprinting for stable merge

## [1.1.1] - 2026-03-05

### ✨ Improved

- **Model list auto-detects from IDE** — No more hardcoded model names. The model picker now shows the actual model you're using in real-time
- **Chat display cleaned up** — Text no longer shifts to the right, proper word wrapping, and thinner scrollbar for a cleaner reading experience
- **Input bar matches IDE look** — Mode and model pickers now visually match the IDE with `^` prefix and consistent styling

## [1.1.0] - 2026-03-04

### ✨ Improved

- **Input bar redesigned** — Flat, monochrome icons replace emoji for a cleaner IDE-like look
- **Mode/Model pickers** — Match IDE styling with caret prefix and full model names

## [1.0.98] - 2026-03-04

### 🐛 Fixed

- **Image attachment now works** — Selecting images on mobile no longer silently fails

## [1.0.95] - 2026-03-04

### ✨ Improved

- **Smoother chat updates** — Only changed messages update instead of the entire chat refreshing

## [1.0.94] - 2026-03-04

### ✨ Improved

- **Settings persist across sessions** — Language, theme, and notification preferences now survive tunnel reconnects

## [1.0.93] - 2026-03-04

### 🐛 Fixed

- **PIN input no longer resets while typing** — Background checks won't interrupt your PIN entry

## [1.0.73] - 2026-03-04

### 🐛 Fixed

- **Dashboard loads with PIN protection** — Previously showed a blank page instead of the PIN screen

## [1.0.72] - 2026-03-04

### ✨ Improved

- **Charts and diagrams display correctly** — Canvas-based visuals are now converted to images in the chat

### 🐛 Fixed

- **Chat no longer jumps to top** — Scroll position stays where you left it

## [1.0.71] - 2026-03-04

### ✨ Improved

- **Independent scrolling** — Dashboard chat scrolls freely without syncing to IDE

## [1.0.62] - 2026-03-03

### 🐛 Fixed

- **Smooth mobile scrolling** — Fixed touch scroll getting stuck on mobile devices

## [1.0.56] - 2026-03-03

### 🐛 Fixed

- **Chat loading reliability** — Fixed a bug where chat could stop updating after a connection timeout

## [1.0.54] - 2026-03-03

### 🐛 Fixed

- **Chat display errors** — Fixed a script parsing issue that prevented chat from rendering

## [1.0.50] - 2026-03-03

### 🐛 Fixed

- **macOS stability** — Settings changes no longer crash the dashboard on macOS

## [1.0.48] - 2026-03-03

### 🐛 Fixed

- **macOS tunnel setup** — Cloudflare tunnel now installs correctly on macOS

## [1.0.44] - 2026-03-03

### ✨ New

- **Attach any file type** — PDF, code files, text, CSV, and more can now be attached alongside images

### ✨ Improved

- **Smart scroll** — New floating "↓ New" button appears when there are new messages below

## [1.0.38] - 2026-03-03

### ✨ New

- **Redesigned input toolbar** — Attach, commands, mode/model selection all in one compact row
- **Better chat styling** — Tasks, diffs, code blocks, tables all properly styled

## [1.0.35] - 2026-03-03

### ✨ New

- **Workflow commands** — Type `/` to use workflows directly from your phone
- **Photo & file sharing** — Attach photos or files to your prompts with compression for fast upload
- **Easy navigation** — "← Back to Chat" button on every panel

## [1.0.31] - 2026-03-03

### ✨ New

- **Mobile-first redesign** — Bigger chat area, compact menu, and larger touch targets
- **Quick actions** — Context-aware buttons that hide when the agent is working

## [1.0.30] - 2026-03-03

### ✨ New

- **Open files from chat** — Click file references in chat to view them directly

## [1.0.29] - 2026-03-03

### 🐛 Fixed

- **Chat display improvements** — Fixed black squares, invisible buttons, and touch scrolling issues
- **iOS zoom fix** — Input fields no longer cause unwanted zoom on iPhone

## [1.0.26] - 2026-03-02

### ✨ New

- **Live chat rendering** — See your IDE conversation with full styling on your phone
- **Model & Mode control** — Switch AI models and modes remotely
- **Theme sync** — Dashboard matches your IDE's light/dark theme

## [1.0.11] - 2026-02-28

### ✨ New

- **Remote terminal** — Run commands from your phone
- **Git integration** — Check status, view diffs, commit, push, and pull remotely
- **File editor** — View and edit files with save functionality

## [1.0.0] - 2026-02-25

### 🚀 Initial Release

- Mobile dashboard for remote IDE control
- Live chat streaming from Antigravity IDE
- Accept/Reject agent suggestions remotely
- Quick action buttons (Continue, Yes, No, Stop)
- Cloudflare Tunnel for secure remote access
- Password protection
- Dark/Light theme
- File browser
