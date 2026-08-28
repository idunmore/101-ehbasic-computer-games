# target.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- R1 is assigned an illegal value, so corrected that from 57,296 to 57.296
- Fixed the GOTO 8220 so it targets the correct line 820.
- Fixed the range-rounding expressions (restored the multiplication).

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Used EhBASIC's native TWOPI constant and corrected ordinary PRINT/input syntax and control flow.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Replaced backslash statement separators with EhBASIC colons.
