# canam.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected misread variables, relational operators, and the rain-event GOTO target.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Adapted the original multi-terminal/file-based race to a single terminal with in-memory state.
- Replaced unsupported MAT and CHANGE operations while retaining EhBASIC's native TAB() layout.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
