# life2.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected FOR/NEXT keywords and statement separators that had been misread in the listing.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Replaced prematurely exited state-lookup, board-border, and player-turn FOR
  loops with equivalent counters so RETURN reaches the correct GOSUB frame.
- Added trailing spaces to numeric board labels so their three-column fields
  align with the three-character cells under EhBASIC, and separated the player
  number from the following coordinate prompt.
- Restored player-counter initialization after each generation so the neighbor
  weight held in B cannot appear as a player number.
- Adjusted dialect-dependent syntax, control flow, initialization, or terminal output for EhBASIC while preserving the original program logic.
