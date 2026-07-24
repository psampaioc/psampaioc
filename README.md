# Pedro Sampaio de Camargo 👋

<p align="left">
  <img src="https://komarev.com/ghpvc/?username=psampaioc&style=flat-square&color=blueviolet" alt="profile views" />
  <img src="https://img.shields.io/badge/Location-Coimbra%2C%20Portugal-0077B5?style=flat-square" alt="location" />
  <img src="https://img.shields.io/badge/Student-University%20of%20Coimbra-004466?style=flat-square" alt="university" />
  <img src="https://img.shields.io/badge/Lab-HCMR%20%7C%20ISR--UC-FF6B35?style=flat-square" alt="lab" />
</p>

> **"Assume Breach. Hunt actively. Contain in seconds. Document everything."**

---

## 🧭 Who Am I?

Engineering student at the **University of Coimbra** (DEEC, Polo II), collaborating with the **Human-Centered Mobile Robotics Lab (HCMR)** at **ISR-UC** (Institute of Systems and Robotics).

By day: **Robotics & Systems Engineer** — ROS 2, computer vision, embedded Linux, real-time networking.  
By night (and 2023–2024): **SOC Analyst at Citadel Cyber Security (Rehovot, Israel)** — multi-tenant SIEM engineering, threat hunting, email perimeter defense, and incident response under *actual* wartime conditions.

**Personality:** Light and funny, but serious and hardworking when it matters. I believe the best defense is deep technical understanding — not buzzwords.

---

## 🛡️ Cybersecurity: The "Assume Breach" Years (2023–2024)

### **Citadel Cyber Security** — *Rehovot, Israel*
**SOC Analyst (Tier 1→3 + Consultant) | Multi-tenant MSSP defending 40+ critical infrastructure clients**

| Domain | What I Did |
|--------|------------|
| **SIEM Engineering** | Operated **5+ SIEMs simultaneously** (Splunk, Sentinel, QRadar, CrowdStrike). Wrote **SPL/KQL** detection logic daily — translated threats across query languages in minutes. |
| **Threat Hunting** | Proactive hunting via behavioral paradoxes: `svchost.exe` phoning home, service accounts running encoded PowerShell at 04:00. Built lookup tables & automated correlation funnels. |
| **Email Perimeter (SEG)** | Proofpoint & Defender for O365. Raw SMTP header forensics, sandbox detonation (ISO/IMG/XLM macros), lookalike domain takedowns via SPF/DKIM/DMARC enforcement. |
| **Endpoint Containment** | Remote EDR shell forensics — process trees, memory dumps, network isolation. **Owner from alert → investigation → client report → remediation rule.** |
| **CTI Integration** | Daily parsing of gov/industry intel feeds → IoC extraction → dynamic watchlist injection with false-positive stress testing against 30-day log history. |
| **CrowdStrike Outage (19/07/2024)** | Live incident: coordinated containment & recovery across fleet when the sensor *became* the threat. |

**Philosophy forged there:**  
> *MTTD and MTTC are the only metrics that matter. Dwell time in seconds, not days. The attacker is already inside — your job is to make their stay expensive and short.*

---

## 🤖 Robotics & Systems: Current Focus

### **HCMR Lab / ISR-UC** — *Coimbra, Portugal*
Building autonomous marine/airborne perception stacks — where robotics meets real-world uncertainty.

| Project | Stack | Highlights |
|---------|-------|------------|
| **`connectivity_check`** | ROS 2 Jazzy, C++17, nl80211 netlink, raw ICMP sockets | Single-node RSSI + ping monitor. Zero custom msgs, zero YAML, zero launch files. `CAP_NET_RAW` + `CAP_NET_ADMIN` + `--net=host`. |
| **`video_ws`** | ROS 2, OpenCV, ONNX Runtime (CUDA/CPU), CRNN + CTC decode | Unified vision node: HDMI capture → ROI crop → OCR telemetry → JSON pub. Zero-copy, event-driven. |
| **`AEGIS`** | Python, Ollama, SQLite WAL, `subprocess` sandboxing | Local AI orchestrator for 8GB VRAM: affinity scheduling (group by model), VRAM kill-switch (`torch.cuda.synchronize()`), CWD-isolated code execution, async HITL approval. |

**Hardware side:** Private PCB/KiCad repo for a company collaboration — analog front-ends, power integrity, DFM-ready layouts.

---

## 🧰 Technical Toolbox

