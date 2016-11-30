# 3D Printing
Use best practices for the printer you're working with - these are general guides for printing the parts in this repository.

## Conversion
### Export
Inventor part files (.IPT) must be exported to a 3D format, typically STL, to be "sliced" in a program like Cura and 3D printed. Exporting can be done using the file menu (*File->Export->CAD Format*), or using the 3D printing environment (*Environments->3D Printing*) in Inventor Pro. Make sure to use **millimetres** as the unit for exporting, to ensure the scaling of the part is accurate.

### Splitting parts
The main mounting part in each of the prototypes is comprised of three separate solid bodies (the core and two clamps) which must be printed separately. One way to do this is to derive a new part from a *single* solid body in the multi-body part, using *Manage->Make Part*. The isolated part can then be exported and printed as normal.

## Supports
Many of the parts have distinct overhangs and holes which **must** be supported when printing: please use support-generation options in your slicing program, and enable these supports for all surfaces - *not just from the printing bed*.

If your printer requires it, use a 'raft' for bed adhesion and level printing. On an Ultimaker 2/3 this isn't necessary, but you should still use a 'brim' for the larger parts.

## Orientation
The parts should be oriented on the printing bed to minimise the amount of support necessary, and either in line with or at 90 degrees to any screw holes in the part (don't print at a 45 degree slant!). If the part has a large, flat surface, use this as the base.

## Quality
These parts need to fit together fairly precisely, and must be consistently strong in order to flex and mount properly. Use 0.1mm (100 micron) layers, and a nozzle no larger than 0.6mm. Don't push the printer's speed above recommended limits, as this will weaken and deform the part.

PLA material was used for the prototypes and should work fine for most purposes. However, PLA isn't particularly durable and weakens rapidly with heating, so if you want to make a durable prototype, or use hot glue on parts, then you should investigate ABS or other more advanced materials for printing.

## Post-processing
Remove support material by force - pliers help with this. Holes need to be cleared of support material, using a small screwdriver head or an undersized drill - don't bore out the holes too much, though.

Some holes may be slightly tight, depending on the printer and print settings. You can push or thread screws through.
