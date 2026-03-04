# 🚔 Police Simulator

**GTA V Police Role-Play Script for Stand Mod Menu**

[![Version](https://img.shields.io/badge/version-1.6.2-blue.svg)](https://github.com/Valley658/POLICE_SIM/releases/latest)
[![License](https://img.shields.io/badge/license-Free-green.svg)](#)
[![Languages](https://img.shields.io/badge/languages-12-orange.svg)](#-supported-languages)

---

## 📋 Overview

Police Simulator is a comprehensive police role-play script for GTA V via the [Stand Mod Menu](https://stand.gg). 
Put on a uniform, patrol the streets, respond to crimes, and climb the ranks from **Cadet** to **Chief of Police**.

---

## ✨ Features

### 🎯 Core
- **Duty System** — Start/End duty with 7 police uniforms
- **Patrol Vehicles** — 11 vehicles (Police Car, Sheriff, FBI, Bike, etc.)
- **Crime Response** — Random crime events with radio alerts
- **Wave Mode** — Survive escalating waves of criminals
- **Partner System** — AI partner rides along with customizable weapons

### ⚔️ Tactical
- **Spike Strips** — Burst criminal vehicle tires
- **Roadblocks** — Set up police barricades
- **Flashbang** — Stun nearby criminals
- **Smoke Grenade** — Blind criminals with smoke
- **Warning Shot** — Intimidate suspects into fleeing

### 🛡️ Backup & Support
- **Backup Units** — Call up to 4 police backup units
- **Helicopter** — Air support with police helicopter
- **SWAT Raid** — Deploy tactical SWAT team (up to 6 operators)
- **K9 Unit** — Police dog companion (attack / follow commands)

### 🔍 Operations
- **Traffic Stop** — Pull over vehicles, order drivers out
- **Speed Trap** — Set up speed enforcement with fines
- **Undercover Mode** — Switch to civilian clothes & vehicle
- **Prisoner Transport** — Transport arrested prisoners for bonus points
- **Bounty Board** — Track and eliminate high-value targets
- **Emergency Calls** — Respond to 6 types of urgent emergencies
- **DUI Checkpoint** — Set up sobriety checkpoints
- **Suspect Search** — Search pedestrians for contraband
- **Escort Mission** — VIP protection escort missions
- **Police Boat** — Water patrol capability

### 📊 Progression
- **Rank System** — 9 ranks from Cadet to Chief of Police
- **Difficulty Presets** — Easy / Normal / Hard / Extreme
- **Duty Stats** — Track arrests, kills, and duty time
- **Logging System** — Automatic event logging with per-session log files

---

## 📥 Installation

### Step 1 — Find Your Stand Directory

Your Stand folder is located at:

```
%appdata%\Stand
```

You can also open it by pressing `Win + R`, then typing `%appdata%\Stand` and pressing Enter.

### Step 2 — Install the Script File

Copy **`POLICE_SIM.pluto`** into the **`Lua Scripts`** folder:

```
Stand/
└── Lua Scripts/
    └── 📄 POLICE_SIM.pluto   ← Put here
```

### Step 3 — Install the Store Folder

Copy the **`Police Simulator`** folder into the **`store`** folder:

```
Stand/
└── store/
    └── Police Simulator/     ← Put this entire folder here
        ├── Language/
        │   ├── English.txt
        │   ├── Korean.txt
        │   ├── Chinese.txt
        │   ├── Japanese.txt
        │   ├── Spanish.txt
        │   ├── French.txt
        │   ├── German.txt
        │   ├── Italian.txt
        │   ├── Portuguese.txt
        │   ├── Russian.txt
        │   ├── Polish.txt
        │   └── Vietnamese.txt
        └── Setting/
            └── Setting.txt
```

### Step 4 — Launch

1. Open **GTA V** with **Stand** injected
2. Open the Stand menu
3. Go to **`Lua Scripts`** → **`POLICE_SIM`**
4. Select **`Start Duty`** to begin patrol!

---

## 📁 Final Folder Structure

```
%appdata%\Stand/
├── Lua Scripts/
│   └── POLICE_SIM.pluto
└── store/
    └── Police Simulator/
        ├── Language/
        │   ├── English.txt
        │   ├── Korean.txt
        │   └── ... (12 language files)
        ├── Setting/
        │   └── Setting.txt
        ├── Image/           (auto-created)
        └── logs/            (auto-created, per-session log files)
```

---

## 🌐 Supported Languages

| Language | File |
|----------|------|
| 🇺🇸 English | `English.txt` |
| 🇰🇷 한국어 | `Korean.txt` |
| 🇨🇳 中文 | `Chinese.txt` |
| 🇯🇵 日本語 | `Japanese.txt` |
| 🇪🇸 Español | `Spanish.txt` |
| 🇫🇷 Français | `French.txt` |
| 🇩🇪 Deutsch | `German.txt` |
| 🇮🇹 Italiano | `Italian.txt` |
| 🇧🇷 Português | `Portuguese.txt` |
| 🇷🇺 Русский | `Russian.txt` |
| 🇵🇱 Polski | `Polish.txt` |
| 🇻🇳 Tiếng Việt | `Vietnamese.txt` |

The script **automatically detects** your Stand/OS language on first launch. 
You can also change the language manually via the in-game menu.

---

## 🎖️ Rank System

| Rank | Points Required |
|------|----------------|
| Cadet | 0 |
| Officer | 10 |
| Corporal | 25 |
| Sergeant | 50 |
| Lieutenant | 100 |
| Captain | 200 |
| Commander | 350 |
| Deputy Chief | 500 |
| Chief of Police | 750 |

Earn points by arresting criminals, completing bounties, delivering prisoners, and more.

---

## 📝 Changelog

See [Releases](https://github.com/Valley658/POLICE_SIM/releases) for the full changelog.

---

## ⚙️ Requirements

- **[Stand Mod Menu](https://stand.gg)** (Regular or above)
- **GTA V** (PC)

---

## 📜 License

Free to use. Do not resell.

---

**Made by Valley658**
