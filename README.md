# AI-Incident-Management-
Project
# AI-Powered Incident Management Platform

An intelligent backend platform that automates IT incident ticket workflows — from intake to resolution — using OCR, AI categorization, and smart technician assignment.

## Overview

Manual ticket triage is slow and inconsistent. This platform eliminates that bottleneck by automatically reading, categorizing, prioritizing, and routing incoming incident tickets — reducing response time and distributing workload fairly across technicians.

## Features

- 📄 **OCR-based ticket ingestion** — extracts structured data from raw incident reports
- 🤖 **Automated categorization & prioritization** — classifies tickets by type and urgency without manual input
- 👷 **Smart technician assignment** — routes tickets based on workload distribution and skill match
- 📊 **Ticket analytics** — tracks volume, resolution patterns, and team performance
- 🔌 **RESTful API** — clean endpoint design for integration with external tools or frontends

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Runtime | Node.js |
| Framework | Express.js |
| Database | MongoDB |
| OCR | Tesseract / OCR library |
| Architecture | RESTful APIs, Middleware, Service Layers |

## Architecture

```
Incoming Ticket (raw/scanned)
        ↓
   OCR Processing
        ↓
  Categorization Engine
        ↓
  Priority Scoring
        ↓
  Technician Assignment
        ↓
  MongoDB Storage + Analytics
```

## Getting Started

```bash
# Clone the repository
git clone https://github.com/garrema/incident-management-platform.git
cd incident-management-platform

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env

# Start the server
npm start
```

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/tickets` | Submit a new incident ticket |
| GET | `/api/tickets` | Retrieve all tickets |
| GET | `/api/tickets/:id` | Get a specific ticket |
| PATCH | `/api/tickets/:id` | Update ticket status |
| GET | `/api/analytics` | View ticket analytics |

## Key Results

- Automated end-to-end ticket handling with zero manual categorization
- Balanced workload distribution across technician pool
- Scalable architecture supporting high ticket volume

## Author

**Monish Siddardha Garre** — [LinkedIn](https://www.linkedin.com/in/monish-siddardha-garre-73a897328/) · [GitHub](https://github.com/garrema)
