🏙️ NagarMithra — AI Citizen Infrastructure Alignment Platform

NagarMithra is an open-source, multilingual AI platform designed to connect citizen infrastructure needs with public infrastructure planning and investment.

The platform collects citizen complaints and petitions through text, voice, and multiple communication channels, analyzes them using AI and geospatial techniques, identifies infrastructure demand hotspots, and provides decision-support tools for public-sector planning.

NagarMithra currently focuses on infrastructure sectors such as:

💧 Water & Sanitation

🛣️ Roads & Mobility

⚡ Clean Energy

🏥 Healthcare

🌐 Digital Public Infrastructure

🎓 Education

🌱 Flood & Climate Resilience

The project is designed with Digital Public Good (DPG) principles, including open standards, interoperability, multilingual accessibility, privacy protection, and transparent decision-support mechanisms.

🌍 Key Features
🗣️ Multilingual Citizen Platform

Accepts citizen complaints through text and voice.

Supports multiple Indian and BRICS-region languages.

Performs language detection, translation, classification, and urgency analysis.

Supports citizen petitions and community upvoting.

🗺️ GIS & Infrastructure Hotspot Analysis

Uses geographic data to identify areas with concentrated infrastructure demands.

Uses DBSCAN clustering for spatial hotspot detection.

Provides interactive maps and district-level information.

🤖 AI Project Prioritization

Uses Multi-Criteria Decision Analysis (MCDA) to evaluate infrastructure projects.

Considers demand, infrastructure deficit, vulnerability, and feasibility.

Provides estimated beneficiaries, project timelines, costs, and SDG alignment.

💰 Public Spending Analysis

Compares citizen demand and infrastructure deficits with planned capital spending.

Identifies areas where demand and planned investment may not be aligned.

📊 Policy Simulation

Allows users to experiment with infrastructure budget allocations.

Estimates changes in infrastructure deficits and selected socioeconomic indicators.

🧠 AI Policy Copilot

Generates structured policy briefs and procurement drafts.

Connects recommendations to underlying citizen and demographic data.

🔗 Open Data & Interoperability

Provides machine-readable exports such as:

GeoJSON

CSV

JSON-LD

Provides OpenAPI documentation for integration with other systems.

📁 Project Structure
NagarMithra/
│
├── backend/
│   ├── app/
│   │   ├── api/
│   │   │   └── endpoints.py
│   │   ├── models/
│   │   │   └── schemas.py
│   │   ├── services/
│   │   │   ├── multilingual_nlp.py
│   │   │   ├── voice_processor.py
│   │   │   ├── data_store.py
│   │   │   ├── hotspot_engine.py
│   │   │   ├── recommendation_engine.py
│   │   │   ├── misalignment_engine.py
│   │   │   ├── policy_simulator.py
│   │   │   └── ai_copilot.py
│   │   └── main.py
│   │
│   ├── tests/
│   │   └── test_api.py
│   │
│   └── requirements.txt
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Navbar.jsx
│   │   │   ├── GISMap.jsx
│   │   │   ├── CitizenPortal.jsx
│   │   │   ├── RecommendationView.jsx
│   │   │   ├── MisalignmentView.jsx
│   │   │   ├── PolicySimulator.jsx
│   │   │   ├── AICopilotModal.jsx
│   │   │   └── DPGHub.jsx
│   │   │
│   │   ├── services/
│   │   │   └── api.js
│   │   ├── App.jsx
│   │   └── index.css
│   │
│   ├── index.html
│   │   └── package.json
│
├── README.md
└── package.json

⚙️ Backend

The backend is built with Python and FastAPI.

It provides:

REST APIs

Citizen complaint processing

NLP and multilingual processing

Voice processing

GIS hotspot analysis

Project prioritization

Spending analysis

Policy simulation

AI-generated policy documents

💻 Frontend

The frontend is built with React.

It provides the user interface for:

Citizen submissions

GIS maps

Project recommendations

Spending analysis

Policy simulation

AI policy tools

DPG/open-data features

⚙️ How to Run
Prerequisites

Install:

Python 3.10+

Node.js 18+

npm 9+

Option 1 — Run the Full Project

From the project root:

npm install
npm run dev


This starts both services:

Frontend  → http://localhost:5173
Backend   → http://localhost:8000

Option 2 — Run Backend Separately
cd backend
pip install -r requirements.txt
uvicorn app.main:app --reload --port 8000


Backend API:

http://localhost:8000


Swagger API documentation:

http://localhost:8000/docs


ReDoc documentation:

http://localhost:8000/redoc

🧪 Run Backend Tests
cd backend
pytest tests

💻 Run Frontend Separately

Open another terminal:

cd frontend
npm install
npm run dev


Frontend:

http://localhost:5173

🌐 Supported Regions

NagarMithra contains regional baseline data and multilingual support for selected regions across:

🇮🇳 India

🇧🇷 Brazil

🇿🇦 South Africa

🇨🇳 China

🇷🇺 Russia

The architecture can be extended to additional countries, administrative regions, languages, and infrastructure sectors.

🔐 Privacy & Responsible AI

NagarMithra is designed around privacy-preserving and transparent decision-support principles.

Important design considerations include:

PII protection and data minimization

Coordinate anonymization/jittering where appropriate

Transparent MCDA criteria and weights

Human oversight of AI-generated recommendations

Separation between citizen feedback and administrative decisions

Open standards and interoperable APIs

AI-generated outputs should be treated as decision-support information, not as automatic government decisions.

📊 Technology Stack
Frontend

React

JavaScript

Leaflet

Chart.js

Lucide

Backend

Python

FastAPI

Pydantic

Pytest

🤖 AI & Analytics

NLP

Speech-to-text

Multilingual processing

DBSCAN clustering

MCDA

Geospatial analytics

Policy simulation

📡 Data & Standards

REST API

OpenAPI 3.1

GeoJSON / RFC 7946

CSV

JSON-LD

👥 Authors

Built by Greeshma and Team

NagarMithra is developed as an open-source civic technology project focused on multilingual citizen participation, infrastructure analytics, and transparent public-sector decision support.

🚀 Project Goal

The long-term goal of NagarMithra is to provide an interoperable digital infrastructure through which citizen needs can be collected, understood, geographically analyzed, and presented to decision-makers in a transparent and evidence-based format.

The platform is designed to help connect grassroots infrastructure demands with planning, budgeting, and public-service delivery while keeping humans responsible for final policy and investment decisions.
