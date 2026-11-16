# 3D Printed Enclosure & Mechanical Files

This folder contains the complete mechanical design files for the **Waveshare ESP32-S3-RLCD-4.2** desktop satellite stand.

---

## Files in this Directory

| File Name | Format | Description |
|---|---|---|
| **`front_rlcd_modified.stl`** | STL | Front bezel frame with display window and mounting standoffs |
| **`front_rlcd_modified.blend`** | Blender 3D | Master editable source model in Blender |
| **`back_rlcd.step`** | STEP (CAD) | Snap-fit rear cover with ventilation, speaker grilles, and header port |
| **`buttons_rlcd.step`** | STEP (CAD) | Tactile push-button extension caps (`KEY`, `PWR`, `BOOT`) |

---

## 3D Printing Recommendations

* **Material:** PETG or PLA+ recommended (PETG offers superior durability and heat resistance for indoor desktop use).
* **Layer Height:** `0.20 mm` (optimal balance between surface quality and print speed).
* **Perimeters / Walls:** `3` walls for strength.
* **Infill:** `15% - 20%` (Gyroid or Grid).
* **Supports:** 
  * `front_rlcd_modified.stl`: minimal tree supports under the overhangs.
  * `back_rlcd.step`: print flat on build plate with support for the rear connector cutout.
* **Orientation:** Print all parts with their largest flat decorative face facing the build plate (textured PEI sheet gives an attractive matte finish).

---

## Button Assembly

Looking at the rear cover from the back, the button layout corresponds to:
1. **Left:** `KEY` (GPIO18 - short press interrupts Voice Assistant, long press toggles microphone MUTE).
2. **Center:** `PWR` (Hardware power on/off).
3. **Right:** `BOOT` (GPIO0 - manual push-to-talk wake without saying the wake word).
