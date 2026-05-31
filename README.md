# 🖥️ MAD Optimizer — PC Lag Fix & Performance Tweaker

> A Windows batch script that optimizes low-end ("potato") PCs for better gaming and general performance through registry tweaks.

---

## 📋 Overview

**MAD Optimizer** (`M4D.bat`) is a lightweight Windows batch utility built in 2023 that applies targeted registry tweaks to squeeze more performance out of underpowered machines. It presents a simple menu-driven interface and lets you apply specific optimizations without needing to manually edit the registry.

---

## ✨ Features

The script offers four optimization modules:

| Option | Description |
|--------|-------------|
| **[1] GPU Tweaks** | Enables per-CPU-core DPC for NVIDIA drivers to reduce GPU scheduling latency |
| **[2] Fix Full Screen** | Fixes fullscreen exclusive mode issues (GameDVR/FSE behavior tweaks) |
| **[3] Boost FPS** | Comprehensive FPS boost — power settings, MMCSS tuning, disabling bloat |
| **[4] Optimize CPU** | Raises game task scheduling priority via MMCSS registry keys |

### What the FPS Boost does (Option 3):
- Disables **Power Throttling** for consistent CPU performance
- Disables **Hibernation** and **Fast Startup** to reduce boot overhead
- Disables **GameDVR / Xbox Game Bar** recording overlay
- Tunes **MMCSS (Multimedia Class Scheduler)** for gaming workloads — higher GPU/CPU priority, high scheduling category
- Removes **network throttling** limits
- Speeds up **process and service kill timeouts** for snappier response
- Disables **background Windows Consumer Features**, advertising ID, and silent app installs
- Disables **auto maintenance** tasks
- Restores **Windows Photo Viewer** file associations
- Disables virtual bus and kernel debug network adapter services (`kdnic`, `NdisVirtualBus`)
- Sets DirectX kernel (`DXGKrnl`) monitor latency tolerance to zero for lower display latency

---

## 🚀 Usage

1. **Download** `M4D.bat` from this repository.
2. **Right-click** the file and select **"Run as administrator"**.  
   *(The script checks for admin rights and will exit if not elevated.)*
3. **Choose an option** from the menu by typing the number and pressing Enter.
4. Repeat for any additional tweaks you want to apply.
5. **Restart your PC** after applying changes for full effect.

```
WELCOME TO MAD OPTIMIZER /(-_-)\ LAG FIX 5.2

[1] GPU Tweaks
[2] Fix Full Screen
[3] Boost FPS
[4] Optimize CPU
[0] Exit
```

---

## ⚙️ Requirements

- **OS:** Windows 10 / Windows 11
- **Privileges:** Administrator rights (required)
- **GPU:** Options 1 and parts of Option 3 are tailored for **NVIDIA GPUs** (`nvlddmkm` driver keys)

---

## ⚠️ Disclaimer

> This script modifies the **Windows Registry**. While the changes are reversible, use at your own risk.  
> It is recommended to **create a system restore point** before running the script.  
> The author is not responsible for any system instability caused by these tweaks.

---

## 📁 Files

```
MY-2023-OPTIMIZER/
└── M4D.bat    # Main optimizer script (237 lines)
```

---

## 👤 Author

**mnvvshu** — made this as a batch project back in 2023.

- Discord: [discord.io/mad](https://discord.io/mad)
- GitHub: [@mnvvshu](https://github.com/mnvvshu)
