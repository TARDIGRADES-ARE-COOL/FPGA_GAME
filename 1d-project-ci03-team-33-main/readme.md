# Keep Talking or the FPGA Explodes

Keep Talking and Nobody’s FPGA Explodes is a high-stakes, real-world electronics puzzle game inspired by Keep Talking and Nobody Explodes created by Steel Crate Games. The twist is, rather than a virtual online game, this is a physical mockup!


**Number of players**: 2+

**Procedure**: The 7 segment displays the timer countdown from 3 minutes. A player, the Expert, is given the instruction manual, while the Technician carries out his orders. Based on the pair’s ability to decode the incomplete instruction to defuse the bomb, the Technician will solve the modules. The game runs for 3 minutes, and ends once the timer runs out, or when the players successfully completes all three modules.

**Winning Condition**: The players complete all three modules to win the game. Otherwise, they lose.


## Game Modules

There are three modules:
  1. Red big button
  2. Wire sequence
  3. button sequence

## Controls and Displays

* Game timer: io_led[2]
* start game : io_dip[0][1]

* Rbb : io_button[0]
* Wire sequence button : io_button[1]
* button sequence : io_button[3]

* io_led[0][0] = led on rbb
* io_led[0][1] = led on wire 
* io_led[0][7] = led on button
* io_led[0][6] = win or lose indicatore

When modules are completed, the leds light up and timer stops.







