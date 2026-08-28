# spcwar.bas

This program required corrections to **both** the OCR/transcriptions, and adjustments to the code (syntax, logic, features) as part of porting it.

## spcwar.bas vs. spcwar-16k.bas

I've made two ports of the original `spcwar.bas` here.  The gameplay is the same, but the "full" original version requires more memory than most BE6502 builds will have (24KB vs. the stock 16KB):

- **spcwar.bas** - This is the full port, and requires 24KB of RAM to run.

- **spcwar-16k.bas** -  This version will run on a 16KB machine; the instructions were moved out of the main game and into a separate markdown file (`spcwar-16k-instructions.md`)

## OCR/Transcription Corrections

- Restored the damage array, course indices and bounds, coordinate rounding, status messages, counters, and calculator flag.

## Porting

- Added explicit spaces before string literals following numeric PRINT items to preserve the source dialects' output under EhBASIC.
- Converted the full Star Trek listing to in-memory EhBASIC syntax; this full edition still requires an expanded-memory system rather than a standard 16 KB build.
- Removed unsupported RANDOM/RANDOMIZE seed statements.
- Standardized random draws on EhBASIC's sequence-advancing RND(0) form.
