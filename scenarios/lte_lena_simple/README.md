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

LTE regression: one co-located eNB and UE

**Version:** 1.0

## Description

Эталон регрессии к lena-simple-epc (одна пара, 1.1 с). Совпадает: eNB и UE в одной точке (55.0 N, 37.0 E, высота 0), earfcn 100, полоса 5 МГц (25 RB), tx_power_dbm 30, t_end_s=1.1. Штатный пример ставит оба узла в одну декартову точку и гоняет UDP вниз и вверх (1024 байта, 100 мс, старт 0.5 с). Здесь радиоинтерфейс LENA без фидера: UDP в sibgu-hap создаётся только вверх (512 байт, 100 мс, старт 1 с) и только если в сцене есть спутниковый шлюз, поэтому PDCP в этом прогоне пустой. Сравнивать имеет смысл RSRP и SINR. HAPS-1 — заглушка SNS-3 с неподвижной трассой (иначе симулятор берёт устаревший TLE); eNB на неё не посажен.

## Simulation Parameters

- **JD Origin:** 2460311.0 (UTC: 2024-01-01 12:00:00)
- **Start Time (s):** 0
- **End Time (s):** 1.1
- **Traffic Step (s):** 0.01
- **Geometry Step (s):** 1
