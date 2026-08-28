# kinema.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- The closing parenthesis on line 110 was missing, rendering the line a syntax error.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Expanded dialect-specific command abbreviations and output statements to EhBASIC keywords.
