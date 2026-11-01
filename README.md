# 🚗 Automotive Engineering Simulations Dashboard

An interactive, web-based educational and professional platform designed to bridge mathematics, engineering theory, and practical automotive manufacturing applications.

🌐 **Live Platform Access:** [https://rashidia.github.io/Automotive-simulation-student-version/](https://rashidia.github.io/Automotive-simulation-student-version/)

---

## 🎯 Platform Objective
The objective is simple and direct: connect foundational mathematics, core engineering principles, and real-world automotive design and manufacturing processes into interactive, visual simulations.

---

## ✨ Dashboard Features

The main page (`index.html`) is a single self-contained file with no external libraries:

* **Module cards** for every simulator, with icon, description, topic tags and a NEW badge for recent additions.
* **Search and topic filters** to find a simulator quickly.
* **Live stats** (number of simulators, topics, and how many you have opened).
* **"Continue where you left off"** row and per-card open counts, saved in the visitor's own browser.
* **"Surprise me"** button that opens a random simulator.
* **Dark and light themes**, following the system setting by default.
* **Keyboard shortcuts:** `/` search, `1`–`6` open a simulator, `T` switch theme, `Esc` clear search.
* **Animated background**, hover tilt and glow on cards, and a mobile-friendly layout. Animations are turned off for visitors who prefer reduced motion.

---

## 🛠️ Included Simulations

The platform currently includes six interactive simulation modules:

1. **Car Anatomy Lab** 🆕
   * **Focus:** A realistic 3D car for exploring how a vehicle is built, with six systems: body and frame, engine, transmission, suspension and wheels, control systems (steering and brakes), and electrical.
   * **What you can do:** Switch between systems, explode the body into sub-assemblies, see inside the cabin with see-through panels and part labels, drive the car with adjustable speed, steering and brakes, and watch live values for each system (gear ratios, suspension travel, brake pressure, battery voltage and current).
   * **Guided tour:** A 10-step automatic tour with spoken narration in **English or Bahasa Melayu** (or audio off). Narration uses the browser's built-in speech voices, so the quality depends on the voices installed on the device.
   * **Key Learnings:** How the main systems of a car work and fit together, from crash structure and the four-stroke cycle to gear selection, Ackermann steering, hydraulic braking and the 12 V electrical system.

2. **Adaptive Spot Welding Simulator**
   * **Focus:** Explore how closed-loop feedback systems work in resistance spot welding.
   * **Key Learnings:** Dynamic resistance tracking, feedback control loops, and quality consistency.

3. **Automotive Welding Math Simulator**
   * **Focus:** Explore the mathematical principles behind spot welding, Gas Metal Arc Welding (GMAW), and laser welding.
   * **Key Learnings:** Visualize how mathematical equations directly relate to weld outcomes, heat input, and nugget growth.

4. **Car Plant Process Simulator**
   * **Focus:** Learn about end-to-end automotive manufacturing shop floor processes through simulation.
   * **Key Learnings:** Production flow, bottlenecks, assembly sequencing, and plant logistics.

5. **Laser Seam Tracking Simulator**
   * **Focus:** Explore the concept of tracking a welding seam in an automated laser welding process.
   * **Key Learnings:** Machine vision principles, sensor feedback, and real-time path correction.

6. **Torque Line Monitor**
   * **Focus:** Understand torque monitoring systems in modern automotive assembly lines.
   * **Key Learnings:** Fastener torque verification, error-proofing (poka-yoke), and assembly data tracing.

---

## 🚀 Getting Started Locally

If you wish to run or inspect the dashboard source code locally:

1. **Clone or Download** the repository to your local directory.
2. Ensure you have the main dashboard file (`index.html`) along with the individual HTML simulation files in the same root directory.
3. Open `index.html` in any modern web browser or run it via a local development server (e.g., VS Code Live Server).

> **Note on Car Anatomy Lab:** the file is large (about 16 MB) because the 3D car models are embedded inside it, so it may take a few seconds to load. It needs a browser with WebGL (any current Chrome, Edge, Firefox or Safari). For the spoken tour, a Malay or Indonesian system voice is needed for Bahasa Melayu narration; without one the tour shows the text only.

---

## ➕ Adding a New Simulator

1. Put the new `.html` file in the same folder as `index.html`.
2. Open `index.html` and add one entry to the `MODULES` list near the top of the script (file name, title, topic, colour, description, tags and an icon).
3. Update the Project Structure section below, then commit.

---

## 📂 Project Structure

```text
├── index.html                               # Main simulation dashboard
├── Car Anatomy Lab Latest.html              # 3D car anatomy module (six systems, guided tour EN/BM)
├── Adaptive Spot Welding Simulator.html     # Adaptive welding module
├── Automotive Welding Math Simulator.html   # Welding math & physics equations module
├── Car Plant Process Simulator.html         # Manufacturing workflow module
├── Laser Seam Tracking Simulator.html       # Machine vision & laser tracking module
├── Torque Line Monitor.html                 # Assembly torque monitoring module
└── README.md                                # This file
```

---

## 🧩 Credits and Notes

* The Car Anatomy Lab uses [three.js](https://threejs.org/) for 3D rendering. The car shell, wheels, brake discs, calipers and interior come from a Mitsubishi Lancer Evolution model, and the body-in-white structure from a Toyota Camry model, both supplied by the author. Please check the original model licences before wider redistribution.
* This is a student version intended for teaching. Values shown in the simulators are simplified for learning and are not for real vehicle design or safety decisions.
