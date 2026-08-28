# rocket.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Restored assignment separators, multiplication operators, and the corrupted velocity, thrust, altitude, and crater-depth equations.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Replaced backslash statement separators with EhBASIC colons.
- Split long source lines to fit EhBASIC's 71-character input buffer.