```text
Languages:       C/C++17  •  Python  •  Bash  •  SPL/KQL/SQL  •  CMake
Robotics:        ROS 2 (Jazzy/Humble)  •  DDS/RTPS  •  composable nodes  •  ament_cmake
Computer Vision: OpenCV  •  ONNX Runtime  •  CRNN/OCR  •  V4L2  •  GStreamer
Networking:      nl80211/netlink  •  raw sockets (ICMP/TCP/UDP)  •  ModemManager  •  DDS discovery
Containers:      Docker (--net=host --ipc=host --pid=host)  •  colcon in-container  •  capability management
SIEM/SEC:        Splunk (SPL)  •  Microsoft Sentinel (KQL)  •  QRadar  •  CrowdStrike  •  Proofpoint
Infra/Linux:     systemd  •  udev  •  capabilities(7)  •  netfilter/iptables  •  realtime scheduling
Hardware:        KiCad  •  STM32/ESP32  •  PCB design (signal/power integrity)  •  JTAG/SWD debug
```

---

## 📂 Featured Repositories

| Repo | Description | Stack |
|------|-------------|-------|
| [`ROS2_Conectivity_Check`](https://github.com/psampaioc/ROS2_Conectivity_Check) | Minimal RSSI + ICMP monitor — single binary, hardcoded config, 1Hz log line | C++17, ROS 2, nl80211, raw ICMP |
| [`video_ws`](https://github.com/psampaioc/video_ws) | HDMI → ROI → OCR → telemetry pipeline. V1 (modular) → V2 (unified, zero-copy) | C++, ROS 2, ONNX, OpenCV |
| [`AEGIS`](https://github.com/psampaioc/AEGIS) | Local LLM orchestrator: VRAM-aware scheduling, sandboxed exec, async HITL | Python, Ollama, SQLite WAL |
| [`Programa-de-Gestao-de-Condominios`](https://github.com/psampaioc/Programa-de-Gestao-de-Condominios) | C++ console app — fractions, condominiums, expenses, movements (Data Structures course) | C++17, STL, file I/O |

> 🔒 *Private repo: PCB/KiCad hardware design for industry partner*

---

## 📜 Writing & Talks

- **["Cibersegurança: Minha Perspectiva Prática"](https://github.com/psampaioc/psampaioc/blob/main/Ciberseguranca_by_Pedro_Sampaio.pdf)** — 9-part field manual from the Citadel trenches (SIEM, SEG, hunting, governance, CrowdStrike outage, developer paradox). *Portuguese, June 2024.*
- **GitHub Profile README** — You're reading it. Built to be useful, not just pretty.

---

## 🎯 What I'm Looking For

- **Robotics/Autonomy R&D** — perception, localization, multi-agent systems, marine/airborne platforms
- **Security Engineering** — detection engineering, SIEM architecture, endpoint hardening, DevSecOps
- **Embedded Linux / Real-time Systems** — Yocto, PREEMPT_RT, capability-based sandboxing
- **Technical Leadership** — bridging the "developer vs. security" paradox with empathy and tooling

---

## 🌐 Connect

<p align="left">
  <a href="https://www.linkedin.com/in/pedro-camargo-cyber/">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:cyberpedrosecurity@proton.me">
    <img src="https://img.shields.io/badge/Email-8B0000?style=for-the-badge&logo=protonmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://github.com/psampaioc">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
</p>

---

## 📊 GitHub Pulse

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=psampaioc&show_icons=true&count_private=true&theme=tokyonight&hide_border=true&custom_title=Pedro's%20GitHub%20Stats" height="165" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=psampaioc&layout=compact&theme=tokyonight&hide_border=true&custom_title=Top%20Languages" height="165" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com/?user=psampaioc&theme=tokyonight&mode=weekly&hide_border=true" height="165" />
</p>

---

<details>
<summary><b>🎲 Fun Facts / Easter Eggs</b></summary>

- My home lab started in **Cisco Packet Tracer** + VMs on a laptop that froze at 4 VMs — taught me Linux resource discipline the hard way.
- Learned offensive security on **TryHackMe/Hack The Box** to become a better defender (reverse-engineering the kill chain).
- Served in the **IDF** (2020–2023) — discipline under stress, "Tachles" mindset: cut bureaucracy, solve the problem.
- The `connectivity_check` node runs on my robot's Raspberry Pi — it texts me when WiFi drops below -80 dBm.
- I write detection rules like I write code: **tested against 30 days of history**, version-controlled, peer-reviewed.
- Coffee preference: **Portuguese bica** (espresso) — no sugar, no milk, just pure extraction.

</details>

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,4,6,8,10,12,14,16,18,20,22,24,26,28,30&height=100&section=footer&animation=twinkling" />
</p>

<p align="center">
  <sub>Built with ❤️, C++, Python, and a healthy dose of <code>Assume Breach</code>.<br>
  © 2025 Pedro Sampaio de Camargo — <a href="https://github.com/psampaioc">psampaioc</a></sub>
</p>
