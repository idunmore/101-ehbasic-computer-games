# bagels.bas

This program required adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

**None.**

## Porting

- Added explicit spaces before implicitly adjacent numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Guarded the PICO and FERMI output loops when their counts are zero, because
  EhBASIC executes a FOR loop body once even when its initial value exceeds
  its limit.
- Replaced the secret-number generation loops with equivalent counter loops
  so retrying a duplicate digit does not leave an active FOR frame behind.
- Replaced the unsupported DEC CHANGE operation with string/array conversion code.
