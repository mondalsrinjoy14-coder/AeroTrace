# AeroTrace ✈️

A software prototype for investigating potential GNSS spoofing and jamming through aircraft ADS-B data analysis.

## Overview

AeroTrace examines suspicious aircraft movement and patterns affecting multiple aircraft to help analysts investigate possible navigation interference.

It highlights anomalies and supporting evidence. Alerts indicate potential issues and do not confirm spoofing or jamming.

## Features

- Interactive aircraft tracking dashboard.
- CSV import, preview, and flight replay.
- Physics-based checks for unusual aircraft movement.
- Multi-aircraft correlation and spatial clustering.
- Investigation views with supporting evidence.
- Alert rules and notification integrations.
- Optional machine-learning components requiring separate setup and suitable model artifacts.

## Technology

- **Frontend:** TypeScript, React, TanStack Start, Tailwind CSS
- **Backend:** Python, FastAPI
- **Storage:** SQLite
- **Data:** ADS-B provider integrations and imported CSV datasets

## Repository Structure

The application source is inside `Aerotrace-main/`.

- `src/` — frontend components and dashboard
- `backend/` — API, ingestion, detection, and storage
- `backend/tests/` — backend tests

See the [application README](Aerotrace-main/README.md) for setup information.

## Demo Workflow

1. Open the dashboard.
2. Import a compatible aircraft CSV dataset.
3. Preview the data and start tracking or replay.
4. Inspect suspicious movements and generated alerts.
5. Review the evidence associated with each event.

Use clearly labelled simulated datasets when demonstrating the system.

## Security and Limitations

- Store API credentials in backend environment variables.
- Never commit real credentials or expose them through frontend variables.
- The backend currently requires authentication and additional security hardening before public production use.
- ADS-B anomalies can also result from data errors or coverage gaps.
- This is a research and demonstration prototype, not a certified aviation safety or navigation system.

## Credits

Developed collaboratively for the AeroTrace project.
Based on the team's earlier SpoofSky work.
