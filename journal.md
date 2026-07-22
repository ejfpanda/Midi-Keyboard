# Midi Keyboard

## Day 1 July 18th 2026 , Cumulative time: 2 Hours

I went into KiCad and added the raspberry pi pico and then connected the +3v3 and ground symbols.

Then I added 30 switches for now and 30 diodes to make matrix wiring.

I decided to split it with high octave keys and low octave keys.

I first did the high octave keys and went with 2 rows and 5 columns. 

The matrix wiring took me less time than my last project, as I didn't have to learn it all over again.

I then went ahead and made the low octave key matrix with 2 more rows and again 5 columns.

Next I put the global labels onto the raspberry pi pico.

I also added two rotary encoder switches and added the encoder button matrix.

I also put in an LCD and SD card using an 8 pin connector for LCD and 4 pin with SD card.

Then I tried to add in the I2S DAC, but I was researching it and was very confused on how to put the footprint and symbol in at first but got it eventually and I had to ask how to connect everything from a friend.

## Day 2 July 19th 2026, Cumulative time: 4.5 hours

I started this day almost into July 20th, so I was kinda tired.

I went over everything in the schematic because I still wasn't sure about everything.

Then I transferred the schematic over to the PCB editor.

I had a tough time trying to organise everything because I wasn't sure what the best way was of connecting everything in a nice layout.

I settled on one way eventually and hammered at it for like 2 hours until I realised I had gone wrong somewhere because I couldn't find a way to get two components to route together.

The hard part was that some of my footprints were so small that you couldn't cram too many wires near or in it.

So I got stuck and then I gave up for the night.

## Day 3 July 20th 2026, Cumulative time: 8 hours

I remember this day was very frustrating because I'd spent like an hour rerouting everything twice but both times my computer crashed and I forgot to save.

So on the third time when I routed it I made sure to save every few seconds but then it just didn't crash.

I was very happy with the second time I routed it and a bit less happy with the final time but it's still ok.

I then finished the day by adding 3D models to all of the components, getting it ready for export to CAD.

I also started the CAD for almost an hour. 

I started by doing the sketch for the base and importing the board, before suddenly realising I had forgotten mounting holes in the board, so I went back and did that.

## Day 4 July 21st 2026, Cumulative time: 12 hours

I continued with the CAD.

I made the base with mounting holes.

I then used a fastened mate to connect the base with the board.

The base has an indent along the inside, with the outsides extruded more so that the board can rest inside a border.

The outside is smooth due to the use of Fillet within Onshape.

I then proceeded with the lid.

At first I tried to leave most of the 3D parts uncovered, but then I realised that looked ugly.

My final plan was to raise the level of the lid by extruding the corners and then have only the keys, the rotary encoders and the raspberry pi pico sticking out.

I also removed a section of the base of the board and lid which covered the USB.

## Day 5 July 22nd 2026, Cumulative time: ?? hours

Today, I made the firmware code.

I added the key matrix.

I added the fact that one of the rotary encoders changed the octave, and the other changed the midi channel.

I also added the LCD code for the display and the background, with labels which updated with octave shifts and channel changes.

Finally the main loop, where the midi was notified of key presses.

Also there is a time.sleep of 0.001 for a delay in order to prevent CPU overload.




