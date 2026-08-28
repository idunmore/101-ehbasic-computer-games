# fotbal.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected numerous missing/misnumbered instruction and play-table lines, including the omitted HALF-BACK OPTION and runback calculation.
- Restored malformed array references, comparisons, arithmetic operators, PRINT separators, and GOTO targets that materially affected play.
- Restored truncated field dividers and kickoff/gameplay output text.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Retained the original TAB()-based layout using EhBASIC's native positioning support.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Replaced backslash statement separators with EhBASIC colons.
- Split long source lines to fit EhBASIC's 71-character input buffer.
