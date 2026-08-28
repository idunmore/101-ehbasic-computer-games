# poker.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected “CARDS SO YOU WANT” to “CARDS DO YOU WANT.”
- Corrected LET$S=H$ to LET J$=H$.
- Removed the stray semicolon from GOSUB 195;.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
