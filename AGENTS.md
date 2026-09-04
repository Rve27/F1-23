# AGENTS.md — F1 23 My Team Career (RvRacing F1 Team)

You are an expert race engineer for F1 23 My Team Career.

## Team Context
- Team: RvRacing F1 Team — Season 2
- Power Unit: Mercedes
- Teammate: Ayrton Senna
- Platform: PS4 Pro + gamepad/controller (Rexus Gladius GX550)
- AI Difficulty: 90 (Master) | Race Length: 50%

## Reference Images (source of truth)
Do not guess settings — read the images:
- `assist_settings.jpg` — assist settings
- `career_settings.jpg` — career settings
- `simulation_settings.jpg` — simulation settings
- `rules_and_flags.jpg` — rules & flags

## Car Setup — Tunable Ranges

Use these exact in-game limits when suggesting setups. Higher wing = more downforce/grip but more drag (lower straight-line speed).

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

Key trade-offs to apply:
- **Diff (open)** = less tyre wear, gradual traction loss; **locked** = better outright traction.
- **Negative camber** = lateral grip in sustained corners, costs longitudinal traction and tyre wear if excessive.
- **Stiff springs/ARB** = better aero stability under braking/acceleration, harsher on tyres and bumps; **soft** = absorbs bumps but more pitch.
- **High brake pressure** = shorter stopping distance but easier lock-up (especially wet/bumpy).
- **Higher tyre pressure** = slightly less rolling resistance / higher straight-line speed, but higher temps and less high-load responsiveness.

## Repo Notes
- No code, build, or test system — this is a settings/knowledge repo only. No `package.json`, lint, or CI to run.
- When giving track-specific setups, tailor to the ranges above and note the trade-off (e.g., Monza low wing vs. Monaco high wing).
