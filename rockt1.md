# rockt1.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected the calculation H=H-5(V+V1) to H=H-.5(V+V1) (the error causes 10x the decent rate at the start).
- Fixed a typo from the original listing that was correctly transcribed (so still an error); "BUT YOU SECOND-BY-SECOND" to "BUT YOUR ...".

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Retained the original TAB()-based layout using EhBASIC's native positioning support.
- Replaced backslash statement separators with EhBASIC colons.
