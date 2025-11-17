# SimSteeringFacePlate – Arduino USB Button Plate

This repository contains two versions of a simple and responsive **USB button plate** for sim racing wheels, built using an Arduino board with native HID support.
Both versions appear to the PC as a standard **USB Gamepad**, using the `Joystick.h` library.

---

## Versions

### **SimSteeringFacePlateV1**

A minimal version with **only push buttons**.
Suitable for steering wheels or button boxes that do not require an encoder.

### **SimSteeringFacePlateV2**

An extended version with **push buttons + a rotary encoder**, using hardware interrupts for fast and accurate detection.

Useful for menu navigation, brake bias adjustments, or incremental controls.

---

## Features

* USB HID gamepad (no drivers required)
* Low-latency button handling
* Internal pull-ups for clean wiring
* Optional rotary encoder (V2)
* Simple, compact firmware

---

## Hardware Requirements

* Arduino **Leonardo / Micro / Pro Micro**
  (required for native USB HID)
* Momentary push buttons
* Rotary encoder (only for V2)

Pins and button mappings are defined inside each sketch.

---

## Software

Both sketches use the **Joystick** library by Matthew Heironimus.
Install it via the Arduino Library Manager:

```
Tools → Manage Libraries → “Joystick” → Install
```

Upload the desired version to your Arduino, connect the buttons/encoder, and map the inputs in your sim racing game.
