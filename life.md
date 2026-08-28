# life.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- These were primarily array-subscript and variable name issues, with a couple of cases of using , as a separator.

## Porting

- Replaced DEC keyboard-file LINE INPUT with quoted row-by-row INPUT ending with DONE.
- Used EhBASIC's native ELSE clause and TAB() positioning for the generation display.
- Joined spaced GO TO/GO SUB keywords into EhBASIC's GOTO/GOSUB forms.
- Converted DEC array/suffix syntax to EhBASIC-compatible numeric variables and parenthesized subscripts.
