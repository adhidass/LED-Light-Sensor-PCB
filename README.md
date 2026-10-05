# First KiCad Project
## Light sensor that has adjustable threshold using potentiometer, uses LED as the photodiode and LMC6482 op-amp
![Board](Docs/LED%20Light%20Sensor.png)

[Schematic (PDF)](Docs/LED%20Light%20Sensor.pdf)

## How it works
1. Sensor: Light makes the photodiode leak a tiny current.
2. Amplifier (U1A): turns that current into a voltage, centered on a 1.65 V reference.
3. Comparator (U1B): compares the sensor voltage against the potentiometer's level. The output goes high or low depending on which is larger.

Powered by 3.3 V through a 3-pin header (3.3 V, Vout, GND).

## Status
Designed in KiCad, DRC clean. Not yet fabricated or tested.

## Files
- `Hardware/`: KiCad project files
- `Docs/`: schematic PDF and board image
- `LED Light Sensor.zip`: Gerber and drill files for manufacturing

## Credit: 
A step by step tutorial by @inkedbhav on tiktok. Assisted by Claude AI (Sonnet 5.5)
