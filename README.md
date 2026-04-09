![Chernobyl Siren](assets/hero.png)

# ☢️ Chernobyl Alarm Siren — Reverse Engineering & Documentation

![Status](https://img.shields.io/badge/status-work_in_progress-orange)
![License](https://img.shields.io/badge/license-MIT%20%2B%20CC--BY-blue)
![KiCad](https://img.shields.io/badge/KiCad-9.x-blue)

---

## 🎥 Source Video

The original schematic was derived from this video: The Last Alarm of Chernobyl's SKALA Computer (Chornobyl Family)

👉 **[Watch on YouTube](https://www.youtube.com/watch?v=xC0qYnh_3Fw)**

---

## 🧭 Why this project exists

This repository aims to preserve, understand, and reconstruct a piece of **analog engineering history**.

The circuit analyzed here represents:

* Soviet-era semiconductor design choices
* germanium  transistor behavior
* analog sound generation techniques used in critical infrastructure
* a real-world artifact tied to one of the most significant events in modern history

This is not just a circuit.
It is **engineering under constraints, in context, and under pressure**.

---

## 📦 Repository structure

```text
assets/        Original scans and images
datasheets/    Original Soviet component datasheets
hardware/      KiCad schematic reconstruction
spice/         LTspice / ngspice models
bom/           BOMs (modern + KiCad import)
docs/          Technical notes and assumptions
```

---

## 🔬 What is inside

### 🧾 Original components (identified)

| Type       | Original Part   | Description       |
| ---------- | --------------- | ----------------- |
| Transistor | MP26B / МП26Б   | Germanium PNP     |
| Transistor | P702 / П702     | Germanium NPN power |
| Diode      | D237A / Д237А   | Rectifier         |
| Capacitor  | K50-6 / К50-6   | Electrolytic      |
| Capacitor  | K42U-2 / К42У-2 | Film              |
| Speaker    | 4GD-35 / 4ГД-35 | 8Ω loudspeaker    |

---

## 🧪 Simulation

```spice
.include chernobyl_siren_models.lib
```

⚠️ Models are **engineering approximations**, not official vendor models.

---

## ⚠️ Authenticity vs reproducibility

| Mode          | Description                             |
| ------------- | --------------------------------------- |
| 🟢 Historical | Original components, authentic behavior |
| 🔵 Modern     | Substitutes, reproducible build         |

👉 These will **not sound identical**

---

## 🔍 Open questions

* 


See `docs/reconstruction-notes.md`

---

## 🤝 Contributing

Contributions welcome:

* schematic fixes
* better SPICE models
* historical sources
* real measurements

---

## ⚖️ License

* Documentation → CC BY 4.0
* Technical assets → MIT

---

## 🧭 Final note

This project sits at the intersection of:

* electronics
* history
* reverse engineering

It is an attempt to understand not only *how it works*,
but also *why it was built that way*.
