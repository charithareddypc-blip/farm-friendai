# 🌾 Farm Friend AI (రైతు మిత్ర AI)
### *Smart, Honest Digital Companion for Indian Farmers*

A modern, mobile-friendly web application designed specifically for Indian farmers to empower daily farm operations with real live weather, transparent plant disease diagnostics, crop planning, precision watering, local task reminders, and MSP-based profitability calculations.

Built with **React 19**, **TypeScript**, **Vite**, and **Tailwind CSS**.

---

## 🌟 Key Features

### 1. Bilingual Support (English & Telugu - ఇంగ్లీష్ & తెలుగు)
- Seamless 1-tap switching between English and Telugu (రైతు మిత్ర AI).
- Full bilingual coverage across all 9 modules: UI labels, weather forecasts, crop names, symptom descriptions, organic/chemical treatments, chatbot responses, and safety manuals.
- Language preference is automatically saved in `localStorage`.

### 2. Live Weather & 7-Day Agricultural Forecast (Open-Meteo API)
- **100% Free** live meteorological data using the [Open-Meteo API](https://open-meteo.com/) — **no paid API keys or credit cards required**.
- Real-time temperature (°C), feels-like, relative humidity (%), precipitation (mm), wind speed (km/h), and WMO weather condition descriptions in English and Telugu.
- **Farming Action Alerts**: Advises whether current weather is safe for chemical spraying (wind < 20 km/h), drying harvested grain, or if rain requires postponing urea top-dressing.
- **Location Selector & Search**:
  - Instant presets for major Indian agricultural districts (Guntur, Vijayawada, Warangal, Karimnagar, Kurnool, Ludhiana, Pune, Belagavi, Coimbatore, Varanasi, Indore).
  - Geocoding search input for searching any Indian mandal, district, or city.
  - "Use My Current Location" button using HTML5 browser geolocation.
- 7-Day forecast cards showing daily max/min temperatures, precipitation sums, and rain probabilities.

### 3. Plant Doctor & Leaf Diagnostic (Transparent & Honest)
- **Honest AI Policy**: Prominently informs farmers that preliminary screening is based on scientific ICAR plant pathology rules and visual comparison matrices. **Never pretends an expensive vision AI is running when no vision model is configured.**
- **Photo Upload & Camera Capture**: Farmers can upload or capture a photo of the infected crop leaf for side-by-side visual inspection.
- **Symptom Matching Matrix**:
  - Filter by crop (Paddy, Cotton, Chilli, Tomato, Maize, Groundnut, Wheat).
  - Select affected plant part (Leaf, Stem, Fruit/Pod, Root).
  - Check observed symptoms (e.g., eye/spindle-shaped spots, upward boat curl for thrips, downward umbrella curl for mites, concentric target rings, bacterial ooze).
- **Comprehensive Remedies**:
  - Severity level (High, Medium, Low) and pathogen cause.
  - Immediate organic/natural remedies (Pseudomonas fluorescens, Panchagavya, fermented buttermilk, Neem oil 10,000 ppm).
  - Recommended scientific chemical treatment with ICAR-standard dosages (e.g., Tricyclazole 75% WP @ 0.6g/L, Spinetoram @ 1ml/L, Mancozeb @ 2.5g/L).
  - Long-term agronomic prevention strategies.
- **Visual Reference Gallery**: Side-by-side photographic comparison guide for common Indian crop diseases.
- 1-Click direct emergency dial to **Kisan Call Centre (`1800-180-1551`)**.

### 4. Crop Advisor & Season Planner
- Suggests suitable, high-yielding crops based on:
  - **Soil Type**: Alluvial (వండలి), Black Cotton (నల్లరేగడి), Red Sandy/Loam (ఎర్ర నేల), Laterite (లేటరైట్), Clay Loam (బంకమట్టి), Sandy Loam (ఇసుక నేల).
  - **Season**: Kharif / Monsoon (జూన్ - అక్టోబర్), Rabi / Winter (అక్టోబర్ - మార్చి), Zaid / Summer (మార్చి - జూన్).
  - **Region / State**: Andhra Pradesh, Telangana, Karnataka, Tamil Nadu, Maharashtra, Punjab, etc.
  - **Water Availability**: High (Canal/Borewell), Moderate, Low/Rainfed.
- Outputs suitability scores, duration in days, expected yield per acre, and critical agronomic advice.

### 5. Smart Watering Assistant (Weather-Integrated)
- Reads real-time rain forecast from Open-Meteo for the next 48 hours.
- Evaluates crop water requirements based on growth stage (Seedling, Vegetative, Flowering, Fruiting, Maturity), soil type, and irrigation system (Drip, Sprinkler, Flood).
- **Dynamic Decision**:
  - **STOP! DO NOT WATER TODAY**: If rain (>4mm) or high rain probability (>55%) is forecast. Highlights saved electricity (3-4 units/acre) and prevents root rot and nitrogen leaching.
  - **IMMEDIATE WATERING REQUIRED**: During critical flowering/grain-filling stages under hot, dry conditions.
  - **LIGHT / NORMAL WATERING**: When soil moisture is adequate.

### 6. Farming Chatbot (Rythu Mitra)
- Built-in Indian agricultural knowledge base — works **offline and 100% free** without OpenAI/Google Cloud paid API keys.
- Answers questions in English, Telugu script, and Tanglish.
- Curated coverage:
  - Government Subsidies: PM-KISAN (₹6,000/yr), Rythu Bharosa, PMKSY Drip Irrigation (70-90% subsidy), Soil Health Card, Solar Pump (PM-KUSUM).
  - Organic preparations: Step-by-step recipe for Jeevamrutham (200L for 1 acre using desi cow dung, gomutra, jaggery, besan).
  - Pests & Deficiencies: Zinc deficiency (Khaira disease), Rice blast, Chilli leaf curl & thrips, Cotton pink bollworm.
- One-tap quick question chips for convenience on mobile devices.

### 7. Fertilizer Calculator & Safety Manual
- Scientific N-P-K nutrient dosage calculation based on ICAR standards.
- Converts pure nutrients into commercial **Urea (46% N)**, **DAP (18-46-0)**, and **MOP (60% K₂O)** bags (45kg / 50kg) for any acreage.
- **Split Application Schedule**:
  - Basal dose at final ploughing / sowing.
  - 1st top dressing (20-25 days after sowing).
  - 2nd top dressing (panicle initiation / flowering stage).
- Organic alternatives: Farm Yard Manure (FYM), Jeevamrutham, Neem cake.
- **CRITICAL SAFETY WARNINGS**:
  - Mandatory PPE (masks, rubber gloves, goggles).
  - Spraying only in wind direction, never against wind.
  - Safe storage away from children, livestock, and water sources.
  - Emergency poisoning hotlines: National Poison Info Centre `1800-116-117` and Ambulance `108`.

### 8. Farming Calendar & Local Reminders
- Personal farm diary stored safely in `localStorage` (no account or login required).
- 1-Click pre-loaded crop cycle schedules:
  - **Paddy** (120-Day lifecycle from basal fertilization to drainage and harvest).
  - **Cotton** (150-Day lifecycle including pheromone trap installation).
  - **Chilli** (150-Day lifecycle with drip and neem oil spray intervals).
- Add custom tasks with crop name, date, category (sowing, irrigation, fertilizer, spraying, weeding, harvesting, mandi), and priority.
- "Due Today" alert banner highlighting tasks needing attention.

### 9. Crop-Cost & Profit/Loss Calculator
- Transparent farm economics engine:
  - Itemized input expenses: Field preparation, seeds, labor, fertilizer, pesticides, irrigation, weeding, harvesting, transport.
  - Revenue estimation based on expected yield (quintals) and price per quintal.
  - **Pre-filled with Official Government Minimum Support Prices (MSP 2024-25 / 2025-26)** published by the Ministry of Agriculture:
    - Paddy Common: ₹2,300 / Q
    - Cotton Medium Staple: ₹7,121 / Q
    - Maize: ₹2,225 / Q
    - Groundnut: ₹6,783 / Q
    - Wheat: ₹2,425 / Q
    - Bengal Gram: ₹5,440 / Q
    - Chilli: ₹9,500 / Q (indicative mandi rate)
  - Farmers can easily override with their local mandi rates.
- Computes:
  - Total Investment (₹)
  - Expected Gross Revenue (₹)
  - Net Profit or Loss (₹) with green/red alert
  - Breakeven cost of production per quintal
  - Return on Investment (ROI %)
  - Interactive SVG Expense Distribution breakdown bar.

---

## 🚀 Quick Start & Setup Instructions

### Prerequisites
- [Node.js](https://nodejs.org/) v18 or higher (v22 recommended).
- npm (Node Package Manager).

### 1. Installation
In the project directory, run:
```bash
npm install
```
*(On Windows PowerShell, if scripts are restricted, run `npm.cmd install`)*

### 2. Start the Development Server
```bash
npm run dev
```
Open your browser and navigate to:
```
http://localhost:5173
```

### 3. Build for Production
To create an optimized production build:
```bash
npm run build
```
The output will be placed in the `dist/` directory.

### 4. Preview Production Build
```bash
npm run preview
```

---

## 🛠️ Tech Stack & Dependencies
- **Framework**: React 19, TypeScript
- **Bundler & Dev Server**: Vite 8
- **Styling**: Tailwind CSS v4 with custom green-and-white farmer palette
- **Icons**: Lucide React
- **APIs**:
  - [Open-Meteo Forecast API](https://api.open-meteo.com/v1/forecast) (No API Key Required)
  - [Open-Meteo Geocoding API](https://geocoding-api.open-meteo.com/v1/search) (No API Key Required)
- **Local Persistence**: Browser `localStorage` for language settings and calendar reminders.

---

## ⚠️ Manual Steps & System Notes
1. **Windows PowerShell Execution Policy**:
   If PowerShell throws a script error (`npm.ps1 cannot be loaded because running scripts is disabled`), simply invoke `npm.cmd` instead of `npm`, e.g.:
   ```powershell
   npm.cmd run dev
   ```
2. **Browser Location Permission**:
   When using the "Use My Current Location" button in the Live Weather tab, allow browser location access when prompted. If declined, the app gracefully falls back to preset agricultural hubs.

---

## 📞 Agricultural Helplines (India)
- **Kisan Call Centre (KCC)**: `1800-180-1551` (Toll-Free, 6:00 AM – 10:00 PM, all Indian languages)
- **National Poison Information Centre (AIIMS)**: `1800-116-117`
- **National Emergency Ambulance**: `108`
- **PM-KISAN Helpline**: `155261` / `1800-115-526`
