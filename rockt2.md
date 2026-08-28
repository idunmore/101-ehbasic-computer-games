# rockt2.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Fixed corrupted constants and variables, including R0, M0, M1=7.45 and B=750.
- Corrected metric/English conversion values and unit-strings.
- Fixed errors in the calculations for distance, fuel and out-of-fuel, and put the missing ^2 in the gravity calculation.

## Porting

- Retained the original TAB()-based layout using EhBASIC's native positioning support.
