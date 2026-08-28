# spcwar-16k.bas

## STAR TREK -- EXTERNAL INSTRUCTIONS FOR THE 16K EDITION

The full conversion of `spcwar.bas` requires running EhBASIC on a machine with **24KB** of RAM.

Most [Ben Eater](https://eater.net/6502)-based machines, for which this series of ports is intended, will *only* have **16KB** of addressable RAM.

To fit the original game into 16KB, and meet the goal of having all of the 101 BASIC Computer Games ready-to-run for the standard BE6502, I created a cut-down version.

It has the same gameplay mechanics and options, but removes the in-game instructions; and they are presented below (and in spcwar-16k-instructions.md):

## Instructions
The galaxy is an 8 by 8 quadrant grid. Each quadrant is divided
into an 8 by 8 sector grid.

### Symbols
| Symbol | Meaning      |
| :---:  |--------------|
|   <*>  | Enterprise   |
|   +++  | Klingon      |
|  \>!<  | Starbase     |
|   \*   | Star         |

### Commands

| Number | Commmand                  |
| :---:  |---------------------------| 
|   0    |Set course and warp factor |
|   1    |Short-range sensor scan    |
|   2    |Long-range sensor scan     |
|   3    |Fire phasers               |
|   4    |Fire photon torpedoes      |
|   5    |Transfer energy to shields |
|   6    |Damage-control report      |
|   7    |Library computer           |
|   8    |End the game               |

### Course Directions

        4  3  2
         \ ^ /
          \^/
      5 ------- 1
          /^\
         / ^ \
        6  7  8

Fractional courses are permitted. Course 1.5 is halfway between
courses 1 and 2. One warp factor is the width of one quadrant.

### Long-Range Scan

The long-range scan uses a three-digit code. The hundreds digit is
the number of Klingons, the tens digit is the number of starbases,
and the units digit is the number of stars.

This is sometimes known as "**KBS**"; Klingons, Bases, Stars.

### Library Computer
The library computer provides three commands as follows:

- **0** - Galactic record
- **1** - Status report
- **2** - Photon-torpedo trajectory calculations