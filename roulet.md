# roulet.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Line 1030 contained an unterminated PRINT " statement.
- The welcome message, good-luck message, and blank lines were shifted from their original line numbers.
- The result for “RED, EVEN, COLUMN 1” was numbered 2980 instead of 3290, leaving branches to 3290 unresolved.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Joined spaced GO TO/GO SUB keywords into EhBASIC's GOTO/GOSUB forms.
- Split long source lines to fit EhBASIC's 71-character input buffer.
