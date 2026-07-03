# project-product-documentation

Centralized, version-controlled repository containing the complete technical blueprint for the Restoration-on-Demand (RoD) platform.

## 🗺️ Core Architecture Flow
```text
  [Farmer: Feature Phone] 
             │  (USSD Service Request)
             ▼
 [Field Expert: Offline PWA] 
             │  (On-site Handshake + IoT Log)
             ▼
[PWA Background Sync] ───┴───► [Cloud AI Engine]
                                     │
                ┌────────────────────┴────────────────────┐
                ▼                                         ▼
[Farmer: SMS Digital Prescription]       [Supervisor: Dashboard Hub]
```

## 👥 Stakeholder Matrix
1. **Players (Institutional Supervisors)**: Manage dashboards, audit AI outputs, and justify capital distribution.
2. **Context Setters (Agricultural Bodies & National Registries)**: Set regulatory standards and scientific AI logic thresholds.
3. **Subjects (Smallholder Farmers & Field Experts)**: End-users executing restoration tasks and utilizing the offline-first tools.
4. **Crowd (Commercial Fertilizer Blenders)**: Monetization opportunities via aggregated soil trend insights.

## 📁 Repository Structure & Additional Documentation
* **[`README.md`](README.md)**: Main architecture overview, stakeholder structures, and system diagrams (This file).
* **`DATA_LOGIC.md`**: Complete agronomic AI engine rules, 4-digit mutual handshake logic, GPS geofencing parameters, and soil health thresholds (pH, N, P) with red-flag alerts.
* **`TECHNICAL_SPEC.md`**: Guidelines for local background caching on the PWA, location territory routing for county networks, and data schema metrics.
