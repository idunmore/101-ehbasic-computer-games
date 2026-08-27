# basbl1.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected misread comparison operators, variables, and stray scan characters in the densely packed game logic.

## Porting

- Combined the original loader and chained baseball game into one in-memory program because EhBASIC has no CHAIN/file-loading workflow here.
- Expanded dialect-dependent conditional and multi-statement logic into EhBASIC-compatible control flow.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Replaced backslash statement separators with EhBASIC colons.
