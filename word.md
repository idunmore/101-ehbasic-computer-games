# word.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Changed line 231 from the OCR/transcribed 230 P(J)=L(J) to 230 P(Q)=L(J).
- Changed the incorrectly transcribed 232 Q=0+1 to the correct 232 Q=Q+1.

## Porting

- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Replaced the unsupported DEC CHANGE operation with string/array conversion code.
- Split long source lines to fit EhBASIC's 71-character input buffer.
