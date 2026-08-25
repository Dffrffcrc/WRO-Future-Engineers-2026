# SSTtechnitum

SSTtechnitum is the team behind this repository, which holds the engineering materials for our self-driven vehicle built for the WRO Future Engineers 2025 season.

## Components Used

| # | Part | Model | Qty |
|---|------|-------|-----|
| 1 | Microcontroller | EvolutionX1, ESP32-S3 | x1 |
| 2 | Motors | EV3 Medium Motors | x2 |
| 3 | Camera | MaixCam | x1 |
| 4 | Distance Sensor | Time of Flight, VL53L0X | x3 |
| 5 | Compass | IMU, BNO055 | x1 |
| 6 | I2C Multiplexer | TCA9548A | x1 |
| 7 | IO Multiplexer | SX1506 | x1 |
| 8 | Battery | NCR18650B | x2 |

## Repository Structure

* **`Documents`** — the team's Engineering Journal.
* **`Schemes`** — schematic diagrams (JPEG/PNG/PDF) showing how the vehicle's electronic components and motors are wired together.
   * `Microcontroller Wiring Diagram.png` — diagram of the microcontroller system.
   * `Overall System Wiring Diagram.png` — diagram of the full vehicle wiring.
* **`Models`** — 3D printing, laser-cutting, and CNC files for the vehicle's physical parts. *(Remove this folder if it's ever left empty.)*
   * `EVO Brick Model.stl` — case that houses the EvolutionX1 Brick.
   * `VL53L0X Lego Mount Model.stl` — mount for the Time of Flight sensor.
* **`Photos`** — two subfolders with team and vehicle photos.
   * `Team` — one official group photo of the full team.
   * `Vehicle` — six photos covering every side of the bot.
      - `Front View.jpeg`
      - `Back View.jpeg`
      - `Left View.jpeg`
      - `Right View.jpeg`
      - `Top View.jpeg`
      - `Bottom View.jpeg`
* **`Software`** — all code written for the competition.
   * `Code` — the two competition programs.
     - `WRO_FE_Open.ino` — used for the preliminary (open) round.
     - `WRO_FE_Colour.ino` — used for the challenge (colour) round.
   * `Library` — every dependency the code needs.
     - `Library/Evo.zip` — our core microcontroller library, bundled with its own external dependencies.
     - `Library/External_libraries` — additional .zip libraries that must be added to the Arduino IDE for the code to run.

## Setup

1. Open the Arduino IDE and go to **Sketch → Include Library → Add .ZIP Library**, then install every library found in `Software/Library/External_libraries`. **All of them are required — the code will not run without the full set.**
2. Using the same Add .ZIP Library process, install `Software/Library/Evo.zip`.
3. Open whichever program fits your round — `WRO_FE_Open.ino` or `WRO_FE_Colour.ino` — in the Arduino IDE.

## Pre-Run Checklist

**Software**
- Board is set to ESP32-S3.
- All sensors are calibrated for the competition venue.
- MaixCam is powered, connected, and detected properly.

**Hardware**
- Every wire is seated in the correct spot.
- No faulty components — swap out anything suspect.
- Structural parts are intact and firmly assembled.
- Wheels are secure, not loose.
- Steering moves freely with no faults.

**Placement**
- Bot is positioned straight on the start line.

---
