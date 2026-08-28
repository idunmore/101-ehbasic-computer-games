# checkr.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected PRINT separators, the first DATA row, and misread comparison and movement logic.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Retained the original TAB()-based layout using EhBASIC's native positioning support.
