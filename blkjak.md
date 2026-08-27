# blkjak.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Line 115 has a period after the line number, which is syntactically invalid; the period just needs to be removed.
- Numerous instances of variables assignments of I or increments by I had been transcribed as 1 and had to be corrected.
- Several line numbers were misinterpreted; including various that were GOTO targets.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Replaced backslash statement separators with EhBASIC colons.
