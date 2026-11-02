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

Kitchen-sink: все типы объектов и переменных netsim

**Version:** 1.0

## Description

Эталонная сцена со всеми типами объектов модели: спутники (Kepler/TLE/OptParam), Walker-группы, HAPS, наземные узлы всех видов, проводные линии/потоки, абонентские регионы (traffic+uplink), пуассон/MM1/QoS, точки наведения, лучи (fixed/steerable, все категории и типы антенн), зоны покрытия, payload (OBP+bent-pipe), транспондерные группы. Все 8 типов антенн. [Загружаемая версия: низкоуровневый payload-блок 'transponders' вынесен в справочник — в текущем загрузчике он содержит баг порчи памяти; см. документ.]

## Simulation Parameters

- **JD Origin:** 2460311.0 (UTC: 2024-01-01 12:00:00)
- **Start Time (s):** 0
- **End Time (s):** 6
- **Traffic Step (s):** 0.01
- **Geometry Step (s):** 60
