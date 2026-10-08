# DOS 286 Emulator

A PC/AT 286 on a monochrome screen in your browser: a boot sequence, a DOS-style prompt, and a built-in BASIC.

![DOS 286 Emulator screenshot](<DOS 286 Emulator - screenshot.png>)

## What's in it

- **`dos286-emulator.html`** is an original simulation of a 286 at 12 MHz: memory test, a SmartDrive-style startup, a QuickMenu-style menu, DOS commands like `DIR`, `TYPE`, `MEM` and `VER`, and a GW-BASIC-style interpreter (`PRINT`, `INPUT`, `LET`, `IF`, `FOR`/`NEXT`, `GOTO` and more). It's not real MS-DOS software
- **`real-dos-jsdos.html`** boots a real DOS-compatible shell with js-dos (DOSBox in WebAssembly). It can run real 16-bit programs you drop in, or boot a FreeDOS image if you set a bundle URL inside the file

## Run it

**Simulation:** download `dos286-emulator.html` and open it in your web browser. Click the screen, then type.

**Real DOS:** it has to be served from a local web server. In this folder run `python3 -m http.server 8080`, then open `http://localhost:8080/real-dos-jsdos.html`.

---
Made by hardwaremack.
