# banner.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected misread variables, missing string suffixes, comparison/arithmetic operators, and GOSUB targets.

## Porting

- Replaced DEC CHANGE/LINE INPUT operations with INPUT, MID$(), ASC(), CHR$(), and string-building loops.
- Converted the message to uppercase with EhBASIC's UCASE$(), matching the
  original uppercase-only input environment while accepting lowercase text.
- Reworked character-pattern output while using EhBASIC's native TAB() positioning.
- Replaced backslash statement separators with EhBASIC colons.
- Split long source lines to fit EhBASIC's 71-character input buffer.
