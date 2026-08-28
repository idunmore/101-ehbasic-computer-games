# wekday.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected line 140's misread Y1 input variable, restoring INPUT M1,D1,Y1.
- Removed the stray @ character from the Friday-the-thirteenth warning.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
