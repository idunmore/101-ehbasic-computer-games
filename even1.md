# even1.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Some line numbers and calculations and comparisons were incorrectly OCRd/transcribed from the printed listing.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
