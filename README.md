## 101 BASIC Computer Games

[![Static Badge](https://img.shields.io/badge/EhBASIC-v2.22p5.7-orange)](https://github.com/Klaus2m5/6502_EhBASIC_V2.22/tree/master/patched)&nbsp;
[![Static Badge](https://img.shields.io/badge/architecture-Ben_Eater_6502-blue)](https://eater.net/6502)&nbsp;
[![Static Badge](https://img.shields.io/badge/EhBASIC-v2.22p5.7--IMDLABS-purple)](https://github.com/idunmore/ehbasic)

Or perhaps a better title would be:

**"101 BASIC Computer Games for the Ben Eater 6502 running EhBASIC"**

This is a "project" based on David Ahl's, now-classic, book of type-in games for early versions of BASIC, in which I have completed porting ***ALL*** of them in a **ready-to-run** form for the [Ben Eater 6502](https://eater.net/6502) (and similar) computer, running [Lee Davidson's](http://retro.hansotten.nl/6502-sbc/lee-davison-web-site/) EhBASIC.

There are various ports of EhBASIC avaialble.  I recommend either [Klaus Dormann's patched EhBASIC v2.22p5](https://github.com/Klaus2m5/6502_EhBASIC_V2.22/tree/master/patched), or [my own](https://github.com/idunmore/ehbasic) (which is based on Klaus's but with various additions and built _specifically_ to run on a stock Ben Eater 6502 build), without needing to be able to code yourself.

### About the Source Material
The original source of these programs was as printed listings in a book, David Ahl's "[101 BASIC Computer Games](https://archive.org/details/101basiccomputer0000davi)", the first printing for which was in July 1973; over 50 years ago.

You typed them into your computer yourself, then ran them.  If you transcribed things accurately, they worked; if not, issues could arise - some obvious, some very subtle.

And, since dialects of BASIC had, sometimes significant, differences, you may have had to make adjustments to the code for it to work on your particular computer or version of BASIC.  Occasionally it would be too much to work, or there was no practical workaround, so a feature would have to be changed or dropped.

### Copyright & Public Domain
Per [this](https://blog.adafruit.com/2022/06/16/david-ahl-places-all-his-classic-computing-publications-into-the-public-domain/) news post, David Ahl generously placed all of his written material (books, articles, programs, tutorials) into the Public Domain.

Similarly, any changes or fixes I've made, or new code I've written as workarounds, to the files **within *this* repository** also formally reside in the Public Domain.

## From Book to Files

[Maury Markowitz](https://github.com/maurymarkowitz) undertook scanning, OCRing (with LLM-driven AI assistance), the original programs from the book.  You should definitely read their [notes](https://github.com/maurymarkowitz/101-BASIC-Computer-Games/blob/main/NOTES.md) on the process!  It is not 100% perfect, but the reasons why, and what compensations have been applied, are very interesting.  Some programs have errors as a result (beyond any present in the original code itself).

I consider Maury's work as a wonderful act of preservation.

*Without it, my little undertaking here would **not** be possible.*

## What *I've* Done Here

Well, for one thing, this is my second time porting this set of programs.  The first used Microsoft BASIC v1.1 from 1977 as the target.  The vast majority of that (>95%) was done manually (i.e., without AI assistance/automation).

My purpose, there, was more about nostalgia-driven fun than preservation:

Why build a "retro" computer if not to run "retro" software on it?  Not everyone codes, even those that build such machines.  Once up and running it is both fascinating and entertaining to see what software was created and used at the time; even if it is simple games you typed in from a book.

And, of course, sometimes you just *[want to play those games](https://www.youtube.com/watch?v=GfJJk7i0NTk&t=108s)*.

*_What I have done (past tense) here is rather different to my first "pure" porting cycle for Microsoft BASIC._*

- I did not want to simply port from my _existing MS-BASIC ports_; the original dialects of BASIC used in these programs often have features not present in MS-BASIC and needed some interesting workarounds, simplifications and, sometimes, writing whole new routines or different solutions entirely.

  However, EhBASIC has features that MS-BASIC does not; for example, EhBASIC supports `IF/THEN/ELSE` constructs, where MS-BASIC has no `ELSE` clause, so fewer workarounds/replacements would be needed to be a proper, or "full", EhBASIC port.  They would not be very interesting ports, either; the bulk of them would simply be replacing RND(1) calls with RND(0) and vice-versa, since MS-BASIC and EhBASIC have inverted the behavior of those calls.

- As I have already corrected any issues arising from the OCR conversion, which was done via reference to scans of the original book or, where that wasn't legible/clear, my own fixes, I do not wish to repeat that!  So, I am going to use my ported MS-BASIC versions as the sources for _those_ corrections.

The end result should, thus, be a port that utilities EhBASIC in full spirit/function, while be dramatically less work.

### An Exception ... Sort of ...
Only one program, "`spcwar.bas`", which is a rather nice version of Mike Mayfield's original, and classic, "Star Trek" program, fails the "runs on a standard Ben Eater 6502 build" test.  And that is simply because the code alone simply **doesn't fit** into the available memory of a BE6502 build with 16KB of RAM, and that's without the space the executing code needs for arrays and variables, etc.

I did two things with that ...

- First, I did a full-fat port ... and that works nicely if you've built an otherwise-compatible version of Ben's 6502 but have adapted the memory map to allow 24KB of RAM.

- Second, I trimmed down that version so that it would fit, and run, as-is, on the standard 16KB RAM build ("`spcwar-16k.bas`").  The gameplay is identical; it just omits the comprehensive built-in instructions/manual.  Those elements you can find in the companion markdown file, "`spcwar-16k.md`").

## Understanding this Project & Repository

For each game:

- I first committed an identical copy of the file from [Maury's GitHub repository](https://github.com/maurymarkowitz/101-BASIC-Computer-Games/tree/main).
- I ported the code, making any necessary corrections, and commit that.
- I added an `gamename.md` file describing the nature of the changes required to make the program run on the target versions of MS-BASIC.

  Sometimes this was as simple as "runs as is", "fixed OCR/transcription issues", or more involved if code and logic has to be changed due to differences in the versions of BASIC involved.

This approach makes it easy to compare the original code with the changed code, simply by diffing the two commits.

## Which Games Work?

All of them.

Unlike when I did the MS-BASIC ports, where I was not 100% sure everything _could_ be ported until I'd successfully tackled them, that's _not_ the case here.  The outcome is a forgone conclusion; it is only the details that vary.

### Bugs

There **will** be some.

There certainly are in the original listings!

Per above, I have played all of these games, to completion, as both winner and loser.  And that was both enjoyable and fascinating.  But there's no chance that there aren't lurking bugs; be they a result of these porting efforts, or logic issues in the original code that have then been ported faithfully!


### What Was Needed (on a Per-Program Basis):

Various types of work were required in correcting and porting these programs, and the commit messages indicate this as follows:

| Message                  | Meaning                                                                 |
|--------------------------|-------------------------------------------------------------------------|
| Add original source file | The original source code runs **as-is**; `gamename.md` will be  present |
| Ported                   | Code changes were required to run under EhBASIC                         |
| Corrected                | Fixes to the OCR/transcription were required                            |
| Corrected and Ported     | Fixes to the OCR/transcription and code changes were required           |

Each program includes a like-named `.md` file that details what was done both from an OCR/transcription perspective and from a true "porting" perspective (i.e., accounting for the differences in BASIC dialects and system capabilities).

### Running these Games

The easiest way to run these games is to copy-and-paste the code directly from the GitHub file view into the Serial Terminal interface connected to your "BE6502", while it is running EhBASIC.  If you've not gone as far as implementing flow-control, and input buffering, you'll want to use my version of EhBASIC, as it fully supports those features.  If you use a different build, you'll need to set your "character pacing" in your terminal program to a value that prevents the data coming into the computer too fast (for the largest programs you'll need line pacing of 0.6s and character pacing of 0.02s).

You could, of course, **type** the code in yourself, but that might be a bit *too* much of a nostalgia trip even for me.

### Copy vs. Fork
Why a copy, not a fork?

- I don't intend to submit PRs upstream, since that would defeat the point of the original.

- I'm starting from a different set/combination of files.

## AI Usage

For my MS-BASIC ports, this was entirely minimal.  Less than 5% of the files there were touched by AI, and they weren't all source code files.

The joy, for me, in retro-computing and programming is about nostalgia.  Porting these programs was, while at times frustrating (as all programming efforts can be), very fulfilling.  It was a transport back-in-time.  It was an experience.  And carried some most enjoyable "learnings" (learning is my very favorite thing to do).

*Turning it over to AI would have robbed me of that.*

However, I've already had my programming nostalgia out of this little batch of BASIC programs, so this time AI is going to **do as much of the work as possible**.

In fact here I'm going to give it all of Maury's OCR/transcribed files, all of my MS-BASIC ports (purely to use for OCR/transcription corrections), and run an agentic AI process to do the conversions to EhBASIC.  If I like the end-result, I'll keep it and make the repo public ... if not, it'll never see the light of day.


## The "Bunny Bonus"

The original book omits a listing for "`bunny.bas`".

As a "celebration" (and a bit of fun), I decided to remedy that; details are in the "`bunny.md`" file.
