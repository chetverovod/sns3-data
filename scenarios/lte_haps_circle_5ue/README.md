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

LTE-only HAPS circle 30 km, 5 UE (one triangular route)

**Version:** 1.0

## Description

LTE-only сцена без SAT/GW: eNB — payload на HAPS, который летит на 30 км по кругу диаметром 20 км (радиус 10 км, 24 точки + замыкание, mode=loop). Пять LTE UE в зоне ячейки: UE-1…UE-4 статичны у центра круга, UE-5 движется по равностороннему треугольнику со стороной 5 км. Бэкхол EPC в ns-3 — локально (вне этого репозитория). t_end_s=1800 ≈ один оборот HAPS при 35 м/с (длина окружности ≈ 62.8 км).

## Simulation Parameters

- **JD Origin:** 2460311.0 (UTC: 2024-01-01 12:00:00)
- **Start Time (s):** 0
- **End Time (s):** 1800
- **Traffic Step (s):** 0.01
- **Geometry Step (s):** 1
