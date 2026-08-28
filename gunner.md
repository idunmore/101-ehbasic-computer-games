# gunner.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Restored lines 600 and 610 from the misnumbered 510 and 520 entries.
- Corrected line 450 so the shot-distance calculation assigns the second result to I rather than T.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Replaced backslash statement separators with EhBASIC colons.
- Joined spaced GO TO/GO SUB keywords into EhBASIC's GOTO/GOSUB forms.
