# IoT Homelab & Smart Home Infrastructure

Welcome to the official repository for my school coursework project focused on designing, building, and configuring a local IoT server, home automation stack, and managed network infrastructure. (Ročníková práca pre tretí ročník, SPSJM)

### Key Highlights
- **Network Segmentation:** IoT traffic isolated with VLANs on a TP-Link ER605 router and TL-SG108E switch.
- **Server:** HP EliteDesk 800 G3 Desktop Mini (i5-7500T, 32 GB RAM) mounted in a 3D-printed 10" Lab Rax rack.
- **Storage:** Samsung 870 EVO 931 GB in an AXAGON dual 2.5" dock, with a second 1 TB SSD planned for RAID 1 mirroring.
- **Core Services:** Home Assistant, Mosquitto MQTT broker, Nextcloud, and a Telegram bot connected to the Gemini API. InfluxDB and Grafana are planned.

## 📚 Documentation & Navigation

**[Project Overview & Summary](docs/project-overview.md)** – Motivation, system goals, and architecture plans.
**[Hardware Inventory & Plans](docs/hardware-inventory.md)** – Ordered hardware, specs, and future expansion.
**[Budget & Expense Tracker](docs/budget.md)** – Financial tracking and component price lists.
**[Progress Log](docs/progress-log.md)** – Timeline and activity log.
**[Repository Master Plan](structure-of-repo/repo-plan.md)** – Target directory layout and long-term structure.

## HARDWARE

**Network (Lab Rax rack)**
- Router: TP-Link ER605
- Switch: TP-Link TL-SG108E
- Cat6 patch cables, 0.25 m
- Existing TP-Link Archer VR300 (AP mode, outside the rack)
- Powerline adapter kit (WiFi extension to the garage)

**Server (Lab Rax rack)**
- HP EliteDesk 800 G3 DM: i5-7500T, 32 GB DDR4, 256 GB NVMe (OS)
- Samsung 870 EVO 931 GB (existing, data disk)
- AXAGON ADSA-D25 dual 2.5" dock
- ADATA SU650 1 TB (planned, mirror disk)
- Rebel NanoPower 650VA UPS (beside the rack)

**IoT**
- ESP32 boards x6
- Reed sensors x3 (garage door, gate, entrance door)
- PIR motion sensor (garage)
- BME280/DHT22 sensors x4 (rooms)
- MQ-2 smoke module (house)
- Dupont wires, resistors, USB cables and power adapters, M3 screws, small power strip

## SOFTWARE
- Home Assistant
- Mosquitto (MQTT broker)
- Nextcloud (NAS/cloud)
- Telegram bot (Python) with Gemini API
- InfluxDB and Grafana (planned)

Router and switch are managed through the ER605's own web interface. No Omada Controller is used.

*Developed on Fedora Linux using VS Code, C# / PlatformIO, and Git/GitHub.*
