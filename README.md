# marcus-bbbcape

Beaglebone Black cape for my robot, see:

- [marcus-base](https://github.com/miek770/marcus-base)
- [marcus-boucliers](https://github.com/miek770/marcus-boucliers)

The general goal is to reduce the amount of loose wires on the robot and the required space. The current platform is not compact at all, and adding more stuff (ex.: cannon, turrent, shields) seems like quite the challenge.

Ideally I would use Molex connectors but it would probably eat up too much space. I would like to keep the PCB as small as possible, mostly to keep the cost down. Right-angle headers would work as well, but I think I'll quickly run out of borders. Perhaps right-angle headers for stuff going down, and straight headers for stuff going up?

The cape should be stackable, which means that P8 and P9 should be female headers with long leads. The alternative would be male headers mounted on the bottom. Then again, with plenty of headers going up I probably won't be able to put another cape on top anyways. Still, having female headers allows me to add wires in the future for unplanned expansions.

## To do list

- Disconnect the switch from the bumpers. It should be completely separate;
- Add other interfaces;
- Document pins usage. Not sure if this is really necessary, the schematic is clear enough. Just need to integrate this info in marcus-base/modules/pins.py which holds a dictionary of pins usage;
- Complete and check pretty much everything.
