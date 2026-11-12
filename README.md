# 🔎 Digital Crime Scene Reconstruction Engine (DCSRE)

### አሻራ (ASHARA) — Digital Forensics & Incident Response Platform

---

## 📌 1. Project Information

| Information          | Details                                                                     |
| -------------------- | --------------------------------------------------------------------------- |
| **Project Title**    | Digital Crime Scene Reconstruction Engine (DCSRE)                           |
| **Project Codename** | አሻራ (Ashara)                                                                |
| **Project Domain**   | Digital Forensics and Incident Response (DFIR)                              |
| **Student Name**     | (dhulkifl seid)Zulkifl Seid                                                                |
| **Student ID**       | 1083-26                                                                     |
| **Project Type**     | Cybersecurity / Digital Forensics                                           |
| **Live Application** | [Visit DCSRE](https://digital-crime-scene-reconstruction-three.vercel.app/) |

## 📖 2. Project Overview

The **Digital Crime Scene Reconstruction Engine (DCSRE)**, codenamed **አሻራ (Ashara)**, is a Digital Forensics and Incident Response (DFIR) platform designed to collect, analyze, correlate, and reconstruct digital evidence associated with cybersecurity incidents.

Modern cyberattacks generate enormous volumes of fragmented digital evidence across operating systems, networks, applications, and security infrastructure. Investigators frequently need to examine Windows Event Logs, Linux authentication logs, network packet captures, and web server logs to understand what happened during an incident.

Manually correlating these different sources is time-consuming, complex, and potentially prone to investigative errors.

DCSRE addresses these challenges by transforming heterogeneous forensic artifacts into structured events, correlating activities chronologically, identifying suspicious behavior through deterministic detection rules, and visualizing relationships between digital entities.

The platform provides investigators with a centralized workspace for examining evidence, reconstructing incident timelines, investigating attack relationships, and generating structured forensic reports.

## 🎯 3. Project Objectives

The primary objectives of Ashara are:

1. Automate the collection and analysis of heterogeneous digital forensic artifacts.
2. Preserve evidence integrity through cryptographic SHA-256 fingerprinting.
3. Normalize different log formats into a Common Event Schema (CES).
4. Reconstruct chronological incident timelines from fragmented evidence.
5. Identify suspicious activities using deterministic detection rules.
6. Map detected behaviors to the MITRE ATT&CK framework.
7. Visualize relationships between compromised systems and suspicious entities.
8. Generate structured forensic investigation reports.
9. Improve investigation efficiency, accuracy, and reproducibility.

## ⚠️ 4. Problem Statement

Modern cybersecurity incidents produce large amounts of fragmented digital evidence distributed across multiple systems and platforms.

Traditional manual forensic investigation faces several challenges:

- Fragmented evidence across heterogeneous sources.
- Time-consuming manual log correlation.
- Difficulty reconstructing accurate incident timelines.
- Limited visibility into relationships between compromised entities.
- Inconsistent investigative conclusions.
- Challenges maintaining evidence provenance and chain of custody.
- Difficulty producing structured and reproducible forensic reports.

**Ashara** addresses these problems by providing a centralized forensic investigation platform that transforms raw digital artifacts into structured, traceable, and evidence-supported incident reconstructions.

## 🚀 5. Key Features

| Feature                           | Description                                                                                         |
| --------------------------------- | --------------------------------------------------------------------------------------------------- |
| 🔒 Cryptographic Evidence Custody | Computes SHA-256 fingerprints when evidence is ingested to support evidence integrity verification. |
| ⚡ Multi-Format Forensic Ingestion | Supports Windows EVTX, Linux logs, PCAP, web server logs, CSV, and JSON.                            |
| 🌐 Common Event Schema            | Normalizes different event formats into a unified structure.                                        |
| 🎯 Deterministic Threat Detection | Uses Sigma-style rule matching to identify suspicious activities.                                   |
| ⏱️ Unified Chronological Timeline | Correlates events from different evidence sources into a unified timeline.                          |
| 🕸️ Interactive Attack Graph      | Visualizes relationships between hosts, IP addresses, processes, and suspicious entities.           |
| 📄 Forensic Report Generation     | Generates structured reports containing findings, timelines, and indicators of compromise.          |
| 🛡️ Role-Based Access Control     | Separates investigator and administrator permissions.                                               |

## 🏛️ 6. System Architecture and Processing Pipeline

DCSRE uses an eight-stage evidence-processing pipeline.

```text
┌──────────────────────────────────────────────────────────────┐
│                  EVIDENTIARY ARTIFACTS                        │
│                                                              │
│  Windows EVTX | Linux Logs | PCAP | Nginx | Apache | CSV     │
└──────────────────────────────┬───────────────────────────────┘
                               │
                               ▼
┌──────────────────────────────────────────────────────────────┐
│ STAGE 1: Evidence Ingestion & SHA-256 Fingerprinting          │
├──────────────────────────────────────────────────────────────┤
│ STAGE 2: Multi-Format Parsing & Event Normalization           │
├──────────────────────────────────────────────────────────────┤
│ STAGE 3: Chronological Timeline Reconstruction                │
├──────────────────────────────────────────────────────────────┤
│ STAGE 4: Sigma Rule Field Matching                            │
├──────────────────────────────────────────────────────────────┤
│ STAGE 5: Deterministic Detection & MITRE ATT&CK Mapping       │
├──────────────────────────────────────────────────────────────┤
│ STAGE 6: Entity Role Classification                           │
├──────────────────────────────────────────────────────────────┤
│ STAGE 7: Attack Graph Reconstruction                          │
├──────────────────────────────────────────────────────────────┤
│ STAGE 8: Forensic Report Generation & SHA-256 Verification    │
└──────────────────────────────┬───────────────────────────────┘
                               │
                               ▼
┌──────────────────────────────────────────────────────────────┐
│                 INVESTIGATOR WORKSPACE                        │
│                                                              │
│   Timeline | Attack Graph | Forensic Reports | Audit Logs     │
└──────────────────────────────────────────────────────────────┘
```

### 6.1 Pipeline Explanation

1. **Evidence Ingestion:** Accepts digital forensic artifacts and calculates SHA-256 fingerprints.
2. **Parsing and Normalization:** Extracts relevant information and converts events into the Common Event Schema.
3. **Timeline Reconstruction:** Orders events using normalized timestamps while accounting for timestamp differences and uncertainties.
4. **Sigma Rule Matching:** Compares normalized event fields against configured detection rules.
5. **Threat Detection:** Identifies suspicious activities and maps applicable findings to MITRE ATT&CK techniques.
6. **Entity Classification:** Classifies relevant entities, including hosts, users, IP addresses, and processes.
7. **Attack Graph Reconstruction:** Visualizes relationships and event-supported connections between entities.
8. **Report Generation:** Produces structured investigation reports with evidence references and integrity verification information.

## 📸 7. Screenshots and Demonstration

### 7.1 Live Deployed Application

🌐 **Live Website:** [Open Digital Crime Scene Reconstruction Engine](https://digital-crime-scene-reconstruction-three.vercel.app/)

### 7.2 Public Portal and 3D Global Cyber Threat Sphere

The landing page provides an introduction to the platform, incident metrics, and an interactive global cyber threat visualization.

\<p align="center">
&#x20; \<img src="[https://github.com/saremworkuu/Digital-Crime-Scene-Reconstruction-Engine/raw/main/landing_page.png](https://github.com/saremworkuu/Digital-Crime-Scene-Reconstruction-Engine/raw/main/landing_page.png)" alt="DCSRE Public Portal and 3D Threat Sphere" width="100%">
\</p>

### 7.3 Forensic Investigator Dashboard

The investigator dashboard provides a centralized workspace for monitoring investigations, reviewing case information, and accessing forensic analysis features.

### 7.4 Project Demonstration Video

The following video demonstrates the functionality and workflow of the Digital Crime Scene Reconstruction Engine.

🎥 **Watch the Project Demonstration:**

[▶ View DCSRE System Demonstration](assets/dcsre-demo.mp4)

> Replace the video link above with your actual video file or hosted video URL after uploading it to GitHub.

## 🗄️ 8. Supported Forensic Artifact Formats

| Artifact Category  | Supported Formats              | Forensic Information                                                      |
| ------------------ | ------------------------------ | ------------------------------------------------------------------------- |
| Windows Event Logs | `.evtx`, `.xml`                | Logon events, process creation, service installation, PowerShell activity |
| Network Captures   | `.pcap`, `.pcapng`             | TCP/UDP flows, DNS queries, HTTP activity, network communication          |
| Linux System Logs  | `auth.log`, `syslog`, `secure` | SSH authentication, sudo activity, user creation, PAM sessions            |
| Linux Audit Logs   | `audit.log`, `auditd`          | System calls, file permission changes, security-related activities        |
| Web Server Logs    | Apache, Nginx access logs      | HTTP requests, suspicious requests, scanner activity                      |
| Generic Data       | `.csv`, `.json`, `.txt`        | Custom SIEM exports and structured investigation data                     |

## ⚖️ 9. Forensic Integrity and Evidence Management

Evidence integrity and traceability are essential components of digital forensic investigations.

DCSRE incorporates the following mechanisms:

**1. Cryptographic Fingerprinting**

SHA-256 hashes are calculated for ingested evidence files to support verification that the evidence has not changed.

**2. Evidence Provenance**

Evidence records are associated with investigation information and available source metadata to support traceability.

**3. Deterministic Detection**

Detection results are based on configured rules and identifiable event records rather than unsupported conclusions.

**4. Role-Based Access Control**

Access permissions distinguish between system administrators and forensic investigators.

**5. Report Integrity Verification**

Generated reports can include content-derived SHA-256 fingerprints to help verify report integrity.

> Note: SHA-256 fingerprinting and audit records support evidence integrity and chain-of-custody documentation. Legal admissibility depends on the applicable jurisdiction, collection procedures, preservation controls, documentation, and validation of the complete forensic process.

## 🛠️ 10. Technology Stack

| Component                     | Technology          |
| ----------------------------- | ------------------- |
| Backend                       | Python 3.11+        |
| API Framework                 | FastAPI             |
| Frontend                      | React               |
| Frontend Build Tool           | Vite                |
| Styling                       | Tailwind CSS        |
| Database                      | PostgreSQL / SQLite |
| Evidence Integrity            | SHA-256             |
| Detection                     | Sigma-style rules   |
| Threat Intelligence Framework | MITRE ATT&CK        |
| API Documentation             | Swagger / OpenAPI   |

## 🚀 11. Installation and Quick Start

### 11.1 Prerequisites

Make sure the following software is installed:

- Python 3.11 or higher
- Node.js 18 or higher
- npm
- PostgreSQL (recommended for production)
- Git

### 11.2 Clone the Repository

```bash
git clone https://github.com/saremworkuu/Digital-Crime-Scene-Reconstruction-Engine.git

cd Digital-Crime-Scene-Reconstruction-Engine
```

### 11.3 Backend Installation

Navigate to the backend directory:

```bash
cd backend
```

Create a Python virtual environment:

```bash
python -m venv venv
```

Activate the environment.

**Linux/macOS:**

```bash
source venv/bin/activate
```

**Windows:**

```powershell
.\venv\Scripts\activate
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

Configure environment variables:

```bash
cp .env.example .env
```

Edit `.env` with your local database and application configuration.

Start the FastAPI backend:

```bash
uvicorn app.main:app --reload --host 0.0.0.0 --port 8000
```

Backend API documentation:

[http://localhost:8000/docs](http://localhost:8000/docs)

### 11.4 Frontend Installation

Open another terminal and navigate to the frontend directory:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

Open the local URL printed by Vite in your terminal. Depending on the configuration, it may be:

- [http://localhost:3000](http://localhost:3000)
- [http://localhost:3001](http://localhost:3001)
- [http://localhost:5173](http://localhost:5173)

## 🔐 12. Security Considerations

The platform is designed with the following security considerations:

- SHA-256 evidence fingerprinting.
- Role-based access control.
- Authentication and authorization.
- Evidence provenance and auditability.
- Controlled access to investigation records.
- Secure configuration through environment variables.
- Separation of evidence processing and presentation.

**Important:** Configure your own administrator credentials for local testing. Never publish default passwords, API keys, database credentials, or other secrets in the public repository.

## 🔮 13. Future Enhancements

Potential future development directions include:

1. Integration with advanced memory forensic frameworks.
2. Expanded digital disk image analysis.
3. Additional threat intelligence integrations.
4. Advanced evidence relationship visualization.
5. Automated forensic case management.
6. Enhanced investigation collaboration.
7. Extended detection rule libraries.
8. Multilingual investigation reports.
9. Advanced forensic analytics and reporting.

## 🎓 14. Academic Project Information

This project was developed as an academic cybersecurity project with the objective of exploring the application of digital forensics, incident response, cryptographic integrity verification, event correlation, and threat visualization.

**Student:** Zulkifl Seid
**Student ID:** 1083-26
**Project:** Digital Crime Scene Reconstruction Engine (DCSRE)
**Codename:** አሻራ (Ashara)

---

\<p align="center">
&#x20; \<strong>አሻራ (ASHARA)\</strong>\<br>
&#x20; Reconstructing Digital Evidence. Revealing the Attack. Preserving the Truth.
\</p>
