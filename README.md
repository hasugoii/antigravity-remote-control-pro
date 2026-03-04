# 🎮 Antigravity Remote Control

> 🌐 **English** | [日本語](README_JA.md) | [Tiếng Việt](README_VI.md) | [中文](README_ZH.md)

> **Your phone. Your IDE. Zero friction.**

You built something amazing with AI agents — but you're **chained to your desk** watching it work. What if you could walk away, grab a coffee, lie on the couch — and still **accept changes, send prompts, attach screenshots, and run workflows** from your phone?

**That's Remote Control.**

<p align="center">
  <img src="https://raw.githubusercontent.com/hasugoii/antigravity-remote-control-pro/main/media/mobile-dashboard.png" alt="Mobile Dashboard" width="300" />
</p>

---

## 😤 The Problem

You know the drill:

- 🪑 **Stuck at your desk** — Your AI agent is coding, but you need to approve every step
- ⏳ **Waiting... waiting...** — Agent finishes, you don't know until you check
- 📱 **Your phone is useless** — Can't accept, can't type prompts, can't see what's happening
- 🤦 **Context lost** — You step away for 5 minutes, come back to a mess

**Remote Control kills all of these.**

---

## ⚡ 3 Steps. 30 Seconds. Done

```
1. Ctrl+Shift+R    → Enable Remote Control
2. Scan QR code    → With your phone camera
3. 📱 You're in    → Full control from anywhere
```

No app to install. No account to create. Just **scan and go**.

---

## 🦁 Tiger With Wings: Remote Control + Agent Auto Approve

This is where it gets **insane**.

