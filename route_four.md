# Route Four Sequential Switch

### Introduction

The Route Four is a sequential switch with control over direction as well as reset. Alternatively the active step can be selected via binary addressing.

It’s made up of four bi-directional switches which are normalised on one side, meaning the switch can be used in a number of ways including 4 to 1, 1 to 4 and 4 individual switches.

![RouteFour01](https://user-images.githubusercontent.com/14010890/227321097-7448b3f8-9711-4ef5-9bbc-f59fdb2e2f44.png)

### The Panel
The panel for this module is double sided so can be fitted either way up. For the purpose of this manual we will assume the panel is fitted with the controls at the bottom and switches at the top. If you’ve fitted the panel the other way round please rotate this manual 180 degrees to read!!

At the top of the panel we have the four switches. Each switch has an LED between the jacks to indicate which stage is active. Below the LED is a binary representation of the switches address.

When the module is in Address Mode the filled circles indicate which of the up/down or step buttons or input jacks need to be pressed or high to select that stage.

The arrows on the right hand switch jacks indicate that this column is normalised together. This normalisation is in a loop so placing a patch cable in any of the right hand jacks connects you to all of them until another jack is inserted.

Here’s a video which hopefully makes things a bit clearer!

<a href="http://www.youtube.com/watch?feature=player_embedded&v=0Fd_a8_5U2g" target="_blank">
 <img src="http://img.youtube.com/vi/0Fd_a8_5U2g/mqdefault.jpg" alt="Watch the video" width="640" height="360" border="10" />
</a>

### Controls
Below the switches we have the 3 control inputs. Up/Down selects which direction the switch is clocked. Reset sets the switch back to stage 00 and the Clock input moves the switch to the next stage.

All of these inputs are comparator based meaning they will operate with any signal that crosses the switching threshold – meaning that as well as gates and triggers, bipolar signals from LFO’s and oscillators along with signals such as envelopes can also be used as long as they have a high enough amplitude.

The threshold voltage is approximately 1.5volts and the maximum frequency that will switch is approximately 3kHz.

Moving further down the panel we come to the two mode switches.

#### Momentary/Latching switch.

In Count mode this switch will only effect the Up/Down input or button. In Address mode the switch effects the Up/Down and Clock inputs along with the Up/Down and Step buttons.

When the switch is set to momentary the Up/Down and Clock inputs will be high as long as the signal into them is high and the Up/Down and Step buttons will have effect as long as they are held.

When the switch is set to latching each time a high signal is put into the Up/Down and Clock inputs or either the Up/Down or Step Buttons are pressed that stage toggles between high and low.

#### Address Mode

This mode enables each stage to be selected via it’s 2 bit binary address.

<table>
  <tr>
    <th>Up/Down Input or Up/Down Button</th>
    <th>Clock Input or Step Button</th>
    <th>Active Stage</th>
  </tr>
  <tr>
    <th>Input Low or Button Unpressed</th>
    <th>Input Low or Button Unpressed</th>
    <th>00</th>
  </tr>
  <tr>
    <th>Input Low or Button Unpressed</th>
    <th>Input High or Button Pressed</th>
    <th>01</th>
  </tr>
  <tr>
    <th>Input High or Button Pressed</th>
    <th>Input Low or Button Unpressed</th>
    <th>10</th>
  </tr>
 <tr>
    <th>Input High or Button Pressed</th>
    <th>Input High or Button Pressed</th>
    <th>11</th>
  </tr>
  </table>

At the bottom of the panel we have 3 buttons for manual control of the switch. Every effort has been made in the design of this module to give a clean switching action when the buttons are used.

The Up/Down, Reset and Step Buttons can be used alongside inputs. Each of the buttons is linked with it’s associated input with a logical OR function. This means for instance, if the Up/Down input is being held high pressing the Up/Down button will have no effect as that control is already high. 

The electronic switches used in this module have a low on resistance (the datasheet states max 35Ω), meaning they have only a very slight effect when switching pitch control voltages. This will of course vary with the input impedance of any oscillator and the output impedance of any control voltage source.

### Build Document
[Here’s a link to build information for the DIY kit.](https://docs.google.com/spreadsheets/d/1wg_cqzuiyMHKkDE1c4eYfdx2wnnBMyvDsO1Q1nh9thw/edit?usp=sharing)

[Route Four Control PCB Schematic](https://drive.google.com/file/d/1SEDUfgUpgz0OHHfbPysNAR-r1CHpate0/view?usp=sharing)

[Route Four Circuit PCB Schematic](https://drive.google.com/file/d/1UQmjEb9ceqT8M1Nsj4mG_63FK3dNioVL/view?usp=sharing)

[Route Four Power PCB Schematic](https://drive.google.com/file/d/1siXZ0h-GG-4yiGUy0K7xZ9Q8PY5frM8F/view?usp=sharing)
