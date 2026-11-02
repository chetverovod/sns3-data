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

One LEO satellite (32 beams) + one user terminal

**Version:** 1.0

## Description

Same geometry as sat_one_ut.json (SAT-1 nadir over UT-1/GW-1 near Khabarovsk at t=0). SAT-1 has 32 SNS-3 beams in 8 spots stepped along the ground track: as one spot leaves UT-1, the next (looking back along-track) takes over. Each spot has user UL/DL (HPBW 2 deg) and feeder UL/DL (HPBW 3 deg). GW-1 is the SNS-3 feeder gateway.

## Simulation Parameters

- **JD Origin:** 2460311.0 (UTC: 2024-01-01 12:00:00)
- **Start Time (s):** 0
- **End Time (s):** 600
- **Traffic Step (s):** 0.01
- **Geometry Step (s):** 60
