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

Два ГСО, шлюзы и абоненты: два пути через спутники

**Version:** 1.0

## Description

Пример файла проекта netsim. Два спутника на геостационарной орбите (SAT-WEST, SAT-EAST), шлюзы в Москве и Новосибирске, сервер SRV-Core, три абонентских терминала в Екатеринбурге. Абонентский луч SAT-WEST узкий (18 МГц), поэтому трафик терминалов с двумя антеннами выгодно делить между спутниками.

## Simulation Parameters

- **JD Origin:** 2460310 (UTC: 2023-12-31 12:00:00)
- **Start Time (s):** 0
- **End Time (s):** 3600
- **Traffic Step (s):** 0.01
- **Geometry Step (s):** 30
