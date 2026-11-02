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

DAMA regression: one UT, CBR aligned with sat-dama-verification-sim

**Version:** 1.0

## Description

Эталон регрессии к sat-dama-verification-sim. Совпадает: один user_terminal, без ВСП и без LTE, t_end_s=50, packet_size=1280, interval_ms=5 (CBR 1280 байт каждые 5 мс; предложенная нагрузка 2.048 Мбит/с на направление). Не задаётся в JSON и поэтому не совпадает: сцена geo-33E, луч 18, RBDC DAMA, ACM, выключенные замирания, состав суперкадра. Орбита и четыре луча те же, что у sat_one_ut (LEO над Хабаровском). hapsimulator шлёт этот CBR в обе стороны с t=1 с и не пишет задержку приложения и составной SINR. Для sat-ra-sim-tn9-comparison другие CBR: 1 байт каждые 100 мс, 60 с.

## Simulation Parameters

- **JD Origin:** 2460311.0 (UTC: 2024-01-01 12:00:00)
- **Start Time (s):** 0
- **End Time (s):** 50
- **Traffic Step (s):** 0.01
- **Geometry Step (s):** 10
