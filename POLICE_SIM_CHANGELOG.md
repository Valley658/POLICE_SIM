# Police Simulator - Changelog

---

## v1.4.0 (2026-03-03)

### Bug Fixes
- **Criminal kill crash fix**: `util.yield(3000)` was called inside a reverse for-loop, corrupting table indices and causing crashes. Deferred cleanup is now handled safely via `util.create_thread`.
- **Bounty target kill crash fix**: Same yield-in-loop pattern was present in bounty target processing, causing identical crashes.
- **SWAT deploy message trailing space fix**: Removed trailing space in `T("SWAT team deployed! ")` which caused translation key mismatch.

### New Features
- **Logging system**: All activity is now logged to `store\Police Simulator\Log.txt` with timestamps.
  - Categories: SYSTEM, DUTY, RADIO, ARREST, KILL, RANK, VEHICLE, CRIME
  - Format: `[YYYY-MM-DD HH:MM:SS] [CATEGORY] message`
  - Logged events: script start/stop, duty start/end, arrests, kills, promotions, vehicle spawns, crime events, language changes, and all radio messages.

### Improvements
- **Enhanced language auto-detection**: 3-tier detection system.
  1. `lang.get_current()` (Stand API)
  2. `menu.get_language()` (compatibility with some Stand versions)
  3. OS locale-based detection (final fallback)
- **UTF-8 BOM handling**: Automatic BOM (Byte Order Mark) removal when loading language files.
- **Language file parsing improvement**: Automatic trimming of leading/trailing whitespace on keys and values for more robust parsing.

---

## v1.3.0

### New Features
- **K9 Unit**: Police dog companion system.
  - Deploy / dismiss / attack / follow commands
  - Auto-attack nearest criminal
  - Minimap blip tracking
- **SWAT Raid**: SWAT tactical team deployment.
  - Deploys with tactical vehicle (Police Riot)
  - Up to 10 SWAT operators
  - Heavy weapons + body armor
- **Undercover Mode**: Disguise as civilian.
  - Toggle between uniform and civilian clothes
  - Spawn random civilian vehicle
- **Smoke Grenade**: Blind nearby criminals.
  - Temporarily stops criminal combat
  - Induces flee behavior
- **Speed Trap**: Stationary speed enforcement.
  - Configurable speed limit (30–200 km/h)
  - Auto-detect speeding vehicles and issue fines
  - Fines convert to rank points
- **Prisoner Transport**: Escort arrested criminals for bonus points.
  - Follow GPS to destination
  - Bonus points on successful delivery
  - Cancellable mid-mission
- **Difficulty System**: 4 difficulty presets.
  - Easy: 15% accuracy, x0.5 health, 50% flee
  - Normal: 30% accuracy, x1.0 health, 30% flee
  - Hard: 50% accuracy, x2.0 health, 15% flee
  - Extreme: 80% accuracy, x3.0 health, 5% flee

---

## v1.2.0

### New Features
- **Tactical Menu**:
  - Spike Strip: Deploy on roads to burst vehicle tires (max 10)
  - Roadblock: Set up / remove police barricades
  - Flashbang: Stun nearby criminals (stops combat + forces surrender)
  - Warning Shot: Fire into the air to intimidate / cause criminals to flee
- **Backup & Support**:
  - Backup Units: Call in police NPC reinforcements (up to 8)
  - Police Helicopter: Deploy Air Maverick for air support, auto-engages criminals
- **Traffic Stop**:
  - Pull over vehicle ahead
  - Order driver out
  - End stop (release vehicle)
- **Bounty Board**:
  - Generate high-value most-wanted targets
  - Reward points on elimination (3–8 pts)
  - Configurable max bounty targets (up to 10)
- **Rank System**:
  - 9 ranks: Cadet → Officer → Corporal → Sergeant → Lieutenant → Captain → Commander → Deputy Chief → Chief of Police
  - Earn points from arrests (3 pts), kills (1 pt), wave clears, etc.
  - View current rank and progress

---

## v1.1.0

### Features
- **Police Mode (Duty)**:
  - 7 police uniforms (Patrol Officer, Highway Patrol, Sheriff, SWAT, FIB)
  - Start / end duty (character swap / restore)
  - Auto weapon loadout (Pistol, Shotgun, SMG, Taser, Nightstick, Flashlight)
- **Patrol Vehicle**:
  - 11 vehicles: Police Car 1–3, Police Muscle, Unmarked, Sheriff 1–2, FBI, FBI SUV, Police Bike, Van
  - Siren toggle, repair, delete
  - Partner NPC auto-boards (when enabled)
- **Crime Response**:
  - 10 randomized crime event types
  - Arrest criminals (approach → handcuff animation → fade-out)
  - Chase criminals (vehicle / on foot)
  - Remove all criminals
- **Wave Mode**:
  - Continuous crime waves (progressively increasing)
  - Auto-starts next wave on clear
- **Settings**:
  - Crime detection range, interval, arrest range
  - Criminal accuracy / health / flee chance / vehicle chance
  - Player invincible / auto heal / clear wanted level
  - Patrol vehicle invincible / partner weapon selection
  - Minimap blips / radio alerts / debug info toggles
- **Multilingual support**: English, Korean, Chinese, Japanese
- **Auto crime detection**: Periodic automatic crime event generation

---

## v1.0.0

### Initial Release
- Base police simulator framework
- Stand mod menu integration
- Pluto (Lua superset) scripting
- Settings save / load system
- Language file system foundation
