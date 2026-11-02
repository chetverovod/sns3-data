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

One LEO satellite + one user terminal

**Version:** 1.0

## Description

Simplified scene from all_objects_showcase.json: SAT-1 (Kepler, i=70°) nadir over UT-1 and GW-1 near Khabarovsk at t=0. GW-1 sits ~6 km from UT-1 so both fit the ~13 km 3 dB spot. GW-1 is the SNS-3 feeder gateway, not a second terminal.

## Simulation Parameters

- **JD Origin:** 2460311.0 (UTC: 2024-01-01 12:00:00)
- **Start Time (s):** 0
- **End Time (s):** 600
- **Traffic Step (s):** 0.01
- **Geometry Step (s):** 60
