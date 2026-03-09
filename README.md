# ⚔️ KitPvP Plugin

A custom **KitPvP plugin** for Minecraft multiplayer servers built with **Java** and the **Spigot API**. Players can choose from a variety of combat kits and fight each other in an action-packed PvP arena.

---

## 🧩 Features

- 🗡️ **Multiple Kits** — Choose from unique kits like Warrior, Archer, Tank, and more
- 📊 **Kill / Death Tracking** — Tracks each player's kills and deaths per session
- 🏆 **Leaderboard** — Top players ranked by kills
- ⚙️ **Custom Commands** — Simple commands to select kits, check stats, and manage the game
- 🔁 **Respawn System** — Players respawn automatically with their selected kit
- 🛡️ **Kit Cooldowns** — Prevent kit spam with configurable cooldown timers
- 💬 **Custom Messages** — Fully customizable kill messages and broadcasts

---

## 🚀 Installation

1. Download the latest `KitPvP.jar` from [Releases](../../releases)
2. Drop it into your server's `/plugins` folder
3. Restart or reload your server
4. Configure the plugin in `plugins/KitPvP/config.yml`

---

## 🛠️ Commands

| Command | Description | Permission |
|--------|-------------|------------|
| `/kit` | Open the kit selection menu | `kitpvp.kit` |
| `/kit <name>` | Select a specific kit | `kitpvp.kit` |
| `/stats` | View your kill/death stats | `kitpvp.stats` |
| `/stats <player>` | View another player's stats | `kitpvp.stats` |
| `/leaderboard` | Show top players | `kitpvp.leaderboard` |
| `/kitpvp reload` | Reload the config | `kitpvp.admin` |

---

## 🔐 Permissions

| Permission | Description |
|-----------|-------------|
| `kitpvp.kit` | Access to kit selection |
| `kitpvp.stats` | Access to stats command |
| `kitpvp.leaderboard` | Access to leaderboard |
| `kitpvp.admin` | Access to admin commands |
| `kitpvp.*` | All permissions |

---

## ⚙️ Configuration

```yaml
# config.yml

settings:
  prefix: "&8[&bKitPvP&8] &r"
  spawn: world,0,64,0   # Set your spawn coordinates
  kit-cooldown: 30       # Seconds before switching kits again

kits:
  warrior:
    enabled: true
  archer:
    enabled: true
  tank:
    enabled: true
```

---

## 📦 Requirements

- **Java** 8 or higher
- **Spigot / Paper** 1.8 – 1.20
- No external dependencies

---

## 🏗️ Built With

| Tech | Purpose |
|------|---------|
| Java | Core plugin logic |
| Spigot API | Minecraft server integration |
| Maven | Build & dependency management |

---

## 📁 Project Structure

```
KitPvP/
├── src/
│   └── main/
│       └── java/
│           └── dev/shubhansh/kitpvp/
│               ├── KitPvP.java          # Main plugin class
│               ├── commands/            # Command handlers
│               ├── kits/                # Kit definitions
│               ├── listeners/           # Event listeners
│               └── managers/            # Stats & player managers
├── resources/
│   ├── plugin.yml
│   └── config.yml
└── pom.xml
```

---

## 🤝 Contributing

Pull requests are welcome! If you find a bug or have a feature idea, open an issue.

1. Fork the repo
2. Create your branch: `git checkout -b feature/my-feature`
3. Commit your changes: `git commit -m 'Add my feature'`
4. Push: `git push origin feature/my-feature`
5. Open a Pull Request

---

## 👤 Author

**Shubhansh** — 16-year-old developer from India  
🌐 [Portfolio](https://shubhansh9.github.io/Shubhansh/) · 📧 shubhanshs90@gmail.com · 🐙 [GitHub](https://github.com/shubhansh9)

---

## 📄 License

This project is open source under the [MIT License](LICENSE).

---

<p align="center">Made with ☕ and ambition</p>
