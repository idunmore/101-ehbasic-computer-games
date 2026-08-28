# digits.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected variables, weighted-term operators, array indices, loop syntax, and the losing-score branch in the prediction algorithm.

## Porting

- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Replaced backslash statement separators with EhBASIC colons.
- Replaced unsupported MAT operations with explicit array loops.
