# golf.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Changes here were mostly minor OCR issues such as variable name, type or value transpositions, with a couple of GOTO target line numbers getting altered.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Replaced backslash statement separators with EhBASIC colons.
- Split long source lines to fit EhBASIC's 71-character input buffer.
