# Bare Metal Experiments in Rust

A simple and minimalist bare metal code experiment for microcontroller learning purposes, using simple examples like a blinking LED program, written in Rust using only core-lib.

## Overview

This project demonstrates bare metal programming in Rust on microcontrolers. It implements a few program examples that runs entirely without an operating system, using only Rust's core library and direct hardware manipulation.

**Boards**
* [Arduino Uno SMD R2](docs/arduino_uno_smd_r2.md)
* [ESP32 TTGO T-Display](docs/esp32_ttgo_tdisplay.md)

### Project Structure

```
bare-metal-rust/
├── Cargo.toml                  # Minimal dependencies (only core library)
├── README.md                   # Project description
├── .cargo/                     # Cargo configuration
├── docs/                       # Hardware setup and instructions
│   ├── arduino_uno_smd_r2.md
│   └── esp32_ttgo_tdisplay.md
└── src/bin/
    ├── arduino_uno_smd_r2/     # Arduino UNO(Xtensa-LX6/AVR) source codes
    │   └── blinks.rs
    └── esp32_ttgo_tdisplay/    # ESP32(Xtensa-LX6) source codes
        ├── blinks.rs
        └── linker.ld
```

## Useful resources

* How to write [the smallest rust no-std code](https://docs.rust-embedded.org/embedonomicon/smallest-no-std.html).
