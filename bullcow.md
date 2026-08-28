# bullcow.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected comparison operators to match the proper bounds, added missing semicolons, and changed line 340's FOR/NEXT loop to have the correct end value (4 instead of P).

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Replaced duplicate-digit and candidate-validation FOR loops with equivalent
  counter loops so retry branches cannot leave loop frames on EhBASIC's
  control stack and corrupt later guesses or RETURN statements.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Split long source lines to fit EhBASIC's 71-character input buffer.
