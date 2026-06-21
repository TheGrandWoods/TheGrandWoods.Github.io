---

🧠 Best‑Practices Setup Guide for Your PC
Hardware:  
- ASUS ROG STRIX B450‑F GAMING II  
- Ryzen 5 3600  
- MSI RTX 3070 Gaming Z Trio  
- 32GB DDR4‑3200 (Corsair CMK32GX4M2E3200C16)  
- Windows 11 Home 25H2  
- SSDs: Kingston A400 + Samsung 980 NVMe  

---

1️⃣ BIOS: Critical Settings for Stability & Performance
(All BIOS references are from your uploaded manual — citations included.)

✔ Enable DOCP / XMP (Memory @ 3200 MHz)
Your RAM is rated for 3200 MHz CL16.  
In BIOS → Ai Tweaker → Ai Overclock Tuner → D.O.C.P. Standard  
The manual states:  
> “When you install XMP memory modules, we provide you the optimal frequency…” 

This gives you ~10–12% more CPU performance in games.

---

✔ Enable ReSize BAR (RTX 3070 supports it)
Top bar → ReSize BAR → On  
Manual:  
> “Enable ReSize BAR support to fully harness GPU memory.” 

This improves 3070 performance in many titles.

---

✔ Set Precision Boost Overdrive (PBO)
BIOS → Advanced → AMD Overclocking → Precision Boost Overdrive

Recommended for Ryzen 3600:
- PBO: Enabled
- PBO Scalar: x2
- Max CPU Boost Clock Override: +50 MHz
- Thermal Throttle Limit: 90°C

This is safe and gives +100–150 MHz under load.

---

✔ Disable C‑States only if you want max responsiveness
BIOS → Advanced → CPU Configuration

For gaming:
- Global C‑State Control: Enabled (default, best efficiency)

For ultra‑low latency:
- Global C‑State Control: Disabled

---

✔ Enable fTPM (Windows 11 requirement)
BIOS → Advanced → AMD fTPM Configuration  
Manual:  
> “AMD fTPM configuration” is under Advanced → Trusted Computing. 

Set:
- fTPM: Enabled
- Secure Boot: Standard

---

✔ Boot Optimization
BIOS → Boot

Set:
- Fast Boot: Enabled  
  Manual: “Fast Boot” is listed under Boot settings. 
- POST Delay Time: 0 sec
- Boot Logo Display: Enabled

---

✔ Fan Curves (Q‑Fan Control)
BIOS → F6 Q‑Fan Control  
Manual:  
> “Select a profile… Standard, Silent, Turbo, Full Speed, Manual.”   
> “Raise fan duty to 100% if CPU exceeds 75°C.” 

Recommended:
- CPU Fan: Standard → Manual
  - 30°C → 20%
  - 50°C → 40%
  - 65°C → 70%
  - 75°C → 100%
- Case Fans: Standard

---

2️⃣ Windows 11: System Optimization

✔ Power Plan
Use AMD Ryzen Balanced:
- Best boost behavior
- Lower latency

---

✔ Disable Background Junk
Settings → System → Power & Battery → Battery Usage  
Disable:
- OneDrive auto‑sync (unless needed)
- Xbox Game Bar background recording
- Widgets

---

✔ Enable Hardware Accelerated GPU Scheduling
Settings → System → Display → Graphics → Default Graphics Settings  
Turn on:
- Hardware Accelerated GPU Scheduling
- Variable Refresh Rate

---

✔ Virtual Memory (Pagefile)
Set custom size on your Samsung 980 NVMe:
- Initial: 4096 MB
- Max: 16384 MB

---

3️⃣ NVIDIA RTX 3070: Best Settings

✔ NVIDIA Control Panel
- Power Management Mode: Prefer Maximum Performance
- Low Latency Mode: On
- Texture Filtering Quality: High Performance
- G‑Sync / FreeSync: Enabled (if monitor supports)

---

✔ DLSS / DLAA / Frame Generation
Use:
- DLSS Quality for 1440p  
- DLSS Balanced for 4K  
- DLAA for 1080p if GPU headroom exists

---

4️⃣ Storage Optimization

✔ Samsung 980 NVMe
Install Samsung Magician  
Enable:
- Rapid Mode
- Trim
- Over‑Provisioning (10%)

---

✔ Kingston A400 SATA SSD
This drive is DRAM‑less. Use it for:
- Games
- Media
- Non‑OS workloads

Avoid:
- Pagefile
- Heavy write workloads

---

5️⃣ Stability & Monitoring

✔ Install these tools
- HWiNFO64 (sensors)
- OCCT (stress testing)
- MSI Afterburner (GPU monitoring)

---

✔ Safe Temps
- CPU: 35–80°C (Ryzen 3600 throttles at 95°C)
- GPU: 40–75°C (RTX 3070 throttles at ~83°C)
- VRM: < 90°C

---

6️⃣ Optional: Light Overclocking

CPU (Ryzen 3600)
Use PBO + AutoOC instead of manual OC.

GPU (RTX 3070)
Typical stable OC:
- +120 to +150 MHz Core
- +600 to +900 MHz Memory
- Power Limit: Max

---

7️⃣ Optional: Silence‑Optimized Setup

- Enable Q‑Fan Silent for case fans  
- Keep CPU fan on Standard (never Silent)  
- Undervolt GPU using MSI Afterburner Curve Editor  
  (e.g., 1900 MHz @ 850–875 mV)

---

8️⃣ Optional: Gaming‑Focused Setup

- Disable C‑States
- Set Windows Game Mode: On
- Disable VBS / Memory Integrity
- Set NVIDIA Low Latency Mode: Ultra
- Use Fullscreen Exclusive mode in games

---

9️⃣ Optional: Creator / Productivity Setup

- Enable C‑States
- Enable Precision Boost Overdrive
- Enable Resizable BAR
- Set Windows Power Plan: Balanced
- Enable VBS / Memory Integrity

---

1️⃣0️⃣ Want me to generate a BIOS‑only optimization sheet you can print?

Choose one:

- Create BIOS‑only optimization sheet  
- Create full PC optimization PDF‑style text  
- Optimize for gaming only  
- Optimize for silence and low noise  

Just tap one and I’ll generate it.