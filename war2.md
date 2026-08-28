# war2.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- These were limited to replacing the , at the ends of the PRINT statements on lines 9 and 11, so that the INPUT requests all occurred on the same line as the prompt.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Expanded dialect-specific command abbreviations and output statements to EhBASIC keywords.
