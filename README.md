<div align="center">
<br/>

# ⚡ AKATOR

**Advanced PC System Monitor**

[![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=flat-square&logo=python&logoColor=white)](https://python.org)
[![PySide6](https://img.shields.io/badge/PySide6-Qt6-41CD52?style=flat-square&logo=qt&logoColor=white)](https://doc.qt.io/qtforpython)
[![Windows](https://img.shields.io/badge/Windows-10%2F11-0078D6?style=flat-square&logo=windows&logoColor=white)](https://microsoft.com)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](LICENSE)

<br/>

*Real-time system monitoring with a cyberpunk neon-on-obsidian UI.*  
*Built across 20 Python modules using PySide6 (Qt6).*

<br/>

</div>

---

## 📦 Install & Run

```bash
git clone https://github.com/yourusername/akator.git && cd akator
pip install -r requirements.txt
python main.py
```

> **Build EXE** → `BUILD.bat` &nbsp;|&nbsp; **Install to Program Files** → `python install_windows.py` *(as Admin)*

---

## 🖥 What It Monitors

| | Page | Metrics |
|--|------|---------|
| ⬡ | Dashboard | Live gauges · stat cards · sparkline charts |
| ⬢ | CPU | Total % · per-core bars · frequency · temp |
| ▣ | Memory | RAM · Swap · breakdown bars · history |
| ◎ | Disk | R/W speed · partition usage |
| ⬥ | Network | Download · Upload · interface table |
| ◈ | GPU | Load · VRAM · temp · clock · power |
| ≡ | Processes | Live sortable table · search |
| ⚡ | Battery | Charge % · status · time remaining |
| 🌡 | Temperature | All hardware sensors |
| ℹ | System Info | OS · CPU · memory · network · uptime |
| ⚠ | Alerts | Configurable thresholds · live log |

---

## 🎨 Design

```
Dark   #0D0F14 · #00D4FF · #7B2FFF · #00FF88 · #FFB800 · #FF3860
Light  #F0F4FF · #0066CC · #6200EA · #00A352 · #F57C00 · #D50000
```

- Animated pulsing logo · circular arc gauges · gradient sparklines  
- Color-coded load — cyan → yellow → red as usage increases  
- System tray · fade-in on launch · ◑ one-click theme toggle  

---

## 📁 Structure

```
akator/
├── main.py                   # entry point
├── BUILD.bat                 # one-click EXE builder
├── install_windows.py        # installs to Program Files
├── requirements.txt
└── src/                      # 20 modules
    ├── app.py                # main window · tray
    ├── theme_manager.py      # dark / light palettes
    ├── data_collector.py     # background psutil thread
    ├── charts.py             # sparkline · gauge · bar chart
    ├── widgets.py            # StatCard · SectionCard
    ├── animated_header.py
    ├── sidebar.py
    ├── status_bar.py
    ├── dashboard.py
    ├── cpu_monitor.py
    ├── memory_monitor.py
    ├── disk_monitor.py
    ├── network_monitor.py
    ├── gpu_monitor.py
    ├── process_monitor.py
    ├── battery_monitor.py
    ├── temperature_monitor.py
    ├── system_info.py
    └── alerts_widget.py
```

---

## ⚙️ Dependencies

```
PySide6 · psutil · Pillow · pyinstaller
```

> GPU monitoring needs `pip install gputil`

---

<div align="center">

Made with ⚡ &nbsp;·&nbsp; [MIT License](LICENSE) &nbsp;·&nbsp; Star if you like it ⭐

</div>
