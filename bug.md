# bug.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Some common errors, including transposition of B for 8, which occurred once in the body output.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Retained the original TAB()-based layout using EhBASIC's native positioning support.
- Converted DEC array/suffix syntax to EhBASIC-compatible numeric variables and parenthesized subscripts.
- Split long source lines to fit EhBASIC's 71-character input buffer.
