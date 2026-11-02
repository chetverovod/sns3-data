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

Витрина: все виды объектов netsim

**Version:** 1.0

## Description

Пример файла проекта netsim: по одному-два объекта каждого вида — группа Уокера, спутники по элементам орбиты и по TLE, высотные платформы, наземные узлы всех типов, проводная сеть, районы, лучи, зоны покрытия, полезная нагрузка, очереди имитации, группы транспондеров.

## Simulation Parameters

- **JD Origin:** 2460311 (UTC: 2024-01-01 12:00:00)
- **Start Time (s):** 0
- **End Time (s):** 3600
- **Traffic Step (s):** 0.01
- **Geometry Step (s):** 60
