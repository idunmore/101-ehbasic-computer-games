# fipfop.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Restored missing and merged lines and corrected numerous misread variables, operators, and branch targets.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Replaced the prematurely exited completion-check FOR loop with equivalent
  counter control so repeated turns do not exhaust EhBASIC's control stack.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Joined spaced GO TO/GO SUB keywords into EhBASIC's GOTO/GOSUB forms.
- Replaced the unsupported COT() call with the equivalent reciprocal of TAN().
