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

Витрина с абонентами LTE

**Version:** 1.0

## Description

Тот же набор объектов, что в витрине всех видов. Базовая станция BS-1 — сота LTE диапазона 1: EARFCN 100 (2120 МГц вниз), полоса 20 МГц, мощность 46 дБм. Рядом два абонента user_equipment. Спутниковые терминалы UT-1 и UT-2 оставлены терминалами спутника.

## Simulation Parameters

- **JD Origin:** 2460311 (UTC: 2024-01-01 12:00:00)
- **Start Time (s):** 0
- **End Time (s):** 3600
- **Traffic Step (s):** 0.01
- **Geometry Step (s):** 60
