# furs.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- An incorrectly converted line number (line 508 was read as 506, which caused and error when line 508 was a GOTO target).
- Lines 1176 and 1177 converted the final /10^2 divisors as /0^2 causing an instant divide-by-zero error.
- Corrected the two HOCHELAGA output line numbers from 180/181 to 1180/1181.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Joined spaced GO TO/GO SUB keywords into EhBASIC's GOTO/GOSUB forms.
