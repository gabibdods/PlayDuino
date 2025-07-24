# 🎵 Arduino Music Player – A Modern Tribute to a Family Heirloom

This project is a personal and technical tribute to a cherished childhood object: my grandmother’s old music box. As an aspiring electronics engineer, I set out to recreate the experience—not as a mechanical device, but as a modern **Arduino-powered music player**.

---

## 💡 Problem Statement

When I was very young, I used to fall asleep listening to a wind-up music box passed down from my grandmother. Over the years, mechanical degradation and heat exposure rendered it non-functional.

Rather than attempting a direct mechanical repair, I saw an opportunity to **honor its legacy** while integrating it into my **engineering portfolio**: building a music player from scratch using an Arduino board, speaker, and audio output.

---

## 🎯 Project Goals

- ✅ Recreate the functionality of a traditional music box using an **Arduino board**.
- 🔊 Add support for **audio output via speaker and 3.5mm audio jack**.
- 🛠️ Write **all firmware and configuration from scratch**, avoiding third-party audio libraries where possible.
- 📦 Modularize the design so the board and peripherals can be reused or extended for future electronics projects.

---

## 🛠️ Tools & Technologies

| Tool / Technology | Purpose |
|-------------------|---------|
| **Arduino IDE**   | Primary development and firmware upload |
| **Custom VHDL IDE** | Created by me, used to document and experiment with embedded design principles |
| **Online Documentation** | Referenced for pinout diagrams, audio signal generation, and circuit validation |

---

## 🧠 Design Decisions

- ⚙️ Instead of repairing the old music box mechanically, I chose to **reimagine it electronically** to better match my long-term goals in electronics and embedded systems.
- ♻️ The **Arduino board** serves as a versatile foundation—not only for this music player, but also for future projects I may stack on top of this base.
- 🎚️ By including both a **speaker and audio jack**, I ensured flexibility in playback: either public or private listening.

---

## 📐 Hardware Overview

- **Arduino UNO or compatible board**
- **Mini speaker module**
- **3.5mm audio jack breakout**
- **Breadboard and jumper wires**
- **Optional push button or switch** for playback control

---

## 🔌 Wiring Summary

| Component         | Pin Connection       |
|------------------|----------------------|
| Speaker           | Digital Pin (e.g., D9) via transistor |
| Audio Jack (L/R)  | PWM-capable Digital Pins (e.g., D9/D10) |
| Optional Button   | Digital Pin + Pull-down resistor |

---

## 📁 Project Structure (Sample)

```bash
music-player/
├── src/
│   ├── music_player.ino        # Core Arduino sketch
│   ├── melodies.h              # Manually defined notes and delays
├── schematics/
│   └── wiring_diagram.png      # Breadboard layout and pinout (if created)
├── docs/
│   └── design_notes.md         # Personal notes and design reasoning
└── README.md                   # You’re here!