[**Agent Auto Approve**](https://open-vsx.org/extension/hasugoii/agent-auto-approve) auto-clicks every button in your IDE — Accept, Continue, Yes, terminal commands, file changes. **Everything.**

Now combine it with Remote Control:

| Alone | 🦁 + 🪽 Together |
|-------|-------------------|
| You click Accept manually | 🤖 Agent Auto Approve clicks **everything** for you |
| You type prompts at your desk | 📱 You type prompts **from your phone** |
| You check the IDE screen | 📸 You see **live screenshots** on your phone |
| You restart workflows manually | ⚡ You tap **one button** to run workflows |
| You can't send images to the agent | 📎 You **snap a photo** and send it directly |

> 🔥 **The result:** Your AI agent codes autonomously. You just **monitor and steer from your pocket.** True hands-free vibe coding.

👉 **[Get Agent Auto Approve](https://open-vsx.org/extension/hasugoii/agent-auto-approve)** — auto-installed as a dependency.

---

## 📎 Send Images & Files — The Killer Feature

Snap a bug screenshot. Photograph a whiteboard sketch. Send a design mockup.

**Attach it directly to your AI prompt — from your phone.**

- 📷 **Camera → AI Agent** — Take a photo, it goes straight into the conversation
- 🖼️ **Gallery pick** — Select multiple images at once
- 📄 **Any file type** — PDF, CSV, code files, text — all supported
- ⚡ **Auto-compressed** — Large images compressed via canvas for fast upload over mobile

No USB cables. No cloud uploads. No email-to-yourself. **Just tap and send.**

---

## 📱 What You Get

### A Full IDE Dashboard On Your Phone

| Tab | What It Does |
|-----|-------------|
| 💬 **Chat** | Live AI conversation with full styling — code blocks, diffs, task progress |
| 📂 **Files** | Browse, read, edit, and save workspace files |
| 💻 **Terminal** | Run commands, see build logs and errors |
| 📸 **Screenshot** | Live IDE screen capture with 5s auto-refresh |
| ⚙️ **Settings** | Theme, language, notifications, Custom CSS, git status |

### Everything You Need, One Tap Away

| Feature | Why It Matters |
|---------|---------------|
| ✅ **Accept / Reject** | Approve agent changes without touching your keyboard |
| ⌨️ **Send Prompts** | Direct your AI agent from anywhere |
| ⚡ **Workflow Commands** | Tap `/` to run any workflow — AntiKit, custom, and more |
| 📎 **Media Attachments** | Send photos and files to your AI prompt |
| 🔔 **Push Notifications** | Agent done? Error? Needs approval? Your phone buzzes |
| 🤖 **Model/Mode Switch** | Change AI model and conversation mode remotely |
| 🔀 **Git Integration** | Status, diff, commit, push — all from your phone |
| 🌙 **Dark/Light Theme** | Syncs with your IDE theme preference |
| 📜 **Smart Scroll** | Never hijacks your reading — floating "↓ New" button |
| 🎨 **Custom CSS** | Override chat styles from IDE Settings Panel or mobile |

---

## ⚙️ Settings Panel (IDE Side)

Configure everything from inside your IDE — no terminal, no config files:

<p align="center">
  <img src="https://raw.githubusercontent.com/hasugoii/antigravity-remote-control-pro/main/media/settings-panel.png" alt="Settings Panel" width="500" />
</p>

| Setting | Where |
|---------|-------|
| 🔛 **Toggle ON/OFF** | One-click enable/disable |
| 📡 **Tunnel Mode** | Quick (instant) or Named (permanent URL) |
| 🔐 **PIN Protection** | 4-6 digit PIN for extra security |
| 🎨 **Custom CSS** | Override dashboard chat styles |
| 📊 **QR Code** | Scan to connect instantly |
| 🤝 **Companion Status** | Shows if Agent Auto Approve is active |

---

## 🌐 Secure By Default

- **Cloudflare Tunnel** — End-to-end encrypted, works through firewalls and NATs
- **Session Tokens** — Auto-generated, rotate on restart
- **Optional PIN** — 4-6 digit lock for shared networks
- **Auto-download** — `cloudflared` binary installed automatically, zero config

| Mode | Best For |
|------|----------|
| **Quick Tunnel** *(default)* | Zero setup — random URL, works instantly |
| **Named Tunnel** *(advanced)* | Fixed URL with custom domain |

---

## 🌍 Use Cases

- ☕ **Coffee break** — Accept changes from the café downstairs
- 🛋️ **Couch coding** — Send prompts while watching Netflix
- 🚌 **On the bus** — Review agent output during your commute
- 🏖️ **On vacation** — Monitor your AI agent building features
- 🤳 **Bug report** — Snap a photo of the bug, send it to the agent
- 🎨 **Design review** — Photograph a whiteboard sketch, AI implements it
- 🤝 **Pair coding** — Share tunnel URL with a teammate

---

## 📋 Changelog

### v1.2.6 — Tunnel Reliability + Custom CSS + Empty Div Fix

- 🎨 **Custom CSS Setting** — Override chat styles from IDE Settings Panel AND mobile dashboard
- 🔧 **Tunnel Restart Fix** — Force-kills stale `cloudflared` processes on restart (Windows + macOS)
- 🧹 **Empty Div Cleanup** — Strips virtual scroller placeholder divs that caused large whitespace gaps
- ⚙️ **All Settings Registered** — `tunnelMode`, `tunnelName`, `customCSS` all visible in IDE Settings
- 🎮 **Settings Panel CSS** — Custom CSS textarea added to the extension's Settings Panel

### v1.2.0 — Chat History Preservation

- 📜 **Chat Accumulation Fix** — Chat history preserved during streaming (no more losing old messages)
- 🔗 **Resilient Fingerprinting** — Tag-based block matching for stable streaming updates

### v1.1.1 — IDE Parity Polish

- 🤖 **Auto-detect Models** — Model picker shows real models from IDE, no hardcoded list
- 📐 **Chat Layout Fix** — Text alignment, word wrapping, thinner scrollbar
- 🎯 **Input Bar Redesign** — Mode/model pickers match IDE styling

### v1.0.44 — Dashboard UX Polish

- 📎 **Multi-Media Attachment** — Attach & send multiple images + files from phone
- ⚡ **Workflow Commands** — Tap `/` to discover and run any workflow
- 📜 **Smart Scroll** — Floating "↓ New" button, never hijacks reading
- 📐 **Input Bar Redesign** — Flat monochrome icons, IDE-like aesthetic

### v1.0.0 — Full Release

- 🖥️ HTML Chat Rendering via CDP
- 🤖 Model/Mode Sync
- 💻 Remote Terminal
- 🔀 Git Integration
- ✏️ File Editor
- 🎨 Theme Sync
- 🔔 Push Notifications
- 📸 Screenshot Capture
- 🌐 Cloudflare Tunnel (Quick + Named)
- 🔐 Token + PIN Auth
- 📊 QR Code Connect

---

## ⌨️ Commands

| Shortcut | Action |
|----------|--------|
| `Ctrl+Shift+R` | Toggle Remote Control ON/OFF |

Command Palette: `Ctrl+Shift+P` → "Remote Control" → Toggle, Settings, Setup CDP, Show QR Code.

---

## 🔧 After IDE Updates

CDP may reset after updates. The extension auto-detects and shows a fix prompt — click **"Setup & Restart"**.

---

## 📦 Installation

### From Open VSX (Recommended)

Search **"Antigravity Remote Control"** in Extensions, or:

👉 **[Install from Open VSX](https://open-vsx.org/extension/hasugoii/antigravity-remote-control)**

### Manual Install

1. Download `.vsix` from [Releases](https://github.com/hasugoii/antigravity-remote-control/releases)
2. `Ctrl+Shift+P` → **"Install from VSIX..."**
3. Select the file → Reload

---

**Made by [hasugoii](https://open-vsx.org/namespace/hasugoii)** · **[Agent Auto Approve](https://open-vsx.org/extension/hasugoii/agent-auto-approve)** · Built for **Antigravity IDE**
