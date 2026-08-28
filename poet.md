# poet.bas

This program required adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

**None.**

## Porting

- Retained the original compact IF/THEN/ELSE structure using EhBASIC's native ELSE support.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Replaced backslash statement separators with EhBASIC colons.
