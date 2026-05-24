
## PCB Specifications

| Parameter | Specification |
|-----------|---------------|
| Microcontroller 1 | ATmega328P (DIP-28 or SMD) |
| Microcontroller 2 | ESP8266 (ESP-12E/F module) |
| Input Voltage | 12-24V DC (industrial standard) |
| Regulated Output | 5V @ 2A, 3.3V @ 800mA |
| Digital Inputs | 6x opto-isolated (24V) |
| Digital Outputs | 4x relay outputs (10A 250VAC) |
| Analog Inputs | 4x (0-5V / 4-20mA selectable) |
| Communication | UART, Modbus RS-485 (optional) |
| PCB Layers | 2-layer |
| PCB Size | 100mm x 80mm |

## Key Components

| Component | Part Number | Function |
|-----------|-------------|----------|
| ATmega328P | ATMEGA328P-PU | Main sensor processor |
| ESP8266 | ESP-12E | WiFi and web server |
| Voltage Regulator | LM2596 | 12V to 5V conversion |
| LDO | AMS1117-3.3 | 5V to 3.3V for ESP |
| Optocoupler | PC817 | Input isolation |
| Relay | SRD-05VDC-SL-C | Output switching |
| RS-485 Transceiver | MAX485 | Modbus communication |

## File Descriptions

| File | Description |
|------|-------------|
| `schematic.pdf` | Complete circuit schematic |
| `pcb_layout.pdf` | PCB layout (top and bottom layers) |
| `gerber_files.zip` | Manufacturing files for PCB fabrication |
| `BOM.csv` | Bill of Materials with part numbers |
| `pcb_render.png` | 3D render of the PCB |

## How to View/Edit

### View Schematics/PCB
1. Download the PDF files
2. Open with any PDF viewer

### Edit (requires EDA software)
- **KiCad** (free, open-source)
- **Altium Designer**
- **EAGLE** (Autodesk)
- **Proteus**

### Order PCBs
1. Download `gerber_files.zip`
2. Upload to PCB manufacturer (JLCPCB, PCBWay, Seeed Studio)
3. Use `BOM.csv` for component procurement

## Production Notes

- 500+ units manufactured and deployed
- Designed for industrial environment (noise immunity, isolation)
- Wide operating temperature range: -20°C to +70°C
- Overvoltage and reverse polarity protection on power input

## Version History

| Version | Date | Changes |
|---------|------|---------|
| v1.0 | 2023 | Initial production release – 500+ units |
| v2.0 | 2024 | Added ESD protection, improved grounding, optional RS-485 |

## Related Repositories

- [ESP8266 Firmware](https://github.com/ayoubgethub2024/embedded-industrial-automation)
- [ATmega328 Firmware](https://github.com/ayoubgethub2024/embedded-industrial-automation/tree/main/atmega328-firmware)
- [PLC Programs](https://github.com/ayoubgethub2024/PLC-industrial-automation)

## Author

Embedded Systems & Industrial Automation Engineer
