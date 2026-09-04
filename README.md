# F1 23 My Team Career Setup

No code — `AGENTS.md` (setup limits) + `team-context.md` (team/career state) + `game-settings.md` (assists/career/simulation/rules). Any AI reading them becomes your race engineer.

## How to Use

### 1. Open this repo in an AI
- **OpenCode:** open this folder and chat directly — the agent automatically reads `AGENTS.md`, `team-context.md`, and `game-settings.md`.
- **ChatGPT / Claude / Gemini:** upload or paste the contents of `AGENTS.md` + `team-context.md` + `game-settings.md` and add: *"You are my F1 23 race engineer. Use only the settings and limits in these files."*

### 2. Request a setup
```
Dry setup for Monza
Wet setup for Monaco, need more rear stability
Rear tyres overheating at Silverstone, here's my setup: [paste]
```

### 3. Apply in game
Copy the values from the AI's answer into the Car Setup menu in F1 23. All values are guaranteed to be within in-game limits (wing 0–50, diff 50–100%, etc.).

## Repo Contents

```
AGENTS.md        — setup limits & repo notes (main AI source)
team-context.md  — team/career state (team, PU, teammate, difficulty)
game-settings.md — assists, career, simulation, rules & flags
README.md        — this file
```

## Updating Team Context & Game Settings

All configuration lives in `team-context.md` + `game-settings.md` + `AGENTS.md` — edit them directly, then commit.

**Team Context** (`team-context.md`) — update when your career progresses:
```md
- Team: RvRacing F1 Team — Season 3 | Power Unit: Honda | Teammate: Max Verstappen
- Platform: PS4 Pro + gamepad (Rexus Gladius GX550)
- AI Difficulty: 95 (Legend) | Race Length: 50%
```

**Game Settings** (`game-settings.md`) — keep in sync with your in-game settings:
- **Assists** (`game-settings.md:3-6`): Traction Control, ABS, Gearbox, ERS/DRS Assist, Racing Line
- **Career** (`game-settings.md:8-11`): Driver Moves, Facility/R&D Management, Resource Rates
- **Simulation** (`game-settings.md:13-16`): Flashbacks, Tyre Temp, Damage, Surface Type
- **Rules & Flags** (`game-settings.md:18-20`): Corner Cutting, Parc Fermé, Safety Car/Red Flags

Example — switching to manual gearbox and no traction control:
```md
- Traction Control: Off | Anti-Lock Brakes: Off
- Gearbox: Manual | ERS Assist: Off
```
