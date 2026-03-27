# <p align="center">📬 DCI Modmail</p>

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=38BDF8&center=true&vCenter=true&width=500&lines=DCI+Modmail+Bot;Open+Source+%7C+Self+Hostable;Modern+Discord+Modmail+Solution;Built+by+DCI+Studios" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Coming_Soon-yellow?style=for-the-badge" />
  <img src="https://img.shields.io/badge/License-MIT-38BDF8?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Built_With-Discord.js-5865F2?style=for-the-badge&logo=discord&logoColor=white" />
  <img src="https://img.shields.io/badge/Node.js-18%2B-339933?style=for-the-badge&logo=node.js&logoColor=white" />
</p>

---

## 📖 Overview

**DCI Modmail** is a free, open-source Discord modmail bot developed by [DCI Studios](https://dcistudios.xyz). It provides a clean and reliable bridge between your server members and your moderation team — all through private Discord threads.

> ⚠️ **This repository is currently in pre-release.** The full source code will be published when officially announced by DCI Studios. File structure is provided below for transparency and community preparation.

---

## ✨ Planned Features

- 📩 Private DM-to-thread modmail system
- 🏷️ Ticket tagging and categorization
- 📝 Full transcript logging
- 🔒 Role-based access control
- ⚙️ Per-server configuration
- 🔔 Customizable open/close messages
- 📊 Ticket statistics and history
- 🚫 User blocklist support
- 🌐 Multi-server support

---

## 🗂️ File Structure

> The following layout represents the planned project structure ahead of the public release.
```
dci-modmail/
│
├── src/
│   ├── commands/
│   │   ├── modmail/
│   │   │   ├── close.js          # Close an active modmail thread
│   │   │   ├── reply.js          # Reply to a modmail thread
│   │   │   ├── silentReply.js    # Reply without notifying the user
│   │   │   └── transcript.js     # Generate a transcript of a thread
│   │   │
│   │   ├── admin/
│   │   │   ├── setup.js          # Initial bot setup command
│   │   │   ├── config.js         # View/edit bot configuration
│   │   │   ├── block.js          # Block a user from using modmail
│   │   │   └── unblock.js        # Unblock a user
│   │   │
│   │   └── utility/
│   │       ├── ping.js           # Check bot latency
│   │       └── stats.js          # View ticket statistics
│   │
│   ├── events/
│   │   ├── messageCreate.js      # Handles incoming DMs and thread replies
│   │   ├── threadCreate.js       # Fires when a new modmail thread opens
│   │   ├── threadDelete.js       # Fires when a thread is deleted
│   │   ├── interactionCreate.js  # Handles slash command interactions
│   │   └── ready.js              # Bot ready event
│   │
│   ├── handlers/
│   │   ├── commandHandler.js     # Loads and registers slash commands
│   │   ├── eventHandler.js       # Loads and registers event listeners
│   │   └── threadHandler.js      # Core modmail thread logic
│   │
│   ├── utils/
│   │   ├── logger.js             # Console and file logging utility
│   │   ├── embed.js              # Shared embed builder helpers
│   │   ├── transcript.js         # Transcript generation utility
│   │   └── permissions.js        # Permission checking helpers
│   │
│   ├── config/
│   │   ├── config.js             # Loads and validates configuration
│   │   └── defaults.js           # Default configuration values
│   │
│   └── index.js                  # Bot entry point
│
├── data/
│   ├── transcripts/              # Saved ticket transcripts (auto-generated)
│   └── database/                 # Local database storage (auto-generated)
│
├── .env.example                  # Example environment variables
├── .gitignore
├── config.yml.example            # Example bot configuration file
├── package.json
├── LICENSE
└── README.md
```

---

## ⚙️ Configuration (Preview)

Below is a preview of the planned `config.yml` structure:
```yaml
bot:
  prefix: "!"
  status: "Watching for messages"

modmail:
  guild_id: "YOUR_SERVER_ID"
  category_id: "YOUR_CATEGORY_ID"
  log_channel_id: "YOUR_LOG_CHANNEL_ID"
  staff_role_id: "YOUR_STAFF_ROLE_ID"

messages:
  open: "Your message has been received. Our team will respond shortly."
  close: "Your modmail thread has been closed. Thank you for reaching out."

transcripts:
  enabled: true
  save_locally: true
```

---

## 🚀 Self-Hosting (Coming Soon) 
---

## 🧠 Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=js,nodejs,github,linux" />
</p>

| Technology | Purpose |
|---|---|
| Node.js | Runtime environment |
| Discord.js v14 | Discord API wrapper |
| JavaScript | Primary language |
| YAML | Configuration format |
| JSON / SQLite | Data storage |

---

## 📢 Release Notice

DCI Modmail will be made fully public when:

- ✅ Core modmail functionality is complete
- ✅ Self-hosting documentation is written
- ✅ Stability testing is finished
- ✅ Official announcement is made by DCI Studios

---

## 🔐 License

This project will be released under the **MIT License** — free to use, modify, and self-host.

---

## 🌐 Official Links

<p align="center">
  <a href="https://dcistudios.xyz">
    <img src="https://img.shields.io/badge/DCI_Studios-Website-38BDF8?style=for-the-badge" />
  </a>
  <a href="https://hosting.dcistudios.xyz">
    <img src="https://img.shields.io/badge/DCI_Hosting-Infrastructure-0EA5E9?style=for-the-badge" />
  </a>
  <a href="https://forums.dcistudios.xyz">
    <img src="https://img.shields.io/badge/DCI_Forums-Community-8B5CF6?style=for-the-badge" />
  </a>
  <a href="https://thecarter.xyz">
    <img src="https://img.shields.io/badge/Carter-Portfolio-6366F1?style=for-the-badge" />
  </a>
</p>

---

## 📬 Contact

<p align="center">
  <a href="mailto:developer@dcistudios.xyz">
    <img src="https://img.shields.io/badge/Email-developer@dcistudios.xyz-D14836?style=flat-square&logo=gmail&logoColor=white" />
  </a>
</p>

---

## 👑 Credits

**Lead Developer:** Carter
**Organization:** DCI Studios

---

<p align="center">
<b>DCI Studios — Architecting Excellence.</b>
</p>
