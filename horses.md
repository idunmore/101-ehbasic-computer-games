# horses.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Restored the horse-speed formula, removed a duplicated race header, and repaired the mutuel calculation and digit formatter.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Set an 80-column WIDTH so EhBASIC tracks the payout table's absolute TAB()
  positions instead of wrapping its internal cursor at the default tab interval.
- Retained the original TAB()-based layout using EhBASIC's native positioning support.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Replaced backslash statement separators with EhBASIC colons.
