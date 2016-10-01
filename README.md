# EagleCAD ULP for NeoDen 4 PNP

The script file in this folder is a EagleCAD ULP (user language program) for exporting PCB for NeoDen 4 pick and place machine. It's based on an existing script file for TM-240A machine, but modified to match the format acceptable by NeoDen 4.

When running the script, it will ask for 'machine x-y coordinates of the first component'. Once the board position is determined (whether you use fixed tray method or PCB conveyor belt), you can locate the first component on the board in machine coordinates, and fill that into the dialog. The script will automatically translate PCB coordinates to machine coordinates.

The exported .csv file can be directly imported to NeoDen 4. For simplicity, I only enabled top layer, but you can modify the script easily to support exporting bottom layer too if your PCB is double sided.

