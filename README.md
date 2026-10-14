# Mini Macro EC11 — ZMK prototype

Prototype firmware source for a **nice!nano V2-compatible nRF52840**, 3 direct-wired switches, and an EC11 (rotation + push). Battery is intentionally omitted for the initial USB-powered test.

**See `ИНСТРУКЦИЯ_RU.md` for wiring and flashing directions in Russian.**

Files:
- `boards/shields/tiny_macropad/tiny_macropad.overlay`: GPIO wiring and encoder configuration
- `config/tiny_macropad.keymap`: A, B, C, media play/pause and volume controls
- `config/tiny_macropad.conf`: encoder support
- `build.yaml`: GitHub build target `nice_nano_v2` on ZMK v0.3

This archive contains **sources, not a precompiled UF2**. Hardware-specific assumptions (clone pinout, bootloader, encoder pulses) require validation. Do not connect battery until polarity and charging circuitry are verified.
