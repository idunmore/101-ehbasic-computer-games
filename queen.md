# queen.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Line 25 had a stray ! after the closing quotation mark.
- Line 320 used addition instead of subtraction: 320 IF T1+T<>2P THEN 3200 Corrected to: 320 IF T1-T<>2P THEN 3200
- Line 2110 changed the wrong coordinate: 2110 LET T=T1-K Corrected to: 2110 LET U=U+K

## Porting

- Printed board entries in fixed five-column TAB() fields and set WIDTH 80 so
  two- and three-digit square numbers remain vertically aligned under EhBASIC.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Joined spaced GO TO/GO SUB keywords into EhBASIC's GOTO/GOSUB forms.
- Split long source lines to fit EhBASIC's 71-character input buffer.
