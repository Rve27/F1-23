# F1 23 My Team Career Setup

No code — just `AGENTS.md` as the single source of settings and car setup limits. Any AI reading it becomes your race engineer.

## How to Use

### 1. Open this repo in an AI
- **OpenCode:** open this folder and chat directly — the agent automatically reads `AGENTS.md`.
- **ChatGPT / Claude / Gemini:** upload or paste the contents of `AGENTS.md` and add: *"You are my F1 23 race engineer. Use only the settings and limits in this file."*

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
AGENTS.md  — settings & setup limits (main AI source)
README.md  — this file
```

## Updating Team Context & Game Settings

All configuration lives in `AGENTS.md` — edit it directly, then commit.

**Team Context** (`AGENTS.md:5-8`) — update when your career progresses:
```md
- Team: RvRacing F1 Team — Season 3 | Power Unit: Honda | Teammate: Max Verstappen
- Platform: PS4 Pro + gamepad (Rexus Gladius GX550)
- AI Difficulty: 95 (Legend) | Race Length: 50%
```

**Game Settings** (`AGENTS.md:10-29`) — keep in sync with your in-game settings:
- **Assists** (`AGENTS.md:12-15`): Traction Control, ABS, Gearbox, ERS/DRS Assist, Racing Line
- **Career** (`AGENTS.md:17-20`): Driver Moves, Facility/R&D Management, Resource Rates
- **Simulation** (`AGENTS.md:22-25`): Flashbacks, Tyre Temp, Damage, Surface Type
- **Rules & Flags** (`AGENTS.md:27-29`): Corner Cutting, Parc Fermé, Safety Car/Red Flags

Example — switching to manual gearbox and no traction control:
```md
- Traction Control: Off | Anti-Lock Brakes: Off
- Gearbox: Manual | ERS Assist: Off
```
