# scenario/waveforms

Allowed return-link waveforms.

## Required Files
- `waveforms.txt`
- `default_waveform.txt`

## `waveforms.txt` Line Format
`ID ModBits CodingRate PayloadBytes DurationSymbols [PreambleSymbols]`

## Additional Rule
- `default_waveform.txt` must contain one default waveform ID.
- DVB (DVB-RCS2): waveform IDs must be 2-22. ID 1 has no SNS3 link-results table.
- LORA: waveform IDs must be 1-2.

## User Notes
- ...
