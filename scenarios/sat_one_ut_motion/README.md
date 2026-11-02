# scenario

Physical scenario definition: node positions, beam configuration,
and communication standard selection.

## Key Subdirectories
- `antennapatterns`: antenna gain pattern files.
- `beams`: beam/channel/gateway assignment.
- `positions`: GW/UT/satellite positions and HAP traces.
- `standard`: selected communication standard (`DVB` or `LORA`).
- `waveforms`: allowed waveforms and default waveform.
- `topology`: dynamic network topology (`.dnt`) files.
- `beamhopping` (optional): static beam hopping plan.

## User Notes
- ...

# Simulation name

One LEO satellite, beam pointing schedule

**Version:** 1.0

## Description

sat_one_ut with a short synthesis schedule: user beams move between the terminal and a point to the east so the antenna report can show dwell.

## Simulation Parameters

- **JD Origin:** 2460311.0 (UTC: 2024-01-01 12:00:00)
- **Start Time (s):** 0
- **End Time (s):** 60
- **Traffic Step (s):** 0.01
- **Geometry Step (s):** 60
