# Fortunes: Geomancy

![Agrippa's Geomantic Figures](figuresplanetaryrulers.jpg "Geomantic Symbols")

- Illustration: from Agrippa's "De Occulta Philosophia" (1533)

## Based on Cornelius Agrippa's "De Occulta Philosophia" (1533)

The fortunes random quotes are often used in UNIX / Linux systems for random quotes. But a connection to the art of fortune telling as taugt by the hermetic philosophers was never made. So here is the first real fortune telling plug for the Linux fortune teller.

The origin of the geomantic figures are unknown. Geomancy was known by renaissance magi. The Geomantic fortune symbols are described by Agrippa von Nettesheim in the chapter: *"De Geomantia, Hydromantia, Acromantia, Pyromantiaquatuor elementorum diuinationibus" (Cap. LV)"* in "De Occulta Philosophia" (1531 - 1533) and in the illustrations of this work.

The geomantic figures were also used used by the adepti of the *Hermetic Order of the Golden Dawn* (est. ca. 1888). Aleister Crowley (1874 - 1947) used geomancy on a regular basis, which is evident in his diaries. 

Because the geomantic symbols are of a binary nature, they'll work so much the better on a computer.

Per Thykjaer Jensen, F.R.C.   
Die Walpurgis, 20250430   

## How to create your own fortune files

In your favorite editor just collect some sentences, and divide them by a %-character. Do it something along these lines:

~~~~
"Do what thou willt shall be the whole of the Law."
   - Aleister Crowley (1875 - 1947)
%
"Nothing beats two guitars, bass and drums."
   - Lou Reed (1942 - 2013)
%
"And so on."
   - Per Thykjaer Jensen
~~~~



## Install

### Install fortune

If you don't have fortune, you'll have to install the program first. 

### Execute the plugin

Copy the geomancy and geomancy.dat files to `/usr/share/games/fortune`. Then run:

`fortune geomancy` in a terminal. 

### Mac

On a Mac you'll have to find out where Fortune's files are kept. On my system they are here:

~~~~~
/opt/homebrew/opt/fortune/share/games/fortune
~~~~~

As above just copy the two files to the directory.

### Create a new *.dat file

Fortune will need both the file with your quotes and a *.dat file. You can create a new *.dat file like this:

~~~~~
rm geomancy.dat
strfile -c % geomancy geomancy.dat
~~~~~

This will create a new .dat for Mac. Now copy the files to the fortune folder mentioned above.