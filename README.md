# IoT Homelab & Smart Home Infrastructure

Welcome to the official repository for my school coursework project focused on designing, building, and configuring a local IoT server, home automation stack, and managed network infrastructure.
(Rocnikova praca pre treti rocnik, SPSJM)

### Key Highlights
- **Network Segmentation:** Isolated IoT traffic using TP-Link Omada router and switch (VLANs & firewall rules).
- **Storage & Server Setup:** Raspberry Pi 5 hosted in a custom 3D-printed 10" Lab Rax rack, featuring mirrored storage via a Dual 2.5" SATA USB Dock (RAID 1 setup).
- **Core Container Services:** Home Assistant, Mosquitto MQTT broker, InfluxDB time-series database, and Grafana dashboards running via Docker.

## 📚 Documentation & Navigation

Use the quick links below to navigate through the detailed project documentation:

**[Project Overview & Summary](docs/project-overview.md)** – Detailed motivation, system goals, and architecture plans.
**[Hardware Inventory & Plans](docs/hardware-inventory.md)** – Complete breakdown of ordered hardware, specs, and future expansion plans.
**[Budget & Expense Tracker](docs/budget.md)** – Financial tracking and component price lists.
**[Progress Log](docs/progress-log.md)** – Step-by-step timeline and activity logs.
**[Repository Master Plan](structure-of-repo/repo-plan.md)** – Target directory layout and long-term project structure.

HARDWARE
- Router: TP-Link ER605 (Omada)
- Switch: TP-Link TL-SG108E
- Rack: Lab Rax 10" (3D printed)
- Raspberry Pi 5 8GB
- Raspberry Pi 5 Active Cooler
- Raspberry Pi 27W USB-C power supply
- UPS: Rebel NanoPower 650VA
- USB dock: AXAGON ADSA-D25 (dual 2.5" SATA)
- Disk 1: Samsung 870 EVO 931GB (existing)
- Disk 2 (later): ADATA SU650 1TB (mirror)
- ESP32 boards x6
- PIR motion sensor (garage)
- Reed sensors x3 (garage, gate, entrance)
- DHT22/BME280 sensors x4 (rooms)
- MQ-2 smoke module (house)
- Powerline adapters (WiFi extension to garage)
- Existing TP-Link Archer VR300 (switched to AP mode)

SOFTWARE
- Home Assistant
- Mosquitto (MQTT broker)
- Nextcloud (NAS/cloud)
- Omada Controller (router/switch management)
- Telegram bot (Python)
- Gemini API (AI)
- Open WebUI (optional, AI frontend)

*Developed on Fedora Linux using VS Code, C# / PlatformIO, and Git/GitHub.*
