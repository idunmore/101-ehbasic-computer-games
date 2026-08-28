# mugwump.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected the position comparisons so lower coordinate guesses and 0,0 do not falsely find Mugwumps.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Replaced the prematurely exited completion-check FOR loop with equivalent
  counter control so turns and automatic replays do not exhaust the stack.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
