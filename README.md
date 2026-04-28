# 🔥 ATI - Furnace Performance Dashboard

Progressive Web App (PWA) untuk monitoring performa **15 Furnace Machines** (ACE & DISA lines).

## 🚀 Live Demo

**URL:** https://andonoimagine-dev.github.io/ati-furnace/

## 📱 Install di Android

1. Buka URL di **Chrome Android**
2. Tap menu **⋮** (3 titik kanan atas)
3. Pilih **"Install app"** atau **"Add to Home screen"**
4. Konfirmasi install
5. Icon muncul di home screen — bisa dibuka seperti app native

## 💻 Install di Desktop (Chrome/Edge)

1. Buka URL di browser
2. Klik ikon **install** (➕) di address bar
3. Klik **"Install"**
4. App muncul di Start Menu / Applications

## ✨ Fitur

- ✅ **Dashboard 15 Furnace Lines** (ACE & DISA)
- ✅ **6 Metrik Utama:** Quality, Charges, Tonase, Gentani, Cycle Time, Temp Compliance
- ✅ **5 Interactive Charts** dengan Chart.js
- ✅ **Dual-axis chart** untuk Charges & Tonase
- ✅ **Heatmap view** untuk overview semua line
- ✅ **Filter range** (4W/8W/12W/26W/Custom)
- ✅ **Toggle Gentani** (Pure Remelting / + Holding)
- ✅ **Toggle Cycle Time** (With Adjust / Without Adjust)
- ✅ **Update Online** dari GitHub data folder
- ✅ **Upload Manual** file Excel
- ✅ **PWA Installable** (Android & Desktop)
- ✅ **Offline Support** via Service Worker

## 📊 Update Data

### Option 1: Online Update (Recommended)
1. Upload file Excel terbaru ke folder `data/` dengan nama `latest.xlsx`
2. Dashboard otomatis deteksi update
3. User klik tombol **"Update Online"** → data ter-refresh

### Option 2: Manual Upload
1. User klik **"Update Data"** di topbar
2. Pilih **"Upload File Excel"**
3. Drag-drop atau browse file `.xlsx`

## 📂 Struktur Excel yang Dibutuhkan

**Kolom Wajib:**
- `Week` (format: "W1 Apr 25")
- `Tanggal` (date format)
- `Line` (format: FM06, FM11, FM22, dll)
- `Jugde` (OK/NG)

**Kolom Optional:**
- `Total Charging` (Kg → auto konversi Ton)
- `Gentani_FM (Pure Remelting)` (kWh/ton)
- `Gentani_FM (+ Holding)` (kWh/ton)
- `Time_With_Adjust` (menit)
- `Time_Without_Adjust` (menit)
- `Temperature Check Komposisi` (°C)

## 🛠️ Tech Stack

- **Frontend:** HTML5 + CSS3 + Vanilla JavaScript
- **Charts:** Chart.js 4.4.0 + chartjs-plugin-datalabels
- **Excel Parser:** SheetJS XLSX.js
- **Fonts:** Inter + IBM Plex Mono
- **PWA:** Service Worker + Web App Manifest
- **Hosting:** GitHub Pages

## 🏭 Line Configuration

**ACE Lines (8):** FM11, FM12, FM14, FM15, FM16, FM17, FM18, FM22  
**DISA Lines (7):** FM06, FM07, FM09, FM10, FM19, FM20, FM21

## 📝 License

MIT © Andono
