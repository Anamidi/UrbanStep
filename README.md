# 🧓 UrbanStep — Senior & Assistive City Walk Navigator

> An assistive urban mobility platform engineered specifically for **Senior Citizens** and **Visually Impaired Individuals**, enabling comfortable, step-free, and safe pedestrian navigation in any city worldwide.

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io)
[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 🌟 What Makes UrbanStep Different?

| Feature | Standard Maps (Google / Apple) | **UrbanStep** |
| :--- | :--- | :--- |
| **Walking Speed Model** | Assumes brisk continuous walking (~4.8–5.0 km/h) without pauses. | **Personalized Pacing**: 3.0 km/h for seniors, 2.7 km/h for cane navigation. |
| **Fatigue & Stamina** | None. No concept of cardiac or joint exhaustion. | **Stamina Pacer™**: Schedules mandatory 3-minute seated rest breaks every 220–250m. |
| **Seating & Benches** | Hidden or non-existent on walking routes. | **Maps verified shaded benches** & transit shelters directly along the path. |
| **Sensory Guidance** | "In 200 feet, turn right onto Main St." | **Announces tactile braille pavers (TGSI)**, curb warnings, and 90dB acoustic crossings. |
| **Caregiver Peace of Mind** | Complex background tracking requiring apps and accounts. | **1-Click WhatsApp Check-in**: Sends pre-formatted itinerary & rest pauses to family. |
| **Cognitive Ergonomics** | Cluttered with ads, reviews, and tiny fonts. | **3-Slide Large-Text Wizard**: 20px+ fonts, high contrast mode, and zero clutter. |

---

## 🚀 Live 3-Slide Progressive Experience

1. **Step 1: Choose City & Walk Route**
   - Quick presets (New Delhi, Mumbai, Bengaluru, Jaipur, London, New York) or search **ANY city worldwide** (e.g. Pune, Chicago, Paris, Dubai, Sydney).
   - Custom Origin & Destination search with live OpenStreetMap Nominatim geocoding.
   - Built-in **Voice Recognition (Speech-to-Text)** via Web Speech API.

2. **Step 2: Rest & Stamina Plan**
   - Calculates distance, step counts, and planned seated bench breaks.
   - 1-Click WhatsApp Caregiver link with pre-formatted itinerary.

3. **Step 3: Guided Walk & Voice Navigation**
   - High-visibility Folium walking map with rest benches and acoustic traffic signals.
   - Hands-free **Voice Guidance Reader (Text-to-Speech)**.
   - Large 20px turn-by-turn instruction cards.
   - 1-Tap Emergency SOS dispatch dialer.

---

## 💻 Local Installation & Setup

### 1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/UrbanStep.git
cd UrbanStep
```

### 2. Create and activate a virtual environment
```bash
# Windows
py -m venv venv
venv\Scripts\activate

# macOS / Linux
python3 -m venv venv
source venv/bin/activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the Streamlit app
```bash
streamlit run app.py
```
Open your browser at **`http://localhost:8501`**.

---

## ☁️ Free Cloud Deployment (Streamlit Community Cloud)

1. Push this repository to your GitHub account.
2. Visit [share.streamlit.io](https://share.streamlit.io/) and sign in with GitHub.
3. Click **"New app"**.
4. Select your repository (`UrbanStep`), branch (`main`), and set the main file path to:
   ```
   app.py
   ```
5. Click **"Deploy"**! Your app will be live with a free public URL (e.g. `https://urbanstep.streamlit.app`).

---

## 🛠️ Tech Stack & Open Data
* **Frontend / Framework:** Streamlit & Streamlit-Folium
* **Maps & Cartography:** Folium & OpenStreetMap (OSM)
* **Routing Engine:** Project OSRM (Open Source Routing Machine) Foot Profile
* **Geocoding:** Nominatim OpenStreetMap API
* **Sensory APIs:** HTML5 Web Speech API (SpeechSynthesis & SpeechRecognition)

---

## 📄 License
This project is open-source under the [MIT License](LICENSE).
