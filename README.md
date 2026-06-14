<div align="center">

# 🎮 2D Micro Game

### A classic 2D side-scrolling platformer built with Unity 6

[![Unity](https://img.shields.io/badge/Unity-6000.4.4f1-black?style=for-the-badge&logo=unity)](https://unity.com/)
[![C#](https://img.shields.io/badge/C%23-Scripts-239120?style=for-the-badge&logo=csharp)](https://docs.microsoft.com/en-us/dotnet/csharp/)
[![Platform](https://img.shields.io/badge/Platform-WebGL%20%7C%20PC-blue?style=for-the-badge)](https://unity.com/)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

<br/>

### 🌐 [▶ Play in Browser](https://play.unity.com/en/games/9bf8fafb-3b5d-49c7-af1d-8495b5b6fab8/web-build)

<br/>

</div>

---

## 🕹️ About the Game

**2D Micro Game** is a fast-paced, sprite-based side-scrolling platformer where every second counts. Run, jump, and stomp your way through a handcrafted level filled with patrolling enemies, hidden tokens, and death zones — all set to an immersive chiptune soundtrack.

The game blends tight, responsive controls with classic platformer design, challenging players to think on their feet while navigating obstacles and outsmarting enemies. Whether you're jumping over gaps, collecting tokens scattered across the environment, or bouncing on an enemy's head to defeat it — every move feels punchy and satisfying.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🏃 **Fluid Player Movement** | Smooth kinematic movement with responsive left/right control and variable-height jumping |
| 👾 **Enemy AI** | Enemies patrol fixed paths and react when the player steps on them or walks into them |
| 💀 **Health System** | Both the player and enemies have HP — stomp once to stun, twice to defeat tougher foes |
| 🪙 **Token Collection** | Animated collectibles are scattered throughout the level for players to discover |
| 🏁 **Victory Zone** | Reach the end of the level to trigger the win condition |
| ⚠️ **Death Zones** | Fall off the world and you're done — instant respawn at the last spawn point |
| 💥 **Bounce Pads & Speed Pads** | Environmental power-ups that launch or accelerate the player across the map |
| 🎵 **Full Audio Design** | Jump, land, collect, hurt, and death sounds plus background music throughout |
| 🎨 **Parallax Backgrounds** | Multi-layered scrolling backgrounds for a sense of depth and visual polish |
| 🌐 **WebGL Build** | Playable directly in the browser — no install required |

---

## 🎬 Screenshots

<div align="center">

![Gameplay Overview](https://i.ibb.co/7tkpj8h7/Screenshot-2026-06-14-113449.png)

<br/>

![Starting Screen](https://i.ibb.co/TxFxsD8h/Screenshot-2026-06-14-113537.png)

<br/>

![Character Death](https://i.ibb.co/Rk2LNBgy/Screenshot-2026-06-14-113625.png)

</div>

---

## 🎮 Controls

| Input | Action |
|---|---|
| `A` / `D` or `←` / `→` | Move left / right |
| `Space` | Jump (hold to jump higher) |
| Release Jump | Cut jump short mid-air |

> 💡 **Pro tip:** Jump and hold to reach full height. Tap quickly for a short hop. Land on top of an enemy to deal damage — side collisions will hurt *you*.

---

## 🧩 Game Mechanics

### 🦸 Player
The player character is a kinematic sprite with physics-driven movement. You move at a max horizontal speed and can perform **variable-height jumps** — holding the jump button extends the jump arc, while releasing it early cuts it short. The player spawns at a defined spawn point and respawns there on death.

### 👾 Enemies
Enemies patrol back and forth along pre-defined patrol paths at half the player's max speed. When the player **lands on top** of an enemy, it loses HP and the player bounces upward. If the player **hits an enemy from the side**, the player dies instantly.

### 🪙 Tokens
Tokens are animated collectibles placed throughout the level. Each one plays a collection animation when picked up before disappearing. They are managed by a central controller that batch-animates all tokens in the scene efficiently.

### ⚠️ Death & Respawn
Falling into a **Death Zone** (off-screen bottomless pit) or colliding with an enemy from the side triggers player death — the death sound plays, the character despawns, and the player respawns at the configured spawn point.

### 🏁 Victory
Reaching the **Victory Zone** at the end of the level triggers the win state, completing the game.

---

## 🗂️ Project Structure

```
2D-micro-game/
├── Assets/
│   ├── Scripts/
│   │   ├── Core/          # Simulation engine, event queue, fuzzy logic
│   │   ├── Mechanics/     # Player, enemy, health, tokens, game controller
│   │   ├── Gameplay/      # Game events (death, jump, collision, victory)
│   │   ├── Model/         # Shared data model (PlatformerModel)
│   │   ├── View/          # Parallax layers, animated tiles
│   │   └── UI/            # HUD and meta-game UI controllers
│   ├── Scenes/            # Main game scene (SampleScene)
│   ├── Audio/             # SFX + background music
│   ├── Character/         # Player & enemy sprites and animations
│   ├── Environment/       # Tilemap sprites and animated tiles
│   ├── Tiles/             # Tile palette assets
│   ├── Prefabs/           # Reusable game object prefabs
│   └── Mod Assets/        # Props, bounce pads, speed pads, particle effects
├── Web Build/             # Exported WebGL build (playable in browser)
└── ProjectSettings/       # Unity project configuration
```

---

## 🛠️ Built With

- **[Unity 6](https://unity.com/)** `6000.4.4f1` — Game engine
- **[Universal Render Pipeline (URP)](https://docs.unity3d.com/Packages/com.unity.render-pipelines.universal@latest)** — Rendering pipeline with post-processing
- **[Cinemachine 3](https://docs.unity3d.com/Packages/com.unity.cinemachine@latest)** — Dynamic camera follow system
- **[Unity Input System](https://docs.unity3d.com/Packages/com.unity.inputsystem@latest)** — Modern input handling
- **[TextMesh Pro](https://docs.unity3d.com/Manual/TextMeshPro.html)** — UI text rendering
- **C#** — All game logic scripted in C#

---

## 👨‍💻 Developer

<div align="center">

**Rayyan Zafar Jaffery**

[![GitHub](https://img.shields.io/badge/GitHub-rzjaffery-181717?style=for-the-badge&logo=github)](https://github.com/rzjaffery)

</div>

---

<div align="center">

*Made with ❤️ and Unity*

</div>
