# 🎯 AI-AimTrainer | Adaptive FPS Training Environment (Unity 6)

An intelligent, real-time adaptive first-person aim trainer developed with **Unity 6** and the **Universal Render Pipeline (URP)**. This trainer dynamically analyzes player targeting performance (reaction latency, accuracy, and hit/miss rates) and adapts target parameters in real-time utilizing **Fitts' Law**.

---

## 🌟 Core Features

- **Adaptive AI Difficulty Engine (Fitts' Law)**: Dynamically adjusts target diameter, distance scaling, lifetime duration, and spawn pacing based on player aiming metrics.
- **FPS Controller Architecture**: Smooth first-person movement mechanics including walking, sprinting, jump physics, crouch mechanics, and customizable mouse sensitivity.
- **Dynamic Weapons System**: Weapons with realistic projectile ballistics, recoil impulses, muzzle flash VFX, and impact particle effects.
- **3D Training Grounds**: Custom training arena designed for spatial aiming, reflex testing, and target tracking drills.
- **High-Definition Graphics**: Built using Unity's modern **Universal Render Pipeline (URP 17.5+)** with volumetric lighting, post-processing, and bloom.
- **Real-Time HUD**: On-screen dynamic HUD providing feedback on hit indicators, crosshairs, ammo counters, and performance statistics.

---

## 🛠️ System Specifications

- **Engine Version**: Unity 6 (`6000.5.7f1` or later)
- **Render Pipeline**: Universal Render Pipeline (URP 17.5.0)
- **Navigation System**: AI Navigation (`2.0.14`)
- **Text & Interface**: TextMesh Pro / uGUI (`2.5.0`)
- **Platform**: Windows Standalone (x86_64)

---

## 📂 Project Architecture

```text
AI-AimTrainer/
├── Assets/
│   ├── FPS/                    # Core gameplay, weapons, player controller, audio, & UI
│   │   ├── Prefabs/            # Player rig, weapon models, target actors
│   │   ├── Scenes/             # MainScene, IntroMenu, WinScene, LoseScene
│   │   └── Scripts/            # AI spawner, gameplay math, and HUD systems
│   ├── ModAssets/              # Shaders, custom materials, textures, and models
│   ├── NavMeshComponents/      # AI navigation surfaces and pathfinding
│   └── Rendering/              # URP graphics assets and post-processing volumes
├── Packages/                   # Package manifest & dependencies
├── ProjectSettings/            # Input axes, physics configuration, and graphics pipeline
├── Builds/                     # [Local] Standalone Windows executable builds
├── .gitignore                  # Production Unity gitignore
└── README.md                   # Documentation
```

---

## 🎮 Getting Started

1. Clone or open the repository folder in **Unity Hub**.
2. Select **Unity 6 (6000.5.7f1)** as the Editor version.
3. Open the project in Unity Editor.
4. In the Project browser, navigate to `Assets/FPS/Scenes/` and open **`MainScene.unity`** (or `IntroMenu.unity`).
5. Click the **Play (▶️)** button to begin training.

### Default Controls
| Action | Key / Input |
|---|---|
| Move | `W`, `A`, `S`, `D` |
| Look | Mouse |
| Fire / Shoot | Left Mouse Button |
| Jump | `Space` |
| Sprint | `Left Shift` |
| Crouch | `Left Ctrl` / `C` |
| Pause / Menu | `Escape` |
