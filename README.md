# debug80-tec1

Machine setups for the Debug80 TEC-1 platform.

## Layout

- `tec1-mon1/`: MON-1 configuration (RAM starts at `0x0800`).
- `tec1-mon2/`: MON-2 configuration (RAM starts at `0x0900`).
- `roms/tec1/`: ROM images used by the setups.

Each machine folder contains a `.vscode/debug80.json` with multiple targets.
Select a target to assemble, load, and debug a specific program on that machine.

## Programs

Current targets per machine:
- `serial` (bit-banged serial demo)
- `matrix` (8x8 LED matrix test)

You can add more programs by dropping new `.asm` files into the `src/` folder
and adding another target in `.vscode/debug80.json`.
