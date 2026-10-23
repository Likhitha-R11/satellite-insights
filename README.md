# 🛰️ Satellite Insights

**Turning Satellite Data into Meaningful Geospatial Insights**

Satellite Insights is a web-based geospatial analysis platform designed to explore satellite imagery and derive meaningful environmental and land-surface information. By combining a web interface with satellite data processing, the project aims to make geospatial analysis more accessible for applications in agriculture, environmental monitoring, disaster assessment, and urban planning.

## 🌍 Overview

Satellite imagery provides valuable information about changes occurring on Earth's surface. Satellite Insights brings together a frontend application and a backend processing system to help users explore satellite-derived information for a selected geographical area and analysis period.

The project integrates **Google Earth Engine (GEE)** for satellite data access and processing with a Flask-based backend and a React-based frontend.

## ✨ Key Capabilities

- **Satellite Data Analysis:** Access and process satellite datasets for geospatial analysis.
- **Vegetation Monitoring:** Use vegetation indices such as NDVI and EVI to study vegetation conditions, where supported by the selected dataset and implemented analysis.
- **Water Analysis:** Use NDWI to help identify and assess water-related features.
- **Built-up Area Analysis:** Use NDBI to investigate built-up and urbanized surfaces.
- **Geospatial Visualization:** Present analysis results through a web-based interface.
- **Environmental Applications:** Support exploratory analysis related to agriculture, environmental change, disaster assessment, and urban development.

*The availability of each capability depends on the implemented application features and supported datasets.*

## 🛠️ Technology Stack

### Frontend
- React.js
- TypeScript
- Vite

### Backend
- Python
- Flask
- Google Earth Engine

### Geospatial Analysis
- Satellite imagery and derived spectral indices
- Geospatial data processing and visualization

## 🏗️ System Architecture

The application follows a frontend–backend architecture.

1. **User Interface:** The frontend provides the interface for selecting analysis inputs and viewing results.
2. **API Communication:** The frontend communicates with the backend through HTTP API requests.
3. **Satellite Data Processing:** The Flask backend accesses Google Earth Engine to retrieve and process supported satellite data.
4. **Index Calculation:** Relevant spectral indices are calculated or retrieved as part of the analysis workflow.
5. **Results Presentation:** The processed outputs are returned to the frontend for visualization, depending on the implemented features.

```text
                 User
                  |
                  v
        React + TypeScript UI
                  |
              HTTP API
                  |
                  v
          Flask Backend
                  |
                  v
       Google Earth Engine
                  |
                  v
       Satellite Data Processing
                  |
                  v
       Analysis Results / Indices
                  |
                  v
         Frontend Visualization
```

## 🛰️ Satellite Indices

| Index | Full Form | Potential Application |
|---|---|---|
| NDVI | Normalized Difference Vegetation Index | Vegetation health and density assessment |
| NDWI | Normalized Difference Water Index | Water feature and surface-water analysis |
| EVI | Enhanced Vegetation Index | Vegetation monitoring with improved sensitivity in some conditions |
| NDBI | Normalized Difference Built-up Index | Built-up area and urban surface analysis |

These indices are derived from specific spectral bands. Their interpretation depends on the satellite sensor, selected bands, data quality, and processing methodology.

## 👩‍💻 My Contribution

My contribution to Satellite Insights focused on **backend development**, including:

- Working with Google Earth Engine to access satellite datasets.
- Supporting satellite data retrieval and processing workflows.
- Working with spectral indices used in environmental and land-surface analysis.
- Developing and working with Flask backend functionality to support frontend–backend communication.

The project was developed collaboratively, with separate frontend and backend codebases.

## 📁 Repository Structure

```text
satellite-insights/
├── clearsat-frontend/
│   └── Frontend application
├── clearsat-backend/
│   └── Backend application
├── README.md
└── .gitignore
```

## 🚀 Getting Started

### Prerequisites

Install the following tools before running the project:

- Git
- Node.js and npm
- Python
- Access to Google Earth Engine, with authentication and permissions configured if required by the backend

### 1. Clone the repository

```bash
git clone https://github.com/Likhitha-R11/satellite-insights.git
cd satellite-insights
```

### 2. Set up the frontend

```bash
cd clearsat-frontend
npm install
```

Start the frontend using the script configured in its `package.json`, commonly:

```bash
npm run dev
```

### 3. Set up the backend

Open a separate terminal from the project root:

```bash
cd clearsat-backend
python -m venv venv
```

Activate the virtual environment on Windows:

```bash
venv\Scripts\activate
```

Install the backend dependencies using the repository's dependency file, if provided:

```bash
pip install -r requirements.txt
```

Configure the required environment variables and Google Earth Engine authentication according to the backend implementation.

Start the Flask application using the entry point and instructions defined in the backend repository.

**Note:** The exact startup commands, ports, environment variables, and dependency filenames should be verified against the actual source code before use.

## 🔐 Security

- Do not commit API keys, passwords, service-account credentials, or private configuration files.
- Keep environment-specific settings in local environment files excluded through `.gitignore`.
- Follow Google Earth Engine authentication and access requirements.

## 🎯 Potential Applications

- Agricultural and vegetation monitoring
- Environmental change analysis
- Water-resource observation
- Disaster assessment and post-event analysis
- Urban growth and built-up area studies

These are intended application areas; the reliability of any analysis depends on the available imagery, implementation, and validation.

## 📌 Project Status

Developed as a collaborative geospatial analysis project. Features, supported datasets, and setup requirements should be confirmed against the current implementation.

