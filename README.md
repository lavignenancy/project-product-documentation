**# project-product-documentation

Centralized, version-controlled repository containing the complete technical blueprint for the Restoration-on-Demand (RoD) platform.

## Core Architecture Flow
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

## Platform Stakeholders

### 1. Players (High Power, High Interest)
* **Institutional Supervisors**: Coordinate large-scale field efforts via the Supervision Dashboard and audit AI outputs to justify funding.

### 2. Context Setters (High Power, Low Interest)
* **Agricultural Bodies**: Provide scientific data for the AI engine and enforce regulatory compliance.
* **National Registries**: Set technical interoperability standards necessary to attract investment.

### 3. Subjects (Low Power, High Interest)
* **Smallholder Farmers**: Primary users whose livelihoods depend on soil health, crop yields, and USSD tools.
* **Field Experts**: Operational staff focused on offline PWA data logging and field execution.

### 4. Crowd (Low Power, Low Interest)
* **Commercial Fertilizer Blenders**: Secondary audience for monetization via aggregated soil health data.


## Repository Structure & Additional Documentation
* **[`README.md`](README.md)**: Main architecture overview, stakeholder structures, and system diagrams.
* **`DATA_LOGIC.md`**: Complete agronomic AI engine rules, 4-digit mutual handshake logic, GPS geofencing parameters, and soil health thresholds (pH, N, P) with red-flag alerts.
* **`TECHNICAL_SPEC.md`**: Guidelines for local background caching on the PWA, location territory routing for county networks, and data schema metrics.
**
