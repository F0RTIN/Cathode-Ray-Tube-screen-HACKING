# Theory of Operation

## CRT Fundamentals

A Cathode Ray Tube (CRT) operates by emitting an electron beam from an electron gun toward a phosphor-coated screen.

The beam is controlled by:
- Horizontal deflection coils
- Vertical deflection coils
- Intensity modulation via RGB signals

The image is generated through raster scanning:
- Horizontal sweep (fast)
- Vertical sweep (slow)

---

## RGB Signal Control

The RGB signals control the intensity of the electron beam.

By modifying resistance in these paths:
- Current changes
- Beam intensity changes
- Resulting brightness is altered

Adding a potentiometer allows dynamic control, while a parallel resistor ensures a minimum current threshold.

---

## Vertical Deflection

The vertical deflection circuit controls the amplitude of the vertical scan.

Reducing resistance:
increases current  
increases deflection amplitude  

Increasing resistance:
reduces current  
compresses the image vertically  

---

## Audio Reactive Concept

The goal was to convert an audio signal into a spatial modulation.

Signal chain:

Audio → Filter → Amplifier → Comparator → Deflection input

Expected behavior:
- Audio amplitude mapped to horizontal deformation

---

## Why It Likely Failed

Several technical challenges:

### Signal Scaling
Audio signals are low voltage (around 1V peak)
insufficient for deflection circuits

### Bandwidth mismatch
CRT deflection operates at high frequencies
audio is not synchronized with scan timing

### Injection point
Deflection circuits are sensitive and non-linear

### Comparator behavior
Threshold switching creates discontinuities and noise

---

## Possible Improvements

- Use envelope detection instead of raw audio
- Add proper gain staging
- Use a controlled injection point
- Consider analog modulation instead of hard thresholding