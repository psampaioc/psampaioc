# Pedro Sampaio de Camargo 👋

<p align="left">
  <img src="https://komarev.com/ghpvc/?username=psampaioc&style=flat-square&color=blueviolet" alt="profile views" />
  <img src="https://img.shields.io/badge/Location-Coimbra%2C%20Portugal-0077B5?style=flat-square" alt="location" />
  <img src="https://img.shields.io/badge/Student-University%20of%20Coimbra-004466?style=flat-square" alt="university" />
  <img src="https://img.shields.io/badge/Lab-HCMR%20%7C%20ISR--UC-FF6B35?style=flat-square" alt="lab" />
</p>

> **Researcher. Strategist. Builder. Document everything.**

---

## Who Am I?

Engineering student at the **University of Coimbra** (FCTUC, DEEC, Polo II), collaborating with the **Human-Centered Mobile Robotics Lab (HCMR)** at **ISR-UC** (Institute of Systems and Robotics).

After managing high-risk environments as a military commander and cybersecurity analyst, I transitioned to the root of technology development. Today, at the University of Coimbra and the Institute of Systems and Robotics (ISR), I develop the hardware and edge computing architectures that power autonomous robots and agentic AI.
My end goal is to use the knowledge of physical engineering to actively lead the next technological revolution: the integration of humans and machines.

I am driven by practical execution, a first-principles approach to complex problem-solving, and the conviction that technology must elevate human capacity. I am equally passionate about connecting with those who are pushing the absolute limits of robotics with dedication. Let's connect and build what comes next.
**Personality:** Light and funny, but serious and hardworking when it matters. I believe the best defense is deep technical understanding — not buzzwords.

---

## 🎯 What I'm Looking For

- **Robotics/Autonomy R&D** — perception, localization, multi-agent systems, land/airborne platforms
- **Security Engineering** — detection engineering, SIEM rules, endpoint hardening, DevSecOps
- **Embedded Linux / Real-time Systems** — 
- **Technical Leadership** — bridging the "developer vs. security" paradox with empathy and tooling

---

## Tech Stack

Languages:       C/C++  •  Python  •  Bash  •  SPL/KQL/SQL  •  CMake
Robotics:        ROS 2 (Jazzy/Humble)  •  DDS/RTPS  •  composable nodes  •  ament_cmake
Computer Vision: OpenCV  •  ONNX Runtime  •  CRNN/OCR  •  V4L2
Networking:      nl80211/netlink  •  raw sockets (ICMP/TCP/UDP)  • DDS discovery
Containers:      Docker (--net=host --ipc=host --pid=host)  • capability management
SIEM/SEC:        Splunk (SPL)  •  Microsoft Sentinel (KQL)  •  QRadar  •  CrowdStrike  •  Proofpoint
Infra/Linux:     systemd  •  iptables  
Hardware:        KiCad  •  STM32/ESP32  •  PCB design (signal/power integrity)

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
| **CrowdStrike Outage (19/07/2024)** | Live incident: Recovery across fleet when the sensor *became* the threat. |

**Philosophy forged there:**  
> *MTTD and MTTC metrics: Dwell time in seconds, not days. The attacker is already inside — our job is to make their stay expensive and short.*

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

- **["Cibersegurança: Minha Perspectiva Prática"](https://github.com/psampaioc/psampaioc/blob/main/Ciberseguranca_by_Pedro_Sampaio.pdf)** — 9-part field report from the Citadel trenches (SIEM, SEG, hunting, governance, CrowdStrike outage, developer paradox). *Portuguese, June 2024.*
- **GitHub Profile README** — You're reading it. Built to be useful, not just pretty.

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

- My cyber home lab started in **Cisco Packet Tracer** + VMs on a laptop that froze at 4 VMs — taught me resource discipline the hard way.
- Learned offensive security on **TryHackMe/Hack The Box** to become a better defender (reverse-engineering the kill chain).
- Served in the **IDF** (2020–2023) — discipline under stress, "Tachles" mindset: cut bureaucracy, solve the problem.
- I write detection rules like I write code: **stress-tested**, version-controlled, peer-reviewed.
- Practice sports everyday, yet sometimes daydreaming about the end of year snowboard trip to come!

</details>

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,4,6,8,10,12,14,16,18,20,22,24,26,28,30&height=100&section=footer&animation=twinkling" />
</p>

<p align="center">
  <sub>Built with excitement, C++, Python, and a lot of work.<br>
  © 2025 Pedro Sampaio de Camargo — <a href="https://github.com/psampaioc">psampaioc</a></sub>
</p>
