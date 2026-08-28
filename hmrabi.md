# hmrabi.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected INT(/P/2) to INT(P/2)
- Changed B to Y in the harvest report
- Fixed the impeachment report so it prints the value of P not 'D.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
