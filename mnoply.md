# mnoply.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Line 7 incorrectly declared the fourth property-file array as H%(40). It needed to be the rent array R(40); H% was already the local house-count array.
- Line 100 had ";S TURN" instead of the possessive "'S TURN".
- Line 200 used NS(2) instead of N$(2).

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Embedded the companion property and message data and removed DEC mapped-file operations.
- Reworked DEC suffixes, abbreviated I/O, dice selection, and loop exits for EhBASIC's runtime behavior.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
