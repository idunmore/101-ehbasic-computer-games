# civilw.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected numerous parentheses, variable names, and transposed multiplication/addition operators in the calculations.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Joined spaced GO TO/GO SUB keywords into EhBASIC's GOTO/GOSUB forms.
- Split long source lines to fit EhBASIC's 71-character input buffer.
