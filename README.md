# X-SyncTrace v4

<p align="center">
  <img src="logo.png" alt="X-SyncTrace Logo" width="300"/>
</p>

<p align="center">
  <b>Advanced Forensic Browser Artifact Analyzer + UBPA Engine</b><br/>
  A powerful, court-ready digital forensics tool for analyzing Chrome, Edge, Firefox & Brave browser history, sync artifacts, and user behaviour patterns.
</p>

<p align="center">
  <a href="https://malwadkarrohan03-dev.github.io/XSyncTrace">
    <img src="https://img.shields.io/badge/Live%20Demo-Online-brightgreen?style=for-the-badge" alt="Live Demo"/>
  </a>
  <img src="https://img.shields.io/badge/Version-4.0-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge"/>
</p>

---

## ✨ Key Features

- 🔍 **Full Browser History Analysis** — Chrome, Edge, Firefox, Brave, Safari
- 🔄 **Sync Events & Cross-Device Tracking** — Visualise sync sessions and linked devices
- 🧠 **UBPA** — User Behaviour Pattern Analysis Engine with confidence scoring
- ⚠️ **Anomaly Detection** — Late-night bursts, high-frequency visits, suspicious domains
- 🔐 **SHA-256 Hash Verification** — Cryptographic chain of custody (ISO/IEC 27037 compliant)
- 📋 **Court-Ready Forensic Reports** — Admissibility checklist, exportable JSON/CSV/PDF
- 🐍 **Python Collector Script** — Read-only on-site acquisition for Windows machines

---

## 🚀 Live Demo

👉 **[https://malwadkarrohan03-dev.github.io/XSyncTrace](https://malwadkarrohan03-dev.github.io/XSyncTrace)**

---

## 📥 How to Use

### Option A — Python Collector (Recommended for Field Use)
1. Download [`xsynctrace_collector.py`](xsynctrace_collector.py) and run it on the target Windows machine:
   ```bash
   python xsynctrace_collector.py --browser chrome --case CASE-001 --examiner "Your Name"
   ```
2. It generates `xsynctrace_export.json` with a SHA-256 hash chain of custody record.
3. Open the tool, go to **Collect Artifacts**, and drop in the JSON file.

### Option B — Direct File Upload
1. Open the [Live Demo](https://malwadkarrohan03-dev.github.io/XSyncTrace) in your browser.
2. Drag and drop your browser's raw `History` SQLite file (or a CSV/TXT export).
3. The tool auto-detects the format and parses it.

### Option C — TXT / CSV Converter
1. Paste or upload plaintext exports from tools like NetAnalysis or Browser History Examiner.
2. Use the **Format Converter** tab to convert to the internal JSON schema.

---

## 🧠 UBPA — User Behaviour Pattern Analysis

The UBPA engine analyses browsing patterns and classifies the user into one of the following profiles:

| Profile | Description |
|---------|-------------|
| 🎓 Student / Researcher | High education/research domain usage |
| 💼 Corporate / IT Employee | High work/professional domain usage |
| 🏦 Banking / Finance Professional | High banking/finance domain usage |
| 🌐 General Internet User | High social media + news usage |
| 🚨 Suspect / High-Risk User | Elevated suspect domain indicators |

Output includes: **Confidence Score**, **Domain Category Breakdown**, **Activity Heatmap**, **Radar Chart**, and a **Court-Ready Evidence Table**.

---

## 📁 Repository Files

| File | Description |
|------|-------------|
| `index.html` | Main tool — single file, runs in browser |
| `xsynctrace_collector.py` | Forensic Python collector script (Windows) |
| `logo.png` | Project logo |
| `README.md` | This file |

---

## 🛡️ Standards Compliance

- **ISO/IEC 27037:2012** — Digital evidence identification, collection & preservation
- **NIST SP 800-86** — Integrating forensic techniques into incident response
- **ACPO Good Practice Guide** — Principles for handling digital evidence

---

## 📦 Build Standalone .exe (Optional)

To create a standalone Windows executable of the Python collector (no Python required on target):

```bash
pip install pyinstaller
pyinstaller --onefile --name xsynctrace_collector xsynctrace_collector.py
```

The `.exe` will be in the `dist/` folder.

---

## ⭐ Support the Project

If you find X-SyncTrace useful, please **star ⭐ this repository** — it helps others discover the tool!

---

**Made for forensic professionals by forensic enthusiasts.**
**<img width="1893" height="906" alt="Screenshot 2026-05-07 182732" src="https://github.com/user-attachments/assets/b77fb359-8990-4b95-a39a-c36d08e614e2" />
<img width="1897" height="915" alt="Screenshot 2026-05-07 182203" src="https://github.com/user-attachments/assets/f7d7a694-fa71-49c0-b1c9-49160b67450f" />
<img width="1887" height="912" alt="Screenshot 2026-05-07 180938" src="https://github.com/user-attachments/assets/f1474ddb-86d1-4803-8d1e-e0389f13295b" />
<img width="1886" height="902" alt="Screenshot 2026-05-07 180741 - Copy" src="https://github.com/user-attachments/assets/a4d59566-5256-41a5-9f9e-6c97515e6be8" />



