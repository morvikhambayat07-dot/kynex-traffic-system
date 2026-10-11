# 🚦 KYNEX 2.0 — Smart Traffic Management & Autonomous Command System

An ultra-modern, production-grade Traffic Operations Command Deck featuring smooth 60 FPS Intelligent Driver physics, full Three.js 3D simulation, interactive Google Maps with multi-map junction creation, and persistent IndexedDB database storage.

---

## ⚡ Quick Start

### Option 1: Direct Browser Launch (Zero Installation Required)
Simply double-click `index.html` or open it directly in any modern browser (Chrome, Edge, Firefox, Brave):
```
C:\Users\ADMIN\.gemini\antigravity\scratch\kynex-traffic-system\index.html
```

### Option 2: Local HTTP Server (PowerShell)
Open PowerShell in this directory and execute:
```powershell
.\server.ps1
```
This automatically hosts the application at `http://localhost:8080` and opens it in your default browser.

---

## 🔐 Operator Demo Access
- **Operator ID:** `OPERATOR001` (or any custom operator badge ID)
- **Security Passcode:** `admin123`

---

## 🌟 Key Upgrades & Features

### 1. Modern Cyberpunk Command Deck Design
- Deep navy/slate glassmorphic theme with glowing telemetry indicators, responsive cyber cards, and smooth micro-interactions.
- Web Audio API procedural synthesizer for audio feedback (UI clicks, violation alarms, and realistic two-tone emergency ambulance siren with mute toggle).

### 2. Smooth 60 FPS Dual-Engine Simulation (2D & 3D)
- **Intelligent Driver Physics**: Vehicles accelerate smoothly, calculate safe braking distances, and queue bumper-to-bumper at red lights without clipping, teleporting, or freezing.
- **Automated 4-Phase Cyclic Signal Controller**:
  - `Phase 1: North-South Green` → `Phase 2: North-South Amber (3s)` → `Phase 3: All-Red Safety Clearance (1.5s)` → `Phase 4: East-West Green` → `Phase 5: East-West Amber (3s)` → `Phase 6: All-Red Safety Clearance (1.5s)`.
  - Configurable sliders for each direction (10s – 90s).
  - Operating modes: **Auto Cycle**, **Adaptive AI** (balances green time based on real-time lane congestion), and **Manual Override**.
- **Full 3D Cyber Perspective (Three.js)**:
  - Instant toggle between **2D Tactical View** and **3D Cyber View**.
  - Interactive 3D OrbitControls (360° rotate, pan, zoom).
  - Quick Camera Presets: *Isometric 45°*, *Top-Down Radar*, *Street CCTV Angle*, and *Chase Angle*.
  - Realistic 3D vehicles with glowing headlights, dynamic brake lights, volumetric traffic signal gantries, and surrounding city skyline buildings.

### 3. Interactive Google Maps & Multi-Map Manager
- **Map Layers**:
  - **Google Road**: Google Maps standard street view.
  - **Google Satellite**: High-resolution satellite aerial imagery.
  - **Google Hybrid**: Satellite imagery with street names and overlays.
  - **Cyber Dark**: High-contrast dark matter theme.
- **Preconfigured Global Intersections**:
  - *Times Square Nexus* (New York, USA)
  - *Shibuya Scramble Crossing* (Tokyo, Japan)
  - *Connaught Place Outer Radial* (New Delhi, India)
  - *Silicon Valley Connected Corridor* (San Jose, USA)
- **Add Another Map / Junction Feature**:
  - Click **"ADD ANOTHER MAP / JUNCTION"** to register custom intersections anywhere in the world.
  - Input custom Name, City, Coordinates (Latitude/Longitude), Speed Limits, and Approach Lanes.
  - *Interactive Coordinate Picker*: Simply click anywhere on the map to automatically populate latitude and longitude!
  - Custom maps are permanently stored in the database and immediately appear in the active junction selector.

### 4. Emergency Green Corridor Pre-emption
- Dispatches emergency ambulance convoys with high-priority signal override.
- Conflicting signals turn Amber then Red, while the corridor locks into Green.
- Real-time cascading progress timeline, flashing siren beacons, and audible oscillating siren.

### 5. Persistent Database & E-Challan Ledger (IndexedDB)
- **Permanent Data Storage**: All violations, custom maps, operator audit logs, and revenue metrics are stored in client-side **IndexedDB** (with LocalStorage fallback) and persist across page refreshes and computer reboots.
- **E-Challan Ledger**:
  - Real-time search and filter by plate number, violation rule, or payment status.
  - Interactive ANPR Evidence Modal: Click any record to inspect simulated 4K CCTV frame with AI bounding box and vehicle OCR metadata.
  - Mark Challans as **Paid** or **Pending**.
- **Backup & Export**:
  - **Export CSV**: Download a spreadsheet of all issued challans.
  - **Backup JSON**: Download complete database backup.
  - **Restore Backup**: One-click restore or import of historical data.

---

## 📁 Project Structure
```
kynex-traffic-system/
├── index.html           # Main command deck application
├── README.md            # Comprehensive documentation
├── server.ps1           # Optional PowerShell local web server
├── css/
│   └── main.css         # Glassmorphism cyber styles & responsive layout
└── js/
    ├── app.js           # Main coordinator & UI event handling
    ├── audio.js         # Native Web Audio API procedural synthesizer
    ├── db.js            # Persistent IndexedDB engine with export/import
    ├── map-module.js    # Google Maps & Leaflet multi-map manager
    ├── rules.js         # Traffic laws database (IPC / MV Act) & ANPR snapshot generator
    ├── traffic-sim-2d.js# 60 FPS 2D Canvas simulation with Intelligent Driver physics
    └── traffic-sim-3d.js# Three.js 3D intersection simulation with OrbitControls
```
