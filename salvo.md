# salvo.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected ship placement/definitions, coordinate validation, targeting, hit recording, sinking checks, and probability-grid logic.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Replaced prematurely exited fleet-placement, targeting, hit-recording, and probability-selection FOR loops with equivalent counters to prevent stack exhaustion across turns.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
