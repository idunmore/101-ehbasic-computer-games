# nim.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Removed a stray period before X(I,Y) on line 425 and repaired line 455's malformed even-column test.
- Corrected line 540 to test D=1 for the singular/plural message.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Replaced exponentiation-based binary conversion with an integer power-of-two
  table, preventing fractional stick counts and false rejection of whole piles.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Replaced backslash statement separators with EhBASIC colons.
- Joined spaced GO TO/GO SUB keywords into EhBASIC's GOTO/GOSUB forms.
