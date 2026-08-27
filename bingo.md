# bingo.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Restored the missing closing quote on the card separator line.
- Restored the first diagonal's RETURN and second-diagonal entry line numbers,
  and corrected the second diagonal's starting row from X to F.

## Porting

- Replaced MAT READ with an explicit READ loop and moved initialization so replay does not redimension arrays.
- Replaced vertical and horizontal win-check FOR loops with equivalent counter
  loops so every RETURN reaches its GOSUB frame under EhBASIC.
- Enquoted DATA string values, so "O" doesn't lose its trailing space
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Joined spaced GO TO/GO SUB keywords into EhBASIC's GOTO/GOSUB forms.
