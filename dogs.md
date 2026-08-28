# dogs.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Several variable names for FOR/NEXT loops, calculations and some logic that resulted in unreachable code (win/loss updates), had to be corrected.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Retained the original TAB()-based layout using EhBASIC's native positioning support.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Replaced backslash statement separators with EhBASIC colons.
