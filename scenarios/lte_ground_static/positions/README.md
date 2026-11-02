# scenario/positions

Position description files for scenario nodes.

## Base Files
- `gw_positions.txt`
- `ut_positions.txt`
- `sat_positions.txt` or `tles.txt`
- `isls.txt` and `start_date.txt` (for constellations)
- `sat_traces.txt` (for HAP traces)

## LTE (optional, `scenario/cellular/`)
- `enb_positions.txt` / `ue_positions.txt`: `Latitude Longitude Height`
- `enb_traces.txt` / `ue_traces.txt`: `id relativePath` (path from `scenario/`)
- Airborne eNB reuses the carrier HAP trace; do not invent a second trajectory.
- `enb.conf`, `ue.conf`: radio / serving-cell mapping for LENA

## Coordinate Formats
- Static nodes (`*_positions.txt`): `Latitude Longitude Height` (3 columns, no time).
- Dynamic tracks / Traces: `Time Latitude Longitude Height` (4 columns).

## NS-3 Time Rules (for 4-column trace files)
- Files must NOT contain headers (text lines).
- Single-line trace files: Time must NOT be 0.0 (e.g., use 0.001).
- Multi-line trace files: Time must be strictly increasing. First line can be 0.0.

## Additional Formats
- In `sat_traces.txt`: `satId traceFile`

## User Notes
- ...
