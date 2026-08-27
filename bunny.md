# bunny.bas

## The Missing Listing

The original book does not seem to have included a listing for this program, which is supposed to print a picture of the "Playboy Bunny".

Since I achieved my goal of porting **ALL** 101 (actually 108, though a couple are two-parters, and I did *two* ports of `spcwar.bas`, which is the text-based "Star Trek" game, in order to have one that would fit for 16KB RAM builds) games, successfully, so that they will just "**load and run**" on a standard Ben Eater 6502 build running either his, or my, builds of MS-BASIC, I thought it might be fun to address *this* omission.

## Making that Right

So, here you go ... `bunny.bas`.

The original picture in the book shows a "Playboy Bunny" constructed purely of the characters in "BUNNY" repeated over and over.  The characters aren't random.

The printout is what you'd get if you printed 49 lines of "BUNNYBUNNYBUNNYBUNNY ... BUNNYBUNNY" all the way across one sheet of paper, and then cut-out a stencil to reveal the image you wanted to show.

### How it Works

So, that's what the code does:

It uses a set of strings, stored as `DATA` statements, which have a 0 in any position that should be covered and a 1 in any position that would be uncovered, by such a stencil.

Each `DATA` statement represents one line in the picture (this is easy to see in the listing).

The code reads a string, while tracking where it is across the page, and using the column value to index into an array of the characters "BUNNY" to determine what character it should be outputting when it encounters a `1` in the string.  The character array index "wraps" or "resets" on the 5th position, so we don't need a 54 character-wide array.

*This results in simple code and a compact data encoding, with the bonus that it makes the actual "drawing" of the picture interesting to watch.*

### Alternate Approaches

I thought, briefly, about doing the binary encoding not as literal strings of `0`s and `1`s, but converting them to integer values.  This would result, on average, in a 50% reduction of the amount of data required, but a) would require adding a routine to convert a decimal value to its binary components, which is more complicated than the, effectively, sub-string/map logic use in my actual code and b) would not be human-readable.

I also would have had to write a script to conver the binary data to decimal ...

## Not Perfect

The final picture output is not a perfect recreation of the original in the book.

I wrote a script to convert the raw picture to columns and rows, and also decided that left-aligning the output was okay, so this results in some minor interpretation issues and differences in which columns were exposed vs. hidden, so some lines won't have the precise character sequences of the original image.
