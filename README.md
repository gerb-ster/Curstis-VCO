# Curtis-VCO

This module is based on the classic CEM3340 VCO chip, although I’m using a AS3340 clone. I’ve took some inspiration from the Maximus VCO design from Thomas Henry. The CEM3340 outputs 3 waveforms with different output levels. To achieve a uniform 10 vpp output around 0 volt, I used a series of op-amps. In the first step the 3 levels is attenuated to 10 vpp, in the next step it’s being offset with 5v to make it swing around 0 volt. I’ve used a trimpot to fine-tune the offset.

The triangle output is then used to ‘wave shape’ a sine output. For this, I also used a classic design from Thomas.

I’ve already made some changes to the PCB design, there was an issue with the power rails on the IO board (hence the bodge wire), some transistor values where wrong, and I made some more room for a good timing cap.

## Status: Finished

- done: first schematic & board design
- done: breadboard and test
- done: design frontpanel
- done: order PCB and build prototype