[h1]Spoolman Setup - Automatic Filament switch[/h1]

Spoolman:
- follow instalation guide of spoolman
- dont forget to add the suggested macros !
- add ur spools to spoolman
- note down the ID of any added spool

Orca Slicer
- open Orca Slicer
- add/choose Filament (u need to setup every filamet)
- open filament settings page, open GCode Tab
- add the following line:

SET_ACTIVE_SPOOL ID=#

(#, must be changed to the spool ID you note down)
- repeat this for every filament, and change the ID so it matches with spoolman

Mainsail/Fluidd:
open ur printer.cfg or the file where ur end maceo is found:

add this line into the macro:
CLEAR_ACTIVE_SPOOL 

this line clears the spool at the end of the print.
