# animal.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Line 100 was missing the closing quotation mark after RSTS.
- Line 2200 stored a newly learned animal as Z9$. It should have included the animal marker: "\A"+Z9$. Without it, learned animals would be truncated when displayed and omitted from LIST.
- Line 12400 was almost certainly an extra-digit transcription of line 2400. The destination itself worked, but the numbering was inconsistent with the surrounding listing.

## Porting

- Replaced DEC file persistence with an in-memory decision tree populated from DATA; learned animals last for the current run.
- Used EhBASIC's native ELSE support while translating the remaining DEC string and input constructs.
- Converted DEC array/suffix syntax to EhBASIC-compatible numeric variables and parenthesized subscripts.
- Expanded dialect-specific command abbreviations and output statements to EhBASIC keywords.
