# Full plan and architecture of the IoT + Homelab project repository on github
---


iot-homelab-rocnikovka/
├── .github/
│   └── workflows/
│       └── deploy.yml              # CI/CD pipeline pre automatické nasadenie
├── docker/
│   ├── docker-compose.yml          # Hlavná definícia služieb (HA, Mosquitto, InfluxDB, Grafana)
│   ├── mosquitto/
│   │   └── config/
│   │       └── mosquitto.conf      # Konfigurácia MQTT brokera
│   ├── nodered/
│   │   └── data/                   # Exportované automatizačné toky (flows)
│   └── grafana/
│       └── provisioning/           # Automatické načítanie dashboardov a dátových zdrojov
├── firmware/
│   ├── esp32-sensors/              # C++ / PlatformIO kód pre meranie teploty/vlhkosti
│   │   ├── src/
│   │   │   └── main.cpp
│   │   └── platformio.ini
│   └── esp8266-relays/             # Kód pre spínacie relé moduly
├── docs/
│   ├── hardware-inventory.md       # Evidencia zakúpeného HW, objednávok a cien
│   ├── architecture.md             # Topológia siete, VLANy, IP adresy a porty
│   └── rocnikova-praca.md          # Hlavný textový obsah ročníkovej práce
├── structure-of-repo/
│   └── repo-plan.md                # Tento dokument (Master Plan)
├── scripts/
│   ├── install.sh                  # Automatizačný skript pre prípravu Linux servera (Fedora)
│   └── backup.sh                   # Zálohovanie databáz a konfiguračných súborov
├── .env.example                    # Šablóna pre heslá, prístupové tokeny a premenné prostredia
├── .gitignore                      # Ignorovanie senzitívnych dát (.env) a dátových priečinkov
└── README.md                       # Hlavný prehľad projektu a návod na spustenie
