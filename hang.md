# hang.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Changes here were mostly minor OCR issues, transposing 1 for I and vice-versa, and one or two misses on line numbers for GOTO targets.

## Porting

- Added explicit spaces before implicitly adjacent numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Replaced RANDOMIZE with a GET-based timing seed so fresh runs do not always open with the same word.
- Replaced prematurely exited FOR/NEXT searches with counter loops, preventing loop-frame accumulation and the line-230 out-of-memory failure.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
