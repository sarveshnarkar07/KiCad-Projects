# KiCad Projects

A collection of electronics projects designed in [KiCad 10.0](https://www.kicad.org/).

## Projects

| # | Project | Description |
|---|---------|-------------|
| 01 | [AC-DC Converter](01%20-%20AC-DC%20Converter/) | Full-wave bridge rectifier with smoothing capacitor and LED indicator |

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

## License

This project is open source.
