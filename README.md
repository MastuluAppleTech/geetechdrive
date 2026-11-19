# 🏎️ GEETECH DRIVE — Mzansi Edition

> **"Moving the Kasi, the Geetech Way."**

A fast-paced, South African-themed 3D endless highway racer built with **Three.js**, **Tailwind CSS**, and **Web Audio API**. Weave through minibus taxis, survive Stage 4 load-shedding blackouts, dodge Metro Police speed traps, and unlock Mzansi street legends from the Renault KWID to the iconic **BMW 325is Gusheshe**[cite: 1, 2].

---

## 🎮 Gameplay Features

### 🏙️ Stage 1: City Streets (`index.html`)
* **Iconic SA Sectors:** Race across **Joburg** (Soweto Towers), **Cape Town** (Table Mountain), **Durban** (Golden Mile), and **Pretoria** (Jacaranda City)[cite: 1].
* **Authentic Mzansi Hazards:**
  * **Weaving Minibus Taxis:** Listen for the double-hoot before taxis swerve across lanes[cite: 1].
  * **Load-Shedding Stage 4:** Sudden grid blackouts plunge the highway into darkness, forcing you to rely on your high-beams for survival[cite: 1].
  * **Highveld Storms & Potholes:** Dynamic rain, lightning flashes, and suspension-wrecking potholes[cite: 1].
* **Kasi FM Procedural Radio:** Live Web Audio API synthesizer streaming **Piano FM** (3 original Amapiano log-drum tracks) and **Hip-Hop FM** (Kasi Trap 808 & Boom Bap)[cite: 1].

### 🏔️ Stage 2: Open Road (`stage2.html`)
* **Cross-Country Biomes:** Unlock Stage 2 via the **BMW 325is Gusheshe**[cite: 1, 2] to tear through the **Karoo**, **Garden Route**, **Drakensberg**, and **Kruger**[cite: 2].
* **Metro Police & The "Cooldrink" Mechanic:**
  * Collect rare **2L Cooldrink** inventory pickups on the highway.
  * If Metro Police pull you over (*"Hawu bhuti, awunayo i-cooldrink?"*), hand over a cooldrink from your boot to drive off clean—or get slapped with a **R1,000 fine** and have your car **impounded** (**R1,500 bail** in the Garage).
* **AI Overtakers & Checkpoint Timer:** Beat the countdown clock to each destination while dodging fast AI street racers overtaking from behind.

### 🔧 Geetech Garage & Progression
* **9 Unlockable Cars:** Renault KWID, VW Polo R-Line, VW Golf 8 GTI, Audi RS3, BMW 325is Gusheshe, Mercedes-AMG A45, BMW M3, Toyota GR Supra, and Lamborghini Huracán[cite: 1].
* **Performance Tuning:** Upgrade **Engine**, **Tyres**, and **Nitro** up to Level 3[cite: 1].
* **Custom SA License Plates:** Personalize your rear plate (e.g., `GEETECH GP`)[cite: 1].
* **Missions, Daily Streaks & Global Top 20 Leaderboard:** Cloud-synced high scores 

---

## 🕹️ Controls

| Action | Desktop (Keyboard / Mouse) | Mobile (Touch) |
| :--- | :--- | :--- |
| **Steer Left** | `A` / `Left Arrow` / Click Left Half | Tap Left Half or Swipe Left[cite: 1] |
| **Steer Right** | `D` / `Right Arrow` / Click Right Half | Tap Right Half or Swipe Right[cite: 1] |
| **Nitro Boost** | `W` / `Up Arrow` / `Spacebar`[cite: 1] | Swipe Up or Hold `⚡ NITRO BOOST`[cite: 1] |
| **Pause** | `P` / `Esc`[cite: 1] | Top-right Pause button[cite: 1] |

---

## 🛠️ Tech Stack & Architecture

* **3D Rendering:** [Three.js (r128)](https://threejs.org/) — procedural low-poly vehicles, skylines, dynamic fog, spotlights, and particle systems[cite: 1].
* **UI & Styling:** [Tailwind CSS](https://tailwindcss.com/) + Orbitron & Rajdhani typography[cite: 1].
* **Audio Engine:** Pure **Web Audio API** procedural sound synthesis (zero external `.mp3` assets required for engine RPM, sirens, taxi horns, thunder, and radio beats)[cite: 1].
* **Backend & Persistence:** `localStorage` for offline garage/inventory saves[cite: 1] + **Firebase Firestore** for the global Top 20 leaderboard[cite: 1].

---

## 🚀 Running Locally

Because the game uses ES modules for the Firebase leaderboard[cite: 1], serve it over a local HTTP server rather than opening the file directly via `file://`:

```bash
# 1. Clone the repository
git clone [https://github.com/YOUR-USERNAME/geetech-drive.git](https://github.com/YOUR-USERNAME/geetech-drive.git)
cd geetech-drive

# 2. Start a local server (Python 3)
python -m http.server 8000

# 3. Open in your browser
# http://localhost:8000/index.html
