# Servo Motor Tester

A simple servo motor tester circuit using the NE555 timer IC. Generates a PWM signal to test and calibrate hobby servo motors.

**Signal path:** 6V DC Input → NE555 Timer → PWM Signal → Servo Output

**Bill of Materials:**

| Ref | Value | Description |
|-----|-------|-------------|
| J1 | Pin Header 2P | 6V DC power input connector |
| U1 | NE555P | Timer IC (DIP-8) |
| RV1 | 100K | Potentiometer for pulse width adjustment |
| R1 | 3M3 | Timing resistor |
| R2 | 56K | Timing resistor |
| R3 | 1K | LED current limiter |
| C1 | 22nF | Timing capacitor |
| D1 | 1N4148 | Clamping diode |
| D2 | LED | Power indicator |
| J2 | Pin Header 3P | Servo output (GND, VCC, SIG) |

- **Input:** 6V DC
- **Designer:** Sarvesh Narkar
- **Tool:** KiCad 10.0