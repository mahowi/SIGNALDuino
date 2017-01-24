# SIGNALDuino uC v3.3-0 (development version)
# (edited, so it can be compiled with Arduino IDE)

System to receive digital signals and provide them to other systems pro demodulatiob. Currently tested with 433 MHZ, but not limited to that frequency or media.

### Getting started

Just copy the folder into your Arduino sketchbook and compile with Arduino IDE.

### Using SIGNALDuino in FHEM

If you want to use the SIGNALDuino with FHEM, you can use it directly from FHEM. No need to compile any sourcecode.
You find more Information here:
http://www.fhemwiki.de/wiki/SIGNALDuino


### Tested microcontrollers

* Aduino Nano

### Signal from my device ist not detected

We have a pattern detection engine, that detect several signal types. Maybe not all, but most of them.

Uncomment #define debugdetect in libs/remotesensor/patterdecoder.h
Search for some output which describes a pattern with serval bits received.
If you find something, open an issue and provide as much information as possible.


### You found a bug

First, sorry. This software is not perfect.
1. Open a issue
- With helpful title - use descriptive keywords in the title and body so others can find your bug (avoiding duplicates).
- Which branch, what microcontroller, what setup
- Steps to reproduce the problem, with actual vs. expected results
- If you find a bug in our code, post the files and the lines. 

### Contributing

1. Open one ore more issue for your development.
2. Ask to be added to our repository or just fork it.
3. Make your modifications and test them.
4. Create a branch (git checkout -b my_branch)
5. Commit your changes (git commit -am "<some description>")
6. Push to a developer branch (git push dev-<xyz >my_branch)
7. Open a Pull Request, put some useful informations there, what your extension does and why we should add it, reference to the open issues which are fixed whith this pull requet.
