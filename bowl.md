# bowl.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Fixed transcription issues that resulted in syntax errors for PRINT and array references.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Replaced MAT array initialization with explicit loops while retaining EhBASIC's native TAB() and boolean NOT support.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Replaced backslash statement separators with EhBASIC colons.
- Split long source lines to fit EhBASIC's 71-character input buffer.
