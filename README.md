# marcus-bbbcape

Beaglebone Black cape for my robot, see:

- [marcus-base](https://github.com/miek770/marcus-base)
- [marcus-boucliers](https://github.com/miek770/marcus-boucliers)

The general goal is to reduce the amount of loose wires on the robot and the required space. The current platform is not compact at all, and adding more stuff (ex.: cannon, turrent, shields) seems like quite the challenge.

Ideally I would use Molex connectors but it would probably eat up too much space. I would like to keep the PCB as small as possible, mostly to keep the cost down. Right-angle headers would work as well, but I think I'll quickly run out of borders. Perhaps right-angle headers for stuff going down, and straight headers for stuff going up?

The cape should be stackable, which means that P8 and P9 should be female headers with long leads. The alternative would be male headers mounted on the bottom. Then again, with plenty of headers going up I probably won't be able to put another cape on top anyways. Still, having female headers allows me to add wires in the future for unplanned expansions.

## 1. To do list

- Add UART2;
- Add battery voltage monitoring (remember the 1.8V analog input limitation);
- Move the top headers' titles below them, otherwise they will be hidden by the right-angle headers I plan on using;
- Correct title, it's partially hidden by the P9 header;
- Output 6.5V somewhere other than for the camera. Some other system may very well need it;
- I don't like how the rangefinders' pins are mirrored, but I've added indications. If it's not too complicated I'd like to mirror 2 of them;
- Add an LED tied to an unused pin, for testing purposes;
- Double-check the big capacitor polarity. I would've thought the square pad to be for the negative pin, but the top silk screen says otherwise;
- Add headers 1st pin markers on all of them and resize the existing 1's (not existing ones but existing 1's);
- Document pins usage. Just need to integrate this info in marcus-base/modules/pins.py which holds a dictionary of pins usage.
