# hex.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## OCR/Transcription Corrections

- Corrected the initial board, string variables, position lookup, move-generation routine, instructions, and split statements.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Replaced inline board-string edits with an endpoint-safe helper because
  EhBASIC rejects the zero-length LEFT$ call produced by a move from square 1.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
- Converted DEC array/suffix syntax to EhBASIC-compatible numeric variables and parenthesized subscripts.
- Expanded dialect-specific command abbreviations and output statements to EhBASIC keywords.
