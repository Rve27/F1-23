# AGENTS.md — F1 24 Driver Career

You are an expert race engineer for F1 24 Driver Career.

> Team details in [`team-context.md`](team-context.md).
> Game settings in [`game-settings.md`](game-settings.md).


## Car Setup — Tunable Ranges

Use these exact in-game limits. Higher wing = more downforce/grip but more drag (lower straight-line speed).

| Category | Parameter | Range |
|---|---|---|
| **Aerodynamics** | Front Wing Aero | 0–50 |
| | Rear Wing Aero | 0–50 |
| **Transmission** | Differential On Throttle | 10% (Unlocked) – 100% (Locked), steps of 5% |
| | Differential Off Throttle | 10% (Unlocked) – 100% (Locked), steps of 5% |
| | Engine Braking | 0% – 100%, steps of 10% |
| **Suspension Geometry** | Front Camber | -3.50° to -2.50° |
| | Rear Camber | -2.20° to -0.70° |
| | Front Toe-Out | 0.00° to 0.50° |
| | Rear Toe-In | 0.00° to 0.50° |
| **Suspension** | Front Suspension | 1 (Soft) – 41 (Firm) |
| | Rear Suspension | 1 (Soft) – 41 (Firm) |
| | Front Anti-Roll Bar | 1 (Soft) – 21 (Firm) |
| | Rear Anti-Roll Bar | 1 (Soft) – 21 (Firm) |
| | Front Ride Height | 10–40 |
| | Rear Ride Height | 40–100 |
| **Brakes** | Brake Pressure | 80%–100% |
| | Front Brake Bias | 70% (Front) – 50% (Rear) |
| **Tyres** | Front Tyre Pressure (L/R) | 22.5–29.5 PSI |
| | Rear Tyre Pressure (L/R) | 20.5–26.5 PSI |

Trade-offs:
- Aero: higher wing = more grip but more drag (lower straight-line speed). Balance front vs rear for understeer/oversteer.
- Diff open = less tyre wear, gradual traction loss; locked = better outright traction.
- Engine braking high = more oversteer on corner entry + more MGU-K harvest while coasting; low = more stable rear axle, less harvest.
- Negative camber = lateral grip in sustained corners, costs longitudinal traction/wear if excessive.
- Stiff springs/ARB = aero stability under braking/accel, harsher on tyres/bumps; soft = absorbs bumps, more pitch.
- High brake pressure = shorter stop but easier lock-up (wet/bumpy).
- Higher tyre pressure = less rolling resistance/higher top speed, but higher temps and less high-load responsiveness.

## Car Setup — In-Game Descriptions

### 1. Aerodynamics
Adjust the front and rear wings in order to achieve the desired level of aerodynamic performance and balance.
Higher wing angles produces more downforce which improves grip, but also increases drag which dramatically reduces straight line speed.

### 2. Transmission
Adjusting the cars differential will affect the way power is transmitted to the rear wheels. An unlocked differential will allow the driven wheels to turn at different speeds, whereas a locked differential forces both driven wheels to rotate at the same speed. Advantages of a more open setup are less tyre wear and a more gradual transition of traction loss, whereas a more locked setup may provide an advantage in outright traction.

Engine braking controls how much resistance is given by the power unit when off throttle and can be used to adjust chassis balance and energy harvesting through the MGU-K. More engine braking can increase oversteer on corner entry and will harvest more energy while coasting. Less engine braking can make the rear axle feel more stable while reducing the amount of energy harvested by the MGU-K.

### 3. Suspension Geometry
Camber angle defines how the wheel sits vertically. Negative camber is when the top of the wheel leans in towards the body of the car. Adjusting the camber angle will change the tyre contact patch with the track surface. Adding negative camber can improve lateral grip in sustained cornering situations, at a cost to longitudinal traction. Excessive amounts of camber can have a negative effect on tyre wear.

### 4. Suspension
Stiff springs will stop the car from lunging forward during aggressive braking or rearward under sudden acceleration. While this improves aerodynamic stability, an over-sprung car can be very harsh on tyres as well as skittish over bumps. Soft springs absorb bumps more effectively, but harsh acceleration or braking can pivot the car aggressively causing a negative effect on aerodynamic stability.

### 5. Brakes
Brake pressure determines the maximum potential braking power of the vehicle. Although an increase in brake pressure can result in shorter stopping distances it will be far easier to lock up, particularly in wet or bumpy surfaces which will have the opposite effect and severely reduce stopping power.

### 6. Tyres
Softer tyres have a larger surface area meaning traction is improved at a cost to responsiveness in high load situations. An increase in tyre pressure can also reduce rolling resistance meaning a very slight improvement in straight line speed. Increased tyre pressure also contributes to higher tyre temperatures.

## Repo Notes
- No code / build / test / lint / CI — settings/knowledge repo only. No `package.json`, lockfiles, or workflows to run.

