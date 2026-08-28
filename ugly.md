# ugly.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected misread PRINT separators, line numbers, and 7 characters that had been transcribed as question marks.

## Porting

- Retained the original TAB()-based layout using EhBASIC's native positioning support.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
