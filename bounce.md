# bounce.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Line 135 in the original listing was interpreted as 125, which caused the input prompt for time interval to be printed out of order and for the restart GOTO to error (missing line number).

## Porting

- Retained the original TAB()-based plotting, which EhBASIC supports, and joined the spaced GOTO keyword.
- Joined spaced GO TO/GO SUB keywords into EhBASIC's GOTO/GOSUB forms.
