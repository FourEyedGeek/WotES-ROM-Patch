# Warriors of the Eternal Sun – ROM Patch

> **This patch requires PlanetChili's V2.0 patch.** It does not apply to a clean ROM.
> Patch the clean ROM with [PlanetChili's V2.0 patch](https://github.com/planetchili/wotes_patch) first, then apply this one.

A community ROM patch for *Dungeons & Dragons: Warriors of the Eternal Sun* (Sega Genesis / Mega Drive), built on top of PlanetChili's V2.0 patch. It fixes bugs and adds quality of life information screens for players who like to see the numbers. It is designed to run in emulators, on FPGAs, and on Flash Carts.

See [CHANGELOG.md](CHANGELOG.md) for the full list of changes.

## Installation

You need your own clean ROM. No ROMs are provided.

1. **Clean ROM:** `Dungeons & Dragons - Warriors of the Eternal Sun (USA, Europe).md`
   SHA-1 `9135F7FDA03EF7DA92DFADE9C0DF75808214F693`
2. **Apply PlanetChili's V2.0 patch** to the clean ROM, following the instructions in [planetchili/wotes_patch](https://github.com/planetchili/wotes_patch).
   The result must be: CRC32 `405ED24B`, SHA-1 `2380B201B872F7BD2C66F2A4D82DF86709332D55`
3. **Apply `WotES-ROM-Patch-v0.40b.bps`** to that Chili V2.0 ROM using [Floating IPS (Flips)](https://www.romhacking.net/utilities/1040/) or [Rom Patcher JS](https://www.marcrobledo.com/RomPatcher.js/). Save it as a new file.
   The result must be: CRC32 `D698CD36`, SHA-1 `11A37009C1DC0187434677AD7837E355BA5E0924`
4. Play it in your emulator or copy it to your flash cart.

If the patcher reports a checksum mismatch, your input ROM is not the Chili V2.0 ROM above.

**Saves:** in-game battery saves carry over. Do not load emulator save states made with a different version.

## Status

Tested in emulators (Kega Fusion, Genesis Plus GX). Not yet tested on original hardware or FPGA; reports are welcome.

## Credits

- **PlanetChili** – the V2.0 patch this work is built on: [planetchili/wotes_patch](https://github.com/planetchili/wotes_patch)
- **FourEyedGeek** – this patch

## Legal

Not affiliated with or endorsed by Sega, Westwood, Hasbro/Wizards of the Coast or PlanetChili. No game data or ROMs are distributed; all rights to the original game remain with their respective holders. PlanetChili's patch is their work and is governed by their own terms. The original work in this repository is released under the [MIT License](LICENSE).
