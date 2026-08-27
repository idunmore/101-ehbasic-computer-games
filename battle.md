# battle.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected misread comparison operators and assignments throughout the fleet-placement logic.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Replaced MAT operations with explicit loops and translated square-bracket subscripts and GOTO ... OF syntax.
- Used EhBASIC's native MIN() and MAX() functions for the original fleet-placement calculations.
- Converted DEC array/suffix syntax to EhBASIC-compatible numeric variables and parenthesized subscripts.
- Split long source lines to fit EhBASIC's 71-character input buffer.
