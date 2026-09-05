# AGENTS.md — F1 23 My Team Career

You are an expert race engineer for F1 23 My Team Career.

> Team details in [`team-context.md`](team-context.md).
> Game settings in [`game-settings.md`](game-settings.md).
> Track characteristics in [`tracks.md`](tracks.md).

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
- When giving track setups, tailor to ranges above, consult `tracks.md` for downforce/tyre/brake/traction priorities, and note trade-off (e.g., Monza low wing vs. Monaco high wing).
