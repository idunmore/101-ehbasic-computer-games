# rusrou.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Restored the missing decimal point in line 40's probability threshold, changing 83333 to 0.83333.

## Porting

- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Replaced backslash statement separators with EhBASIC colons.
