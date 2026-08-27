# batnum.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Numerous OCR/transcriptions issues were present, most of which were either misinterpreting >= in the scanned pages as either > or <= or reading a W as an N. The changes can all be seen by diffing the initial, and this, commit.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Joined spaced GO TO/GO SUB keywords into EhBASIC's GOTO/GOSUB forms.
