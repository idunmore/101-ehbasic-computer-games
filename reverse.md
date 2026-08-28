# reverse.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected the reversal loop variable from I to K and its temporary value variable from S to Z.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Replaced retry-based random list generation with an in-place shuffle that always completes even when EhBASIC initially repeats random values.
- Replaced the prematurely exited win-check FOR loop with equivalent counter control so repeated unsolved moves do not exhaust the stack.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Replaced backslash statement separators with EhBASIC colons.
