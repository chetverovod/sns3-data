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

Три группы и межспутниковые линии над Красноярским краем

**Version:** 1.0

## Description

Пример файла проекта netsim. Геостационарный «Экспресс-103», двенадцать аппаратов «Гонец-М» на элементах TLE, пять высотных платформ над Богучанским округом; межспутниковые и межплатформенные радиолинии, шлюз в Красноярске, абонентский терминал в Богучанах, район «Красноярский край», сетки каналов УКВ-диапазонов.

## Simulation Parameters

- **JD Origin:** 2461270.42005 (UTC: 2026-08-17 22:04:52)
- **Start Time (s):** 0
- **End Time (s):** 86400
- **Traffic Step (s):** 0.01
- **Geometry Step (s):** 30
