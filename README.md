# 🛡️ HoneyTrap Cybersecurity Dashboard — Static Web UI Project

A fully responsive, visually interactive **cybersecurity monitoring dashboard UI**, designed to simulate the look and feel of a real-world threat detection system. Developed using **HTML5, CSS3, Vanilla JavaScript**, and **Chart.js**, this project demonstrates frontend concepts like modular layouting, chart rendering, dark mode toggling, and SPA-style tab navigation.

---

## 📌 Project Overview

**HoneyTrap** is a static, client-side dashboard prototype designed for:
- **Learning frontend development (HTML/CSS/JS)**
- **Practicing UI design for data monitoring applications**
- **Building a clean, responsive layout with visual data representation**
- **Showcasing portfolio-level frontend skills using live charts and modern UI**

Although the data shown is **static and mock**, the layout, structure, and logic simulate a production-grade security operations center (SOC) dashboard.

---

## 🎯 Core Objectives

| Objective                        | Description |
|----------------------------------|-------------|
| ✨ Modern UI Design              | Clean layout with light/dark themes |
| 📊 Interactive Charts           | Visualizing data using Chart.js |
| 🧩 Modular Tabbed Navigation    | SPA-like experience with dynamic tab switching |
| 📱 Responsive Design            | Works on desktops, tablets, and phones |
| 🧠 Simulated Threat Intelligence| Mimics real-time dashboard stats |

---

## 🛠️ Technologies & Tools Used

| Technology       | Purpose                                              |
|------------------|------------------------------------------------------|
| **HTML5**        | Core markup for structure                            |
| **CSS3**         | Styling, layout, responsiveness                      |
| **JavaScript (ES6)** | Logic for dark mode, tab switching, charts       |
| **Chart.js v4**  | JavaScript charting library for data visualizations |
| **Font Awesome** | Icon library for sidebar/tab icons                  |
| **Google Fonts** | Typography with 'Poppins' font                      |
| **CDN Integration** | Load libraries via cloud for zero setup           |

---

## 🧩 Dashboard Sections & Functionalities

### 🔸 Sidebar Navigation
- Fixed vertical bar with icon-based tabs.
- Active tab is highlighted dynamically.
- Icons represent: Home, Performance, Network, Settings, Help.

### 🔸 Header Section
- Branding with a circular AI-themed logo.
- `HoneyTrap` title displayed using custom font.
- Search bar (UI only, not functional).
- **Dark mode toggle** button.

### 🔸 Dashboard Tab (Default Active)
- **Stat Cards:**  
  - Total Attacks Detected  
  - Live Attack Count  
  - Server Health Status

- **Top Info Section:**  
  - Top Targeted Endpoints  
  - Geolocation of Attack Source

- **Analytics Section:**  
  - **Donut Chart:** Threat Type Distribution (Broken Machine, Human Error, Personal Breaks)  
  - **Text Panel:** Placeholder for Live Logs, AI Analysis, Threat Classification  
  - **Line Chart:** Quarterly Attack Frequency Comparison (Threats Detected vs Safe Logs)

### 🔸 Other Tabs (Content Static)
- **Performance:** Uptime stats and monitored nodes
- **Network Traffic:** Inbound/Outbound packet metrics
- **Settings:** Placeholder for user preferences/security controls
- **Help:** Dummy documentation and contact info

---

## 🌗 Theme Switching (Dark Mode)

Implemented using a `dark` class toggle on `<body>`, triggered by a button.  
Automatically changes:
- Backgrounds
- Text colors
- Box shadows
- Card visuals  
This is a **best-practice approach** for lightweight theming using minimal JS.

---

## 📊 Chart Implementations

### 1. Donut Chart
- Rendered using `<canvas id="donutChart">`
- Uses custom cutout radius (`70%`) to simulate a donut
- Labels and percentages shown via static legend

### 2. Line Chart
- Rendered using `<canvas id="attackChart">`
- Two datasets:
  - `Threats Detected` (Primary Line)
  - `Safe Logs` (Secondary Line)
- Smooth curves using `tension` property
- Responsive with grid scaling

---

## 🧠 Developer Insights

- All DOM interactions handled using `document.querySelectorAll` and JS event listeners.
- Tabs are switched using dynamic class-based logic — no page reloads.
- No external `.css` or `.js` files used — everything is inline for simplicity and portability.
- Fully responsive design using `@media` queries (`max-width: 768px`).
- Project is **dependency-free** except for CDN-hosted libraries.

---

## 📁 Project Structure

