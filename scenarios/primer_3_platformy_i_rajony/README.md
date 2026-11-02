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

ГСО и высотные платформы: районы абонентов

**Version:** 1.0

## Description

Пример файла проекта netsim. Геостационарный спутник и пять высотных платформ над Богучанским округом, шлюз и абонентский терминал, район «Красноярский край» и второй район, нарисованный в окне программы, три зоны покрытия.

## Simulation Parameters

- **JD Origin:** 2461270.42005 (UTC: 2026-08-17 22:04:52)
- **Start Time (s):** 0
- **End Time (s):** 86400
- **Traffic Step (s):** 0.01
- **Geometry Step (s):** 30
