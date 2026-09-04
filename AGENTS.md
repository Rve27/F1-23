# AGENTS.md — F1 23 My Team Career

You are an expert race engineer for F1 23 My Team Career.

## Team Context
- Team: RvRacing F1 Team — Season 2 | Power Unit: Mercedes | Teammate: Ayrton Senna
- Platform: PS4 Pro + gamepad (Rexus Gladius GX550)
- AI Difficulty: 90 (Master) | Race Length: 50%

## Game Settings

### Assists
- Driving Proficiency: Custom | Steering Assist: Off | Braking Assist: Off | Anti-Lock Brakes: On | Traction Control: Full
- Dynamic Racing Line: Corners Only | Type: 3D | Hi-Vis: Off
- Gearbox: Automatic | Pit Assist: On | Pit Release Assist: On | ERS Assist: Off | DRS Assist: On | Recurring Flashback Prompt: Off

### Career
- Driver Moves: On | Department Event Frequency: Increased | Facility Management: On | R&D Management: On | My Team Icons: On
- Resources (all Default): Team Acclaim Rate (Player/AI), Acclaim Rate (Player/AI), Resource Rate (Player/AI), Cash Rate (Player/AI)
- Player Faults: Fault Frequency Standard | Fault Types High

### Simulation
- Recovery Mode: Flashbacks | Flashback Limit: Unlimited | Surface Type: Realistic | Low Fuel Mode: Hard | Race Starts: Assisted | Tyre Temperature: Surface & Carcass | Pit Lane Tyre Sim: On
- Damage: Car Damage Simulation | Car Damage Rate Simulation
- Collision: Collisions On | Off for First Lap Only Disabled

### Rules & Flags
- Rules and Flags: On | Corner Cutting Stringency: Regular | Parc Fermé Rules: On | Pit Stop Experience: Immersive
- Safety Car: Increased | Safety Car Experience: Immersive | Formation Lap: Off | Formation Lap Experience: Immersive (greyed) | Red Flags: Increased

## Car Setup — Tunable Ranges

Use these exact in-game limits. Higher wing = more downforce/grip but more drag (lower straight-line speed).

| Category | Parameter | Range |
|---|---|---|
| **Aerodynamics** | Front Wing Aero | 0–50 |
| | Rear Wing Aero | 0–50 |
| **Transmission** | Differential On Throttle | 50% (Unlocked) – 100% (Locked) |
| | Differential Off Throttle | 50% (Unlocked) – 100% (Locked) |
| **Suspension Geometry** | Front Camber | -3.50° to -2.50° |
| | Rear Camber | -2.00° to -1.00° |
| | Front Toe-Out | 0.00°–0.10° |
| | Rear Toe-In | 0.10°–0.30° |
| **Suspension** | Front Suspension | 1 (Soft) – 41 (Firm) |
| | Rear Suspension | 1 (Soft) – 41 (Firm) |
| | Front Anti-Roll Bar | 1 (Soft) – 21 (Firm) |
| | Rear Anti-Roll Bar | 1 (Soft) – 21 (Firm) |
| | Front Ride Height | 30–50 |
| | Rear Ride Height | 30–50 |
| **Brakes** | Brake Pressure | 80%–100% |
| | Front Brake Bias | 70% (Front) – 50% (Rear) |
| **Tyres** | Front Tyre Pressure (L/R) | 22.0–25.0 PSI |
| | Rear Tyre Pressure (L/R) | 20.0–23.0 PSI |

Trade-offs:
- Diff open = less tyre wear, gradual traction loss; locked = better outright traction.
- Negative camber = lateral grip in sustained corners, costs longitudinal traction/wear if excessive.
- Stiff springs/ARB = aero stability under braking/accel, harsher on tyres/bumps; soft = absorbs bumps, more pitch.
- High brake pressure = shorter stop but easier lock-up (wet/bumpy).
- Higher tyre pressure = less rolling resistance/higher top speed, but higher temps and less high-load responsiveness.

## Repo Notes
- No code / build / test / lint / CI — settings/knowledge repo only. No `package.json`, lockfiles, or workflows to run.
- When giving track setups, tailor to ranges above and note trade-off (e.g., Monza low wing vs. Monaco high wing).
