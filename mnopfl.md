# mnopfl.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- The property-name array was incorrectly transcribed as Q$(40) instead of the original G$(I). This wouldn't matter much, but we want to use it later for the game, so this was corrected to be a value the game program, mnoply.bas expects.
- MATLIDA'S MONOPOLY was corrected to MATILDA'S MONOPOLY.
- And the original title record, on line 200, was truncated slightly so as not to exceed line-length limits if moved to a 4-character line number when incorporated into the second part of this port.

## Porting

- Replaced mapped-file output with ordinary arrays and DATA so the property/card tables are built in memory.
- Converted DEC array/suffix syntax to EhBASIC-compatible numeric variables and parenthesized subscripts.
