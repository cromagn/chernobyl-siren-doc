# Chernobyl Alarm Siren Documentation

Documentation project for a Soviet-era alarm siren circuit associated with the Chernobyl alarm infrastructure.

## Purpose

This repository collects and documents:
- the original schematic scan
- original component datasheets
- reconstructed SPICE/LTspice models
- a modern-build BOM for study and bench replication
- KiCad reconstruction work
- notes about assumptions, substitutions, and uncertainties

This project is intended for historical, educational, and technical documentation.

## Repository structure

```text
assets/        Original images and scans
bom/           BOM files for KiCad / Digi-Key
datasheets/    Original component datasheets
docs/          Technical notes and reconstruction notes
hardware/      KiCad schematic files and related material
spice/         LTspice / ngspice models
```

## Original parts identified so far

### Transistors
- MP26B / МП26Б — germanium PNP
- P702 / П702 — silicon NPN power transistor

### Diodes
- D237A / Д237А

### Capacitors
- K50-6 / К50-6
- K42U-2 / К42У-2

### Speaker
- 4GD-35 / 4ГД-35, 8 ohm

## Important note on simulation and replication

The currently included SPICE models are engineering approximations, not official vendor models.

A bench-built modern version may not sound exactly like the original, especially if:
- silicon substitutes are used in place of germanium devices
- the original loudspeaker is replaced
- transistor leakage and temperature behavior differ from original Soviet parts

## Status

Work in progress.

Current status:
- [x] original schematic scan collected
- [x] original transistor datasheets collected
- [x] initial LTspice models prepared
- [x] initial Digi-Key BOM prepared
- [ ] KiCad schematic fully validated
- [ ] waveform validation against hardware
- [ ] exact historical configuration verified

## License

Documentation text in this repository is released under CC BY 4.0 unless otherwise stated.

SPICE models, scripts, and original reconstruction files are released under MIT unless otherwise stated.

Scanned historical materials may be subject to their original rights status; they are included here for identification, preservation, and study.
