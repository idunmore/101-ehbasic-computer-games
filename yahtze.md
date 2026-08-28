# yahtze.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Fixes numerous corruptions/transcription errors that lead to a variety of issues, including broken re-roll loops, scoring, bonus handling, summaries and winner selection.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Replaced unsupported MAT and CHANGE operations with explicit loops and string conversion code.
- Retained the original TAB()-based layout using EhBASIC's native positioning support.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
