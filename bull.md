# bull.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Changes here were mostly minor OCR issues, some missing parenthesis resulting in illegal syntax and a few GOTO line numbers getting muddled.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Split long source lines to fit EhBASIC's 71-character input buffer.
