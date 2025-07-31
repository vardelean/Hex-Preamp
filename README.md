# Hex-Preamp
A GK3 Compatible Hexaphonic Pickup Preamp

## Design Considerations

The idea behind this project was to build a hexaphonic preamp that is Boss GK-3 Kit compatible while it would allow me to use the controls in a slightly different manner.
This design is based on the original GK-3 Kit schematic as published by Boss in their service manual. However, I did not want to have two separate volume controls, one for the Magnetic Pickups (from my guitar) and one for the Synth sounds (from the GK-3 Kit). I wanted to have just one volume control on my guitar for both Mag and Synth. 
In addition, I added a Balance control pot with a center detent to adjust the balance between the Mag pickups and the Synth sound. Since half of this pot (P1B) works as the Volume control in the GK-3, it can also be programmed for several other functions. The programming for this control is done via the Boss software, just like the Volume control in the GK-3 Kit. In my case, I can reprogram the Balance pot function via the VG-800 editor. 
Only one cable is coming out of the guitar, the 13pin cable. I don’t want 2 connectors, one for the GK-3 (13 pin) and the guitar’s jack. Therefore, I replaced the Strat’s jack with a 13 pin DIN connector.
Since I installed my board in a Strat, the 3 potentiometer knobs are now Volume, Balance and Tone.
The Volume and Balance work as explained above, but the Tone is placed at the output of the 5-way pickup selector switch, hence there is just one Tone pot for the 3 magnetic pickups. The Tone pot has no impact on the Synth sounds.

## Other Changes and Modifications of the Original GK-3 Kit Design
- I used better quality opamps (lower noise, lower distortion, and lower power consumption)
- Adjustable gain for each string. I have a GK-5 installed on another Strat that I use with my VG-800, and I noticed that a hotter output from the pickups would benefit the system’s SNR and the note recognition algorithms. Since on this kit I was going to use a Shadows Hex pickup (left over from an ATG Luthier Kit), I had no idea what the proper gain should be, so I decided for a gain trim per string.
- Adjustable gain for the guitar’s main pickups: this is to balance the mag sound compared to the Synth levels.
- Selectable input impedance for the guitar’s pickups to accommodate either SC or HB pickups (SW2). Not really needed, but I’m thinking on replacing the bridge pickup with a humbucker at one point, so this switch may come in handy.
- Selectable input capacitance for the guitar’s pickups to emulate different cable lengths (SW1). I prefer the sound of my SC pickups through a short cable. A preamp removes the cable’s capacitance impact on the pickup’s resonance frequency, so I decided to add a switch that could emulate the cable’s capacitance.
- The Volume control, P2, is a supposed to be a stereo pot, half Log / half Lin.  I couldn't find such a pot, so I decided to make my own custom pot from two stereo pots, one Log and one Lin.
- The Balance pot, P1, is a stereo Lin pot with a center detent. 
- The schematic shows a toggle switch for the UP/DOWN selector (SW3). In my Strat implementation, I used 2 separate tactile switches instead. Either option works well.
- The wiring from the main board’s J2 connector to the 13pin DIN connector was done via an FFC cable. Feeding the FFC cable from the main board to the 13pin connector in a Strat body turned out to be a bit of a challenge. If I ever decide to make another version of this board, I may consider using a different type of cable.

## Power 
The board is powered via the 13pin connector, just like the regular GK-3 Kit. 

## Connectors
JST 1.5mm connectors everywhere except for the FPC connector.

