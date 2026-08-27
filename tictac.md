# tictac.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- The DATA statement on line 2150 was missing a value (a 0 in the series of 0s), which caused an "out of data" error.
- Corrected the duplicated opening line number from 130 to 120.

## Porting

- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Seeded EhBASIC's random-number sequence from keypress timing before play.
- Replaced searches that exited active FOR loops with equivalent counter loops;
  EhBASIC otherwise left loop frames above the GOSUB frame and reported
  `RETURN without GOSUB` at line 1360.
- Joined spaced GO TO/GO SUB keywords into EhBASIC's GOTO/GOSUB forms.
- Split long source lines to fit EhBASIC's 71-character input buffer.
