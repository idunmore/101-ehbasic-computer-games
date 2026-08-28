# stock.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected misread numeric variable names, comparisons, parentheses, and arithmetic operators throughout the market calculations.
- Restored the cash, NYSE-average, stock-change, and special-trend logic to the corrected reference behavior.
- Corrected the revision date and affected display text/separators.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Retained the original TAB()-based layout using EhBASIC's native positioning support.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Joined spaced GO TO/GO SUB keywords into EhBASIC's GOTO/GOSUB forms.
