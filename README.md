# EagleCAD ULP for NeoDen 4 PNP

neoden4-mountsmd.ulp is a merge of rayshobby noeden script and the original mountsmd.ulp.  The purpose is to output component coordinates from EagleCAD to a format suitable for use by the NeoDen4 pick and place machine.  Save the ulp to eagle's ulp directory, and run it from the PCB editor.  It makes no changes to the board, it only generates csv lists of top and bottom SMD components for the placer.

This script adds double sided output (layers 1 - top and 16 - bot) and uses rayshobby formatting and angle calculation merged into the behavior of the original mountsmd.  This script does not request machine coordinates of the first component.

When importing the bottom side into the NeoDen software, make sure that "mirror bottom side" checkbox is checked.  Upon import, the NeoDen software will recompute all the x coordinates to account for the flip.  All coordinates are recomputed based on the location of the first component, either from your BOM list, a fiducial or manually added via for alignment.


