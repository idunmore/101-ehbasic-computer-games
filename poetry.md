# poetry.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected line 1420's target from 1456 to 1450.
- Restored the omitted line 1610 and repaired the subsequent selection-dispatch numbering and targets.
- Removed duplicated dispatch lines and corrected the B5 branch target.

## Porting

- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Joined spaced GO TO/GO SUB keywords into EhBASIC's GOTO/GOSUB forms.
