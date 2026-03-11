# Tero.Ops

**Enterprise Asset Management for maritime and industrial operations — from vessel to shore, online or offline.**

Tero.Ops is purpose-built for fishing fleets, aquaculture operations, and industrial facilities. It replaces spreadsheets and paper logs with a single platform that works at sea and on shore, giving fleet operators real-time visibility into asset health, maintenance schedules, spare parts inventory, and regulatory compliance.

## What Tero.Ops Does

### Asset & Fleet Management
Hierarchical tracking of vessels, equipment, and sub-components. Every asset has a full maintenance history, associated spare parts, QR code for field scanning, and links to scheduled jobs. Supports unlimited nesting (vessel → engine → pump → seal) for accurate equipment modeling.

### Preventive Maintenance
Schedule maintenance jobs based on calendar intervals, meter readings (engine hours, fuel consumption), or whichever comes first. When a job is completed, the next occurrence is automatically created. No more missed oil changes because someone forgot to update a spreadsheet.

### Procurement & Inventory
End-to-end workflow: inventory request → purchase order → supplier dispatch → partial receipt. Tracks stock levels with min/max/reorder thresholds. Supports partial deliveries across different ports — critical when fishing vessels pick up parts at multiple stops.

### Project Coordination
Group related work requests into projects for drydocks, overhauls, or equipment upgrades. Track each request through 8 workflow states with contractor assignment, priority management, and full documentation.

### Digital Inspections
Structured inspection checklists on phones and tablets. Photo attachment with auto-timestamping and geolocation. Deficiencies automatically create follow-up tasks. Inspection records are audit-ready for port state control and classification societies.

### Compliance & Reporting
Auto-generated ISM Code compliance reports. Gap analysis flags missing documents and expired certificates. Full audit trail for Samgöngustofa (Icelandic Maritime Administration) and IMO standards. One-click report generation from aggregated vessel data.

### Meter & Consumption Tracking
Track fuel consumption, engine hours, water usage, and other measurable resources. Meter readings — manual or from IoT sensors — trigger maintenance jobs when thresholds are crossed.

## Key Design Principles

**Offline-first.** Works completely offline on iOS, Android, and web. Data is encrypted on-device and syncs automatically when connectivity returns. Designed for vessels at sea with intermittent or no internet.

**Maritime-native.** Not a generic CMMS adapted for ships. Fleet hierarchy, multi-port procurement, vessel inspections, and ISM Code compliance are built in — not bolted on.

**Mobile-first.** QR code scanning, photo capture, and touch-optimized interfaces designed for use on deck, in engine rooms, and on processing floors.

**Bilingual.** Full platform support in English and Icelandic with native maritime terminology in both languages.

**Role-based.** Fine-grained permissions scoped to company, fleet, and worksite level. Crew sees their vessel. Fleet managers see the fleet. Contractors see their assigned work.

## Who Uses Tero.Ops

| Role | What They Get |
|------|---------------|
| **Fleet Manager** | Real-time maintenance status across all vessels, automated scheduling, fleet-wide dashboards |
| **Technical Manager** | Spare parts tracking, work order management, drydock project coordination |
| **Compliance Officer** | One-click ISM Code reports, gap analysis, audit-ready inspection records |
| **Procurement Officer** | Request-to-receipt workflow, partial delivery support, vendor management |
| **Crew / Field Technician** | Mobile maintenance recording, QR scanning, offline inspections |
| **CEO / Shipowner** | Fleet health overview, compliance status, procurement cost visibility |

## Tech Stack

- **Frontend:** React, TypeScript, Ionic, Vite
- **Mobile:** Capacitor (iOS, Android, Desktop)
- **Data Grid:** AG Grid with server-side pagination
- **Auth:** Passwordless magic links, JWT, optional 2FA
- **API:** RESTful with JWT authentication

## About Tero

Tero ehf. is an Icelandic technology company building operational software for the fishing and aquaculture industry. Tero.Ops is the company's flagship product, used by fleet operators to manage vessel maintenance, equipment, inventory, and regulatory compliance.

**Website:** [tero.is](https://tero.is)
