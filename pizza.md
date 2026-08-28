# pizza.bas

This program required adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

**None.**

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Converted DEC array/suffix syntax to EhBASIC-compatible numeric variables and parenthesized subscripts.
- Split long source lines to fit EhBASIC's 71-character input buffer.
