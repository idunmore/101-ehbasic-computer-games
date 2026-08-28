# hi-q.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected the board declaration from the misread DIM B(7,8) to DIM B(70).

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Replaced prematurely exited board-update and game-over FOR loops with equivalent counters so their RETURN statements reach the correct GOSUB frame.
- Returned failed jump-over-a-peg validation to the main input routine normally instead of branching out of a subroutine and leaving its stack frame behind.
- Retained the original TAB()-based layout using EhBASIC's native positioning support.
- Replaced backslash statement separators with EhBASIC colons.
