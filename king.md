# king.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Line 34: MAGNIFICIENT to MAGNIFICENT.
- Line 50: initial treasury 64000 to 60000, and restored the missing closing parenthesis.
- Line 310: corrupted A(HW) expression restored as A+HW.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Split long source lines to fit EhBASIC's 71-character input buffer.
