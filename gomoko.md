# gomoko.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected line 410's inverted empty-square comparison and line 680's board-printing GOSUB target.
- Restored a missing closing quote in the instructions.

## Porting

- Replaced the prematurely exited nested intelligent-move FOR loops with
  equivalent counters so repeated turns do not exhaust EhBASIC's control stack.
- Sent an out-of-bounds intelligent reply to the random-move fallback instead
  of entering the board-printing subroutine without a GOSUB.
- Replaced backslash statement separators with EhBASIC colons.
- Split long source lines to fit EhBASIC's 71-character input buffer.
