# nucleo-morpho-shields

>[!WARNING]
> **THIS REPOSITORY IS WORK IN PROGRESS**
>
> There could be incorrect tolerances.

KiCAD library for prototyping shields on Nucleo64 boards utilising Morpho connectors.

## Idea

The idea is inspired by proto-shields for Arduino UNO, but I needed one for Nucleo64 boards to be used in KiCAD 9. No suitable part was found in the KiCAD repository. I therefore decided to make my own.

Specification:

- stackable on top of the Nucleo64 board via the Morpho connectors
- contains a cut-out for easy access to the on-board tact buttons
- fits within the outline of the Nucleo board
	- no parts are exposed outside the main board
	- includes the lower part of the Arduino UNO with a cut-out
- contains mounting holes in the same locations


## Structure of the repository

### Folder `libraries`

Contains the footprint and symbol libraries:

- `Morpho-Nucleo64.kicad_sym` : symbol for KiCAD
- `Morpho-64.pretty` : footprint with outer dimensions

### Folder `dimension_references`

Contains documentation from STMicroelectronics and Arduino. These were used to retrieve and derive the dimensions of boards.