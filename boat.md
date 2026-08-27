# boat.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- A good number of the variable names and computational expressions are very hard to read in the original listing and were incorrectly OCRd/transcribed.
- Fixing them required not just reading the original listing but some logical deduction as it was not possible to make out, reliably, all of the variable names there.
- Restored a missing closing quote in the introductory text.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Joined spaced GO TO/GO SUB keywords into EhBASIC's GOTO/GOSUB forms.
- Split long source lines to fit EhBASIC's 71-character input buffer.
