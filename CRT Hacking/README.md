# CRT Audio Reactive Hack

This project explores analog modifications of a Cathode Ray Tube (CRT) display to enable manual and experimental control over image deformation and color channels.

## Safety Warning

CRT displays operate at high voltages (several kilovolts) and can retain charge even when powered off.

- Risk of electric shock
- Dangerous stored energy
- Only attempt if properly trained

Always discharge the CRT before handling.

---

## Project Goals

- Control RGB channels manually
- Modify vertical image scaling
- Experiment with audio-reactive image deformation (prototype)

---

## Hardware Modifications

### RGB Channel Control

For each RGB channel:

- Replace the original resistor (e.g. R903 for Red) with:
  - a 10kΩ potentiometer
  - a 1kΩ resistor in parallel

Purpose:
- Enable adjustable intensity
- Prevent unsafe low resistance values

---

### Vertical Compression

- Replace resistor R350 with a 10kΩ potentiometer

Effect:
- Adjust vertical deflection amplitude
- Compress or stretch the image vertically

---

## Audio Reactive System (Experimental)

A prototype circuit was designed:

1. Audio input
2. Low-pass filter
3. Amplification stage
4. Comparator
5. Injection into horizontal deflection

Result:
- Non-functional
- Unstable behavior

See `/schematics/` for details.

---

## Results

(Add images here)

---

## Documentation

- docs/theory.md
- docs/modifications.md
- docs/troubleshooting.md

---

## Limitations

- Audio system not working
- Behavior depends on CRT model
- Requires manual tuning

---

## License

Open-source hardware / documentation