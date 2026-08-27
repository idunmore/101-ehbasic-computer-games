# boxing.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Some common errors, including transposition of B for 8 and I for 1, which caused both calculation and FOR/NEXT errors ("next without for" in the main "rounds" loop).
- Some PRINT separation characters were missing/incorrect.
- Line 980 was read as 981, and looking at the listing it is easy to see why, but this was a GOTO target (a knockout), so that results in a runtime error.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Joined spaced GO TO/GO SUB keywords into EhBASIC's GOTO/GOSUB forms.
