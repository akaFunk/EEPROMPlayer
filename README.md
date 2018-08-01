# EEPROMPlayer
The EEPROMPlayer is an audio player that can play audio from an (E)EPROM using no microcontroller, but only simple logic ICs and an analog audio amplifier.

The EPROM used is compatible to standard 27C010 EPROMs. The clock is generated using an NE555 timer and then diveded several times using 74LS74 flip-flops. Each clock signal is fed to one of the address lines of the EPROM. The EPROM holds the raw audio data in 8 bit. The 8 data lines are passed into an R2R-network which does the digital to analog conversion. An LM386 is used to amplify the signal.

## Images
![Version 1 using a breadboard](https://raw.githubusercontent.com/akaFunk/EEPROMPlayer/master/images/version1.jpg)
![Version 2 using a milled PCB](https://raw.githubusercontent.com/akaFunk/EEPROMPlayer/master/images/version2.jpg)
