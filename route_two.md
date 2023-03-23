# Route Two Dual Switch

### Introduction

The Route Two is a dual switch module with each channel made up of two switches normalised as a Single Pole Double Throw (SPDT) switch. The switches are bi-directional meaning they can be used to switch signals in either direction.


### The Panel

The panel for this module is double sided so can be fitted either way up. For the purpose of this manual we will assume the panel is fitted with the controls at the bottom and switches at the top. If you’ve fitted the panel the other way round please rotate this manual 180 degrees to read!!

The two channels are identical so for most of this manual we’ll just talk about a single channel. Further down the page are a number of videos to illustrate various aspects of the switches operations.

At the top of each channel we have the two switches. The two middle connectors are normalised together so putting a single patch cable into either connector connects to both – putting a patch cable into both breaks the normalisation and each cable connects only to the switch it’s plugged into.

Each switch has an LED between the jacks to indicate which stage is active. The graphics for each switch indicates the initial states for each switch. One is normally closed, the other normally open. As the switch is activated the two switches swap states.

The connectors below the switches are for Gate Output and Clock Input.

The Gate Output differs depending on which mode the channel is in. In momentary mode it’s high when the Clock Input is high or the Pushbutton is pressed. In Latching mode it goes to a divide by two mode – going high on the first clock signal or button press and low on the next.


The Clock Input is comparator based meaning it will operate with any signal that crosses the switching threshold. This means that as well as gates and triggers, bipolar signals from LFO’s and oscillators along with signals such as envelopes can also be used as long as they have a high enough amplitude. The threshold voltage is approximately 1.5 volts and the maximum frequency the module will switch at is approximately 3kHz.

Moving further down the panel we come to the mode switch. There are two modes – momentary and latching. In Momentary mode the switches swap states as long as the clock is High or the Pushbutton is pressed. In Latching mode the switches change state each time a clock signal is received or the pushbutton is pressed.

The electronic switches used in this module have a low on resistance (the datasheet states max 35Ω), meaning they have only a very slight effect when switching pitch control voltages. This will of course vary with the input impedance of any oscillator and the output impedance of any control voltage source.

### Normalising one channel to the other

There are two jumpers on the board that enable you to normalise one channel to the other – this allows one channel to control the other until the normalisation is broken.

As the module can be used either way up with the reversible channel, it’s up to you which channel is normalised to which – or if you even want any normalisation at all.

The image below shows where one of the jumpers is fitted. To change or remove the jumper the back board will need to be removed by undoing the two screws and pulling the back board off.


The video below shows switching operation with the different modes. One channel is normalised to the other here to demonstrate how the normalisation works.


This next video illustrates how the switch can be used for dividing down.


This final video demonstrates how the normalisation between the two switches in each channel works.


### Build Document

[Here’s a link to build information for the DIY kit.](https://docs.google.com/spreadsheets/d/1wg_cqzuiyMHKkDE1c4eYfdx2wnnBMyvDsO1Q1nh9thw/edit?usp=sharing)

[Route Two Schematic](https://drive.google.com/file/d/1OwmmElXsMm2NfkOyAtBcOy8VB6d9OHcL/view?usp=sharing)
