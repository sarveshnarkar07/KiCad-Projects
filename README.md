# KiCad Projects

A collection of electronics projects designed in [KiCad 10.0](https://www.kicad.org/).

## Projects

| # | Project | Description |
|---|---------|-------------|
| 01 | [AC-DC Converter](01%20-%20AC-DC%20Converter/) | Full-wave bridge rectifier with smoothing capacitor and LED indicator |
| 02 | [Transformerless Power Supply](02%20-%20Transformerless%20Power%20Supply/) | Capacitive dropper power supply with Zener regulation and 5V output |
| 03 | [Servo Motor Tester](03-%20Servo%20Motor%20Tester/) | NE555-based PWM servo tester with adjustable pulse width |

### 01 - AC-DC Converter

A classic unregulated AC-to-DC linear power supply circuit.

**Signal path:** AC Input → Bridge Rectifier (4x 1N4007) → Smoothing Cap (1000uF) → DC Output

**Bill of Materials:**

| Ref | Value | Description |
|-----|-------|-------------|
| D1-D4 | 1N4007 | Bridge rectifier diodes |
| C1 | 1000uF | Smoothing capacitor |
| R1 | 10K | Bleeder resistor |
| R2 | 2.2K | LED current limiter |
| D5 | LED | Power indicator |
| J1, J2 | Screw Terminal 2P | DC output / AC input connectors |

- **Board:** 2-layer, ~33.5mm x 17mm, all through-hole components
- **Tool:** KiCad 10.0

### 02 - Transformerless Power Supply

A capacitive dropper (transformerless) power supply with Zener voltage regulation and LM7805 5V output.

**Signal path:** AC Input → X-Cap Dropper (C4) → Bridge Rectifier (4x 1N4007) → Filter Caps → Zener Clamp → LM7805 → 5V Regulated Output

**Bill of Materials:**

| Ref | Value | Description |
|-----|-------|-------------|
| J1 | Screw Terminal 2P | AC input connector |
| C4 | 2.2uF (225k) | X-class capacitive dropper |
| R1, R2 | 20K | Discharge resistors |
| R3 | 1M | Bleeder resistor |
| D1-D4 | 1N4007 | Bridge rectifier diodes |
| C2 | 1000uF | Primary filter capacitor |
| C3 | 470uF | Secondary filter capacitor |
| D5, D6 | Zener | Voltage clamping diodes |
| R4 | 2.2K | Zener/LED current limiter |
| D7 | LED | Power indicator |
| U1 | LM7805 | 5V linear voltage regulator |
| C1 | 0.1uF | Regulator decoupling capacitor |
| J2 | Screw Terminal 2P | DC output connector |

- **Board:** 2-layer, all through-hole components
- **Designer:** Sarvesh Narkar
- **Tool:** KiCad 10.0

### 03 - Servo Motor Tester

A simple servo motor tester using the NE555 timer IC. Generates a PWM signal to test and calibrate hobby servo motors.

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

## License

This project is open source.
