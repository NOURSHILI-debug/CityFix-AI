# CityFix AI 🏙️

**AI-Powered Urban Incident Reporting, Prioritization & Geospatial Management**

CityFix AI is a smart urban management solution designed to improve how cities collect, analyze, prioritize, and monitor public infrastructure incidents.

By combining geospatial analysis, artificial intelligence, and ArcGIS Online, the platform aims to transform citizen-reported incidents into actionable information for more efficient urban maintenance and decision-making.

---

## 🎯 Project Overview

Traditional urban incident management often relies on fragmented reporting processes and manual prioritization, making it difficult to identify critical issues and allocate intervention resources efficiently.

CityFix AI addresses this challenge through an integrated workflow that:

- Collects urban incident reports through a citizen-facing reporting interface.
- Analyzes submitted images using AI-based image classification.
- Evaluates incident severity and calculates priority scores.
- Performs spatial analysis to identify geographical patterns and hotspots.
- Visualizes incidents through interactive maps and dashboards.
- Supports field operations and incident status tracking.

## ✨ Key Features

### 1. Citizen Incident Reporting
- Mobile incident reporting through ArcGIS Survey123.
- Image attachments and structured incident information.
- Geolocated incident submissions.

### 2. AI-Based Image Classification
- Image classification across three incident classes.
- Transfer learning for model training.
- Prediction of incident category, severity, and confidence.

### 3. Geospatial Analysis
- Spatial association with administrative neighborhoods.
- Distance calculations to nearby schools and hospitals.
- Hotspot identification and spatial incident analysis.

### 4. Intelligent Prioritization
- Incident priority scoring based on relevant indicators.
- Integration of severity, proximity, and spatial information.
- Identification of high-priority incidents.

### 5. Interactive Visualization
- ArcGIS Web Maps for incident visualization.
- Dashboards displaying key urban indicators.
- Incident filtering and status monitoring.
- Public-facing map through ArcGIS Experience Builder.

### 6. Workflow Automation
- Automated processing of new incident reports.
- Image classification and priority score calculation.
- Updates to the ArcGIS hosted feature layer.
- Routing of the ten highest-priority incidents into an intervention tour layer.

---

## 🏗️ System Architecture

The proposed workflow connects citizen reporting, AI processing, geospatial analysis, and visualization.

```text
       CITIZEN REPORTING
              |
              v
       ArcGIS Survey123
              |
              v
       ArcGIS Online
       Hosted Feature Layer
              |
              v
       IMAGE CLASSIFICATION
       (AI Model)
              |
              v
       SPATIAL ANALYSIS
       - Neighborhood
       - Distance to schools
       - Distance to hospitals
       - Hotspots
              |
              v
       PRIORITY SCORING
              |
              v
       AUTOMATED PIPELINE
              |
        +-----+------+
        |            |
        v            v
    Web Maps      Dashboard
        |            |
        +-----+------+
              |
              v
       INCIDENT MONITORING
       & FIELD OPERATIONS
```

## 🛠️ Technology Stack

| Component | Technology |
|---|---|
| Geospatial Platform | ArcGIS Online |
| Citizen Reporting | ArcGIS Survey123 |
| Field Operations | ArcGIS Field Maps |
| Mapping | ArcGIS Web Maps |
| Dashboard | ArcGIS Dashboards |
| Public Portal | ArcGIS Experience Builder |
| Programming | Python |
| AI / Deep Learning | Image Classification, Transfer Learning |
| Model Development | Google Colab |
| Geographic Data | OpenStreetMap (OSM) |
| Version Control | Git & GitHub |

## 📂 Repository Structure

```text
CityFix-AI/
│
├── docs/                  # Project documentation
│
├── data/                  # Data samples and datasets
│
├── notebooks/             # AI model experiments and training
│
├── src/
│   ├── data/              # Data processing
│   ├── ai/                # Image classification
│   ├── gis/               # ArcGIS and spatial analysis
│   ├── prioritization/    # Incident priority scoring
│   └── pipeline/          # Automated processing workflow
│
├── scripts/               # Execution and simulation scripts
│
├── tests/                 # Unit and integration tests
│
├── requirements.txt
├── .gitignore
└── README.md
```

## 🔄 Project Workflow

The development is organized into five main phases:

| Phase | Focus |
|---|---|
| 1. Data Foundation | ArcGIS layers, data schema, reporting form and initial integration |
| 2. Module Development | AI classification, spatial analysis, scoring and visualization |
| 3. Integration | End-to-end automated processing pipeline |
| 4. Stabilization | Testing, debugging and demonstration preparation |
| 5. Final Presentation | Project demonstration and delivery |

## 👥 Team

Developed as a collaborative university project by a team of five students.

The team is organized around five areas of responsibility:

- **Data Management:** Geographic layers, incident data and spatial attributes.
- **Collection & Field Operations:** Citizen reporting and mobile field workflows.
- **Artificial Intelligence:** Image classification and model evaluation.
- **Analysis & Automation:** Priority scoring, spatial analysis and pipeline integration.
- **Project Management & Visualization:** ArcGIS maps, dashboards and coordination.

## 🚀 Project Status

The project is currently under development. Features and components described in this repository represent the intended system scope and may evolve during implementation.

## 📌 Academic Context

Developed as part of the **TER IDS** academic project.

**Project:** CityFix AI  
**Platform:** ArcGIS Online  
**Development Period:** November 16 – December 4, 2026

---

*Making urban incident management smarter, more transparent, and more efficient.*
