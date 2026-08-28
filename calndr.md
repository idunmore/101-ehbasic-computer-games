# calndr.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected line 180's loop variable from I to N.
- Restored a missing closing quote in the weekday heading.
- Restored the missing trailing semicolon on line 450's TAB statement.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Set an 80-column WIDTH so EhBASIC tracks the absolute TAB() positions used
  by the calendar instead of wrapping its internal cursor counter at the
  default tab interval.
- Retained the original TAB()-based layout using EhBASIC's native positioning support.
- Replaced backslash statement separators with EhBASIC colons.
- Converted DEC array/suffix syntax to EhBASIC-compatible numeric variables and parenthesized subscripts.
