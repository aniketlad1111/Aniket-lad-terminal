# ⚡ Aniket Lad Intelligence Terminal

> **Personal Commodity, FX & India Market Intelligence Dashboard**  
> Built on top of [WorldMonitor](https://github.com/koala73/worldmonitor) by koala73 — integrated, extended and customized.

[![GitHub](https://img.shields.io/badge/GitHub-aniketlad1111-amber?logo=github)](https://github.com/aniketlad1111)
[![WorldMonitor](https://img.shields.io/badge/Based%20On-WorldMonitor%20by%20koala73-purple?logo=github)](https://github.com/koala73/worldmonitor)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)
[![Live](https://img.shields.io/badge/Deploy-GitHub%20Pages-blue)](https://aniketlad1111.github.io/aniket-lad-terminal)

---

## 🌍 Live Demo

**GitHub Pages:** https://aniketlad1111.github.io/aniket-lad-terminal

---

## 📸 Features

| Feature | Description |
|---|---|
| 🥇 **Gold & Silver** | MCX, COMEX, Spot, XAU/USD, XAG/USD, XAU/INR — all in one panel |
| 🛢️ **Oil Markets** | WTI, Brent, OPEC Basket, Dubai Crude, Urals, MCX Crude, Nat Gas |
| 💱 **15 FX Pairs** | Majors + 🇮🇳 India crosses (USD/INR, EUR/INR, GBP/INR, JPY/INR) + Commodity FX |
| 🇮🇳 **India Markets** | NIFTY 50, SENSEX, NIFTY BANK, NIFTY IT, NIFTY METAL, NIFTY ENERGY, MCX instruments |
| 📰 **News Impact** | AI-classified news with OIL/GOLD/FX/INDIA impact scores per article |
| 🌍 **WorldMonitor** | Full integration — click "WORLD INTEL" to open WorldMonitor in-app |
| 🗺️ **Live Map** | 7 chokepoint rings, 10 tankers, 8 refineries, 4 weather events, 4 conflict zones, India infrastructure |
| 🔔 **Smart Alerts** | CRITICAL/HIGH/MEDIUM browser notifications with audio beep |
| ⏱️ **1-Second Refresh** | All prices update every second with micro-jitter simulation |
| 🇮🇳 **IST Clock** | India Standard Time (UTC+5:30) displayed prominently |
| 📱 **Fully Responsive** | Phone, Tablet, Desktop — automatic layout per device |

---

## 📱 Responsive Design

| Device | Layout |
|---|---|
| 📱 **Phone (≤600px)** | Full-screen map + slide-in sidebars + bottom nav bar |
| 📟 **Tablet (≤900px)** | Map + left sidebar, right sidebar hidden, bottom panels reduced |
| 🖥️ **Desktop (>900px)** | Full 3-column layout + 5-panel bottom strip |

---

## 🚀 Quick Start — Local Machine

### Option 1: Just open the file (zero setup)
```bash
# Download or clone this repo
git clone https://github.com/aniketlad1111/aniket-lad-terminal.git
cd aniket-lad-terminal

# Open directly in browser
open index.html          # macOS
start index.html         # Windows
xdg-open index.html      # Linux
```

### Option 2: Local server (recommended — fixes CORS)
```bash
# Using Python (built into macOS/Linux)
python3 -m http.server 8080
# Then open: http://localhost:8080

# Using Node.js
npx serve .
# Then open: http://localhost:3000

# Using VS Code — install Live Server extension and click "Go Live"
```

### Option 3: Ollama AI (for live intelligence analysis)
```bash
# Install Ollama
curl -fsSL https://ollama.ai/install.sh | sh    # macOS/Linux

# Pull model
ollama pull llama3.2

# Start Ollama (runs on port 11434)
ollama serve

# Open terminal and run your dashboard
open index.html
```

---

## 🌐 Deploy as Website (GitHub Pages)

### Step 1: Fork this repo
Click **Fork** at the top of this page.

### Step 2: Enable GitHub Pages
1. Go to your forked repo → **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: **main** → **/ (root)**
4. Click **Save**

### Step 3: Access your live site
```
https://aniketlad1111.github.io/aniket-lad-terminal
```

---

## 🔑 Configure API Keys (Optional — Live Data)

Edit the `CONFIG` section at the top of `index.html`:

```javascript
const CFG = {
  OLLAMA: 'http://localhost:11434',      // Your local Ollama
  MODEL: 'llama3.2',                      // Your Ollama model
  WM_URL: 'https://worldmonitor.app',    // WorldMonitor (auto-linked)
};
```

### Free API Keys for Live Data

| Service | URL | Used For | Free Tier |
|---|---|---|---|
| **Alpha Vantage** | https://alphavantage.co | Live commodity + FX prices | 25 calls/day |
| **AISHub** | https://aishub.net | Live tanker vessel tracking | Free |
| **EIA Open Data** | https://eia.gov/opendata | US energy data, pipelines | Free |
| **OpenWeatherMap** | https://openweathermap.org/api | Weather events | 1000 calls/day |
| **Groq** | https://groq.com | Fast AI inference (Ollama alternative) | Free tier |

---

## 🏗️ Project Structure

```
aniket-lad-terminal/
├── index.html              # Main dashboard (single file, no build)
├── README.md               # This file
├── LICENSE                 # MIT License
├── SETUP.md                # Detailed setup guide
├── CUSTOMIZATION.md        # How to customize for your needs
├── WORLDMONITOR_CREDIT.md  # WorldMonitor attribution
└── docs/
    └── SCREENSHOT.md       # Screenshots & demo info
```

---

## 🌍 WorldMonitor Integration

This project is built on top of **[WorldMonitor](https://github.com/koala73/worldmonitor)** by **koala73**.

- ⭐ Star the original: https://github.com/koala73/worldmonitor
- WorldMonitor is embedded via the "WORLD INTEL" button in the header
- The map chokepoint system, news intelligence architecture, and focal point detection are inspired by WorldMonitor's design

---

## 📊 What's Tracked

### Commodities
- WTI Crude, Brent Crude, OPEC Basket, Dubai Crude, Urals
- Natural Gas (Henry Hub, MCX, EU TTF, UK NBP)
- LNG (JKM Asian Marker)
- Coal (API2, ARA)
- EU Carbon (EUA)

### Precious & Industrial Metals
- Gold (MCX ₹, COMEX $, Spot, XAU/USD, XAU/INR)
- Silver (MCX ₹, Spot, XAG/USD)
- Copper, Platinum, Palladium, Iron Ore, Aluminium

### India Markets
- Indices: NIFTY 50, BSE SENSEX, NIFTY BANK, NIFTY IT, NIFTY METAL, NIFTY ENERGY
- MCX: Gold, Silver, Crude Oil
- Currencies: USD/INR, EUR/INR, GBP/INR, JPY/INR
- Other: India VIX, RBI Repo Rate

### FX Pairs (15 total)
- Majors: EUR/USD, GBP/USD, USD/JPY, USD/CHF, USD/CAD, AUD/USD
- India: USD/INR, EUR/INR, GBP/INR, JPY/INR
- Commodity: USD/RUB, USD/SAR, USD/CNH, USD/AED
- EM: USD/BRL

---

## 🗺️ Map Features

### Chokepoints (7 — with pulsing ring animation)
1. Strait of Hormuz — 20% global oil
2. Strait of Malacca — 80% Asia energy
3. Suez Canal — 12% global trade
4. Bab-el-Mandeb — Yemen route
5. Bosphorus Strait — Black Sea exports
6. Dover Strait — North Sea route
7. Danish Straits — Baltic Sea

### Vessels (10)
VLCCs, LNG carriers, Suezmax tankers including JAI HIND and PETRONET GAS serving India routes

### India Infrastructure
Jamnagar Refinery, Dahej LNG Terminal, Paradip Refinery, Kochi Refinery, ONGC Offshore BG-1, Mundra Port

---

## 🤖 AI Integration (Ollama)

The terminal connects to your local Ollama instance for:
- News severity classification (CRITICAL / HIGH / MEDIUM / LOW)
- Commodity impact scoring per news article
- Trading implication generation

**System Prompt used:**
```
You are an energy commodity trading intelligence analyst.
Classify news by impact on commodity prices.
Rate severity: CRITICAL | HIGH | MEDIUM | LOW
Identify commodity: CRUDE_OIL | GOLD | SILVER | LNG | COPPER | COAL | CURRENCY | MULTIPLE
Output format: JSON with severity, commodity, side, chokepoint, implication, confidence
```

---

## 📱 Phone Usage Tips

- Tap **☰** (menu) in top-left → opens Price/Layer/Region panel
- Bottom nav bar: 🗺️ MAP | 📊 PRICES | 📡 NEWS | 🌍 WORLD | 🔔 ALERT
- Tap any news item to expand AI trading implication
- Tap any price card to open mini chart

---

## 🙏 Credits & Attribution

| Project | Author | Link |
|---|---|---|
| **WorldMonitor** | koala73 | https://github.com/koala73/worldmonitor |
| **Leaflet.js** | Leaflet Team | https://leafletjs.com |
| **CartoDB Dark Tiles** | CartoDB | https://carto.com |
| **Ollama** | Ollama Team | https://ollama.ai |

---

## 📄 License

MIT License — See [LICENSE](LICENSE)

Built by **Aniket Lad** ([@aniketlad1111](https://github.com/aniketlad1111))  
Based on [WorldMonitor](https://github.com/koala73/worldmonitor) by koala73 ⭐

---

*Kolhapur, Maharashtra, India 🇮🇳*
