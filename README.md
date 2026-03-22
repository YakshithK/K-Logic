# K‑Logic Devboard

K‑Logic is a devboard I designed by following the Stasis starter devboard guide. my first PCB that goes! [stasis.hackclub](https://stasis.hackclub.com)

## What this is

- USB‑C powered devboard built with an RP2040
- Designed using the Stasis starter project flow (schematic → layout → silkscreen → fabrication)

## How to use it

- Plug it in over USB‑C.  
- Flash your firmware onto the main microcontroller.  
- Use the headers to hook up whatever logic / stuff you want.

## Why I built it

I've always wanted to get into hardware tech in general and I knew PCBs were going to be my first project in hardware after I found out about Stasis.

## Project structure

- `Journal/` – build log entries for each step (schematic, layout, silkscreen, fabrication, etc.). [github](https://github.com/YakshithK/K-Logic)
- `prod/` – production ZIP I sent to JLCPCB (gerbers + fab files). [github](https://github.com/YakshithK/K-Logic)
- `prod-files/` – BOM, CPL, and other manufacturing‑related files. [github](https://github.com/YakshithK/K-Logic)
- `DRC.rpt` – final DRC report from KiCad. [github](https://github.com/YakshithK/K-Logic)

## Screenshots

I have a bunch of screenshots of:

- Schematic in KiCad  
- PCB layout & 3D view  
- Silkscreen art and labels  
- JLCPCB upload / PCBA screens  

Check the `Screenshots/` dir

## BOM (short version)

Full BOM with links is in `K-Logic-Devboard-BOM-JLCPCB_Assembly_Order.csv` and `prod-files/`

| Part            | Value      | Notes                          |
| --------------- | ---------- | ------------------------------ |
| MCU             | (see BOM)  | Main brain of the board        |
| Flash memory    | W25Q16JVUXIQ | External flash for storage   |
| USB‑C connector | —          | Power + data input             |
| LDO regulator   | —          | Regulates USB power            |
| Passives        | various    | Resistors, caps, etc.          |