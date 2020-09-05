# Freeboard Blocks


## Abstract
A while ago i bought a seaboard block secondhand, seemed fun and it was a really good offer, but then i realized that without one of the blocks or a specific app in windows or IOs phone (neither of wich i have or want to have) i could not change the settings for it, not even the mode or sensitivity of any of the dimensions.

So i dove into the developer material and figured that i could do something with what @Abhoth did, but take it further and make it standalone. and after a pair of sleepless nights i got it working properly, so here it is

## TL;DR

This script frees your roli seaboard blocks from the desktop applications and mobile(only IOS) app to change the settings, making them available in the board itself.

Basicly I made the mode switch and LED into a kind of a shift key, that enables:
- Changing between MPE and normal MIDI mode
- Activating Piano mode
- Setting different sensitivities to each of the mpe dimensions
- Setting midi channels
- Uses octave up and down switches for modesetting (when shift is pressed).
- Deactivates octave up and down switches except for the ones on the "outside", for when you join multiple keyboards.

All this is done by using mode button + another key in the keyboard 

## Usage
**OVERLAY COMING**

If pressing mode button, octave down enables "normal" midi operation, and octave up enables MPE mode

Mode light colour:
  * Teal -> If MPE mode
  * yellow -> normal mode
  * orange -> piano mode off

If not the leftmost block, ignore the octave down key and if not the rightmost block, ignore octave up key (this only applies for multiple blocks together).

There are 3 zones considered, Top row *top flat row over the keys*, bottom row *same, but at the bottom* and the keys themselves.

Oher settings that can be accesed with Mode button:
  * First octave keys: Midi start channel in the key itself, end channel in the bottom row of each key. (C is 1, c# is 2.... until b).
  * Piano mode switch top row Csharp
  * Fixed velocity switch top rpw Dsharp
  * set poly aftertouch top row Fsharp
  * Aftertouch default top row Gsharp
  * Aftertouch disable top row Asharp
  * The second octave is used for settings, defaults and some toggles. the sharps are velocity, lift, glide, slide and press "sliders", and reset to default when pressed over the top row over the keys

All changes in config sync between all blocks in the chain

## Installation instructions
**PROPER INSTALL INSTRUCTIONS COMING**

OF COURSE IF YOU BREAK YOUR DEVICE I AM NOT RESPONSIBLE, do it at your own risk, however this is not hacking anything and should something happen it should be within the warranty (DIDN'T LOOK IT UP, YOU DO YOU).


But basicly you need to download the [IDE](https://juce.com/blocks/code), paste the script and flash it to the device after connecting it.

### References
- IDE https://juce.com/blocks/code
- https://docs.juce.com/blocks/group__LittleFootFunctions.html#ga70967dcba6beea8a66f216f75619ff35 
- https://docs.juce.com/master/group__LittleFootFunctions.html
