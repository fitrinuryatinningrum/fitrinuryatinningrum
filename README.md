<div align="center">

# Fitri Nuryatin Ningrum

**Mechatronics Engineering — Control Systems · Embedded · IoT · AI Agents**

Building systems that sense, decide, and act — from the control model
all the way down to firmware on real hardware.

[![Profile](https://img.shields.io/badge/Profile-fitrinuryatinningrum-2F81F7?style=flat-square&labelColor=24292F&logo=github)](https://github.com/fitrinuryatinningrum)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-fitrinuryatinningrum-0A66C2?style=flat-square&labelColor=24292F&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/fitri-nuryatin-ningrum-356575377)
[![Email](https://img.shields.io/badge/Email-fitrinuryatinningrum@gmail.com-EA4335?style=flat-square&labelColor=24292F&logo=gmail&logoColor=white)](mailto:fitrinuryatinningrum@gmail.com)

[About](#about) · [Skills](#skills) · [Projects](#projects) · [Roadmap](#roadmap) · [Activity](#activity) · [Stats](#stats) · [Contact](#contact)

</div>

---

<a name="about"></a>

## About

I work across the full stack of mechatronics — the discipline where control theory,
firmware, and connected systems meet.

**Control systems.** System modeling, PID design, frequency response, and stability
analysis — translating plant behaviour into a control law that actually converges.

**Embedded systems.** Real-time firmware on ESP32 and STM32: sensor acquisition,
actuator control, and the timing problems that never appear in simulation.

**IoT.** Connected sensor networks over MQTT and REST, with remote telemetry and
alerting.

**AI agents.** Autonomous agents built on [Hermes Agent](https://github.com/NousResearch/hermes-agent)
from Nous Research — systems that call tools, run scheduled work, and retain context
across sessions.

What I value most is the full loop: derive the model, simulate it, build it, watch it
fail on the bench, and find out why.

<details>
<summary><b>Current focus — IoT temperature control with Sugeno fuzzy inference</b></summary>

<br>

A system that prevents **router overheating** by reading a DHT sensor and letting a
*Sugeno fuzzy inference engine* select the cooling action — rather than fixed
`if temp > 40` thresholds, using rules that handle ambiguous real-world conditions
gracefully.

```
Temperature error (ΔT)  +  Rate of change (dT/dt)
        │
        ▼
   Fuzzy Inference (Sugeno)
        │
        ▼
   Defuzzification  →  PWM fan output
```

- Membership functions across cold / normal / warm / hot
- Rule base encoding operator reasoning — *hot **and** rising fast → full output*
- Weighted-average defuzzification
- MQTT telemetry with Telegram alerting on dangerous thresholds

**Status:** in progress

</details>

---

<a name="skills"></a>

## Skills

Self-assessed proficiency. Percentages reflect working familiarity, not certification.

**Scale** — `80–100%` proficient · `50–79%` competent · `25–49%` developing · `<25%` introductory

### Control & Automation

| Skill | Level | |
|---|:---:|:---:|
| PID Tuning & Design | ![](https://img.shields.io/badge/-80%25-3FB950?style=flat-square&labelColor=24292F) | 80% |
| Fuzzy Logic (Sugeno / Mamdani) | ![](https://img.shields.io/badge/-85%25-3FB950?style=flat-square&labelColor=24292F) | 85% |
| MATLAB / Simulink | ![](https://img.shields.io/badge/-55%25-D29922?style=flat-square&labelColor=24292F) | 55% |

### Embedded & Real-Time

| Skill | Level | |
|---|:---:|:---:|
| Microcontroller Firmware (ESP32) | ![](https://img.shields.io/badge/-90%25-3FB950?style=flat-square&labelColor=24292F) | 90% |
| PCB Design (KiCad) | ![](https://img.shields.io/badge/-90%25-3FB950?style=flat-square&labelColor=24292F) | 90% |
| Communication Buses (I2C / SPI / UART / CAN) | ![](https://img.shields.io/badge/-80%25-3FB950?style=flat-square&labelColor=24292F) | 80% |
| C / C++ | ![](https://img.shields.io/badge/-70%25-D29922?style=flat-square&labelColor=24292F) | 70% |

### IoT & Connectivity

| Skill | Level | |
|---|:---:|:---:|
| Telegram Bot Integration | ![](https://img.shields.io/badge/-98%25-3FB950?style=flat-square&labelColor=24292F) | 98% |
| Wireless (ESP-NOW / Wi-Fi / BLE) | ![](https://img.shields.io/badge/-80%25-3FB950?style=flat-square&labelColor=24292F) | 80% |
| REST API / JSON | ![](https://img.shields.io/badge/-80%25-3FB950?style=flat-square&labelColor=24292F) | 80% |
| MQTT & Broker | ![](https://img.shields.io/badge/-70%25-D29922?style=flat-square&labelColor=24292F) | 70% |

### AI & Autonomous Agents

| Skill | Level | |
|---|:---:|:---:|
| Hermes Agent (Nous Research) | ![](https://img.shields.io/badge/-95%25-3FB950?style=flat-square&labelColor=24292F) | 95% |
| Python | ![](https://img.shields.io/badge/-70%25-D29922?style=flat-square&labelColor=24292F) | 70% |
| Prompt Engineering | ![](https://img.shields.io/badge/-60%25-D29922?style=flat-square&labelColor=24292F) | 60% |

### Currently Learning

Kept separate so the numbers stay honest — these are areas I have only just started.

| Skill | Level |
|---|:---:|
| System Modeling & Transfer Function | ![](https://img.shields.io/badge/-15%25-F85149?style=flat-square&labelColor=24292F) |
| State-Space & Stability Analysis | ![](https://img.shields.io/badge/-10%25-F85149?style=flat-square&labelColor=24292F) |
| Dashboard & Telemetry | ![](https://img.shields.io/badge/-10%25-F85149?style=flat-square&labelColor=24292F) |
| LLM Tool Use / Function Calling | ![](https://img.shields.io/badge/-10%25-F85149?style=flat-square&labelColor=24292F) |
| MCP (Model Context Protocol) | ![](https://img.shields.io/badge/-5%25-F85149?style=flat-square&labelColor=24292F) |
| FreeRTOS | ![](https://img.shields.io/badge/-5%25-F85149?style=flat-square&labelColor=24292F) |

### Toolchain

[![Skills](https://skillicons.dev/icons?i=matlab,python,c,cpp,arduino,raspberrypi,nodejs,js,ts,html,css,git,github,vscode,kicad,linux,docker,mqtt,postman)](https://skillicons.dev)

<table>
<tr>
<td valign="top" width="50%">

**Control & Simulation**

![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=flat-square&labelColor=24292F&logo=mathworks&logoColor=white)
![Simulink](https://img.shields.io/badge/Simulink-0076A8?style=flat-square&labelColor=24292F&logo=mathworks&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&labelColor=24292F&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&labelColor=24292F&logo=jupyter&logoColor=white)
![Octave](https://img.shields.io/badge/Octave-079393?style=flat-square&labelColor=24292F&logo=gnu-octave&logoColor=white)

`PID Tuning` · `Fuzzy Logic (Sugeno, Mamdani)` · `Frequency Response` ·
`SISO/MIMO` · `Sampling & Discrete Control`
<br><sub>Learning: `Transfer Function` · `State-Space` · `Stability Analysis`</sub>

</td>
<td valign="top" width="50%">

**Embedded & Hardware**

![C](https://img.shields.io/badge/C-00599C?style=flat-square&labelColor=24292F&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&labelColor=24292F&logo=c%2B%2B&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=flat-square&labelColor=24292F&logo=arduino&logoColor=white)
![ESP32](https://img.shields.io/badge/ESP32-3C8B4C?style=flat-square&labelColor=24292F&logo=espressif&logoColor=white)
![STM32](https://img.shields.io/badge/STM32-03234B?style=flat-square&labelColor=24292F&logo=stmicroelectronics&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-C51A4A?style=flat-square&labelColor=24292F&logo=raspberrypi&logoColor=white)
![PlatformIO](https://img.shields.io/badge/PlatformIO-ED7D31?style=flat-square&labelColor=24292F&logo=platformio&logoColor=white)

`I2C / SPI / UART / CAN` · `PWM & Motor Control` · `Interrupts & Timers` ·
`ADC / DAC` · `PCB Design (KiCad)` · `Fritzing`
<br><sub>Learning: `FreeRTOS`</sub>

</td>
</tr>
<tr>
<td valign="top" width="50%">

**IoT & Connectivity**

![MQTT](https://img.shields.io/badge/MQTT-660066?style=flat-square&labelColor=24292F&logo=mqtt&logoColor=white)
![Node-RED](https://img.shields.io/badge/Node-RED-8F03D8?style=flat-square&labelColor=24292F&logo=nodered&logoColor=white)
![Mosquitto](https://img.shields.io/badge/Mosquitto-660066?style=flat-square&labelColor=24292F&logo=mosquitto&logoColor=white)
![Telegram](https://img.shields.io/badge/Telegram%20Bot-26A5E4?style=flat-square&labelColor=24292F&logo=telegram&logoColor=white)
![Web Serial](https://img.shields.io/badge/Web%20Serial-4285F4?style=flat-square&labelColor=24292F&logo=google&logoColor=white)

`ESP-NOW` · `Wi-Fi / BLE` · `ThingSpeak` · `REST APIs` · `Telegram Bot API`
<br><sub>Learning: `InfluxDB` · `Grafana` · `Telemetry Dashboards`</sub>

</td>
<td valign="top" width="50%">

**AI & Autonomous Agents**

[![Hermes](https://img.shields.io/badge/Hermes%20Agent-5A4FCF?style=flat-square&labelColor=24292F&logo=NousResearch&logoColor=white)](https://github.com/NousResearch/hermes-agent)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&labelColor=24292F&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&labelColor=24292F&logo=typescript&logoColor=white)

**Hermes Agent** — a self-improving autonomous agent with a built-in learning loop:
it creates skills from experience, refines them through use, and searches its own
past conversations for context.
<br>`Scheduled Automations` · `Subagent Delegation` · `Session Memory` · `Agent ↔ Hardware`
<br><sub>Learning: `Tool Use / Function Calling` · `MCP`</sub>

</td>
</tr>
<tr>
<td valign="top" width="50%">

**Tools**

![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&labelColor=24292F&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&labelColor=24292F&logo=github&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=flat-square&labelColor=24292F&logo=visualstudiocode&logoColor=white)
![KiCad](https://img.shields.io/badge/KiCad-005E87?style=flat-square&labelColor=24292F&logo=kicad&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&labelColor=24292F&logo=linux&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&labelColor=24292F&logo=postman&logoColor=white)

`Git` · `GitHub Actions` · `Docker` · `Linux CLI` · `Oscilloscope` ·
`Multimeter` · `Logic Analyzer`

</td>
<td valign="top" width="50%">

**Frontend**

![HTML](https://img.shields.io/badge/HTML-E34F26?style=flat-square&labelColor=24292F&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-1572B6?style=flat-square&labelColor=24292F&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&labelColor=24292F&logo=javascript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&labelColor=24292F&logo=nodedotjs&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&labelColor=24292F&logo=react&logoColor=white)

`Responsive UI` · `SVG Visualization` · `Data Dashboards` · `Single-File Applications`

</td>
</tr>
</table>

---

<a name="projects"></a>

## Projects

### Component Classification — AC & DC

[![Repository](https://img.shields.io/badge/Repository-component--classification-2F81F7?style=flat-square&labelColor=24292F&logo=github&logoColor=white)](https://github.com/fitrinuryatinningrum/component-classification)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&labelColor=24292F&logo=javascript&logoColor=white)](https://github.com/fitrinuryatinningrum/component-classification)

An interactive web application for learning electronic component classification —
**94 components**, **94 vector symbols**, and **5 quiz modes**, fully offline.
Shipped as a self-contained single-file build that runs by double-click, with no
server and no dependencies.

`Interactive Web App` · `SVG Vector Graphics` · `Hash Router` · `Quiz Engine` · `Zero Dependency`

[Open repository →](https://github.com/fitrinuryatinningrum/component-classification)

### Obstacle Avoidance Robot

[![Repository](https://img.shields.io/badge/Repository-obstacle--avoiding--robot-F0883E?style=flat-square&labelColor=24292F&logo=github&logoColor=white)](https://github.com/fitrinuryatinningrum)
[![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&labelColor=24292F&logo=c%2B%2B&logoColor=white)](https://github.com/fitrinuryatinningrum)

An autonomous robot that detects obstacles and navigates around them in real time.
Ultrasonic sensing, microcontroller firmware, and closed-loop motor control — where
embedded code meets control theory.

`Ultrasonic Sensing` · `PID Motor Control` · `Real-time Firmware` · `State Machine`

### Titan-M2 CNC

[![Repository](https://img.shields.io/badge/Repository-titan--m2--cnc-A371F7?style=flat-square&labelColor=24292F&logo=github&logoColor=white)](https://github.com/fitrinuryatinningrum)
[![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&labelColor=24292F&logo=c%2B%2B&logoColor=white)](https://github.com/fitrinuryatinningrum)

A computer numerical control project — precision stepper motion for automated
machining. This is where mechatronics converges: kinematics, step generation, timing,
and machine accuracy in a single system.

`Motion Control` · `Stepper Drivers` · `G-code` · `Kinematics` · `PCB & Wiring`

### IoT Temperature Control — Fuzzy Sugeno

[![Repository](https://img.shields.io/badge/Repository-iot--temperature--control-3FB950?style=flat-square&labelColor=24292F&logo=github&logoColor=white)](https://github.com/fitrinuryatinningrum)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&labelColor=24292F&logo=python&logoColor=white)](https://github.com/fitrinuryatinningrum)
[![Status](https://img.shields.io/badge/Status-In%20Progress-D29922?style=flat-square&labelColor=24292F)]()

An IoT automatic temperature control system for preventing router overheating, using
Sugeno fuzzy inference to select cooling actions — handling ambiguous real-world
conditions rather than fixed thresholds.

`Fuzzy Logic (Sugeno)` · `DHT11 / DHT22` · `MQTT` · `ESP32` · `Telegram Alerts`

<details>
<summary><b>Other repositories</b></summary>

<br>

[![Random Repo](https://github-readme-random-repo.vercel.app/api?username=fitrinuryatinningrum&count=1&theme=default&hide_border=true)](https://github.com/fitrinuryatinningrum?tab=repositories)

[Browse all repositories →](https://github.com/fitrinuryatinningrum?tab=repositories)

</details>

---

<a name="roadmap"></a>

## Roadmap

### IoT Temperature Control — Fuzzy Sugeno

| Stage | Progress | Status |
|---|:---:|:---:|
| Membership functions | ![](https://img.shields.io/badge/-50%25-D29922?style=flat-square&labelColor=24292F) | In progress |
| Sugeno rule base | ![](https://img.shields.io/badge/-35%25-2F81F7?style=flat-square&labelColor=24292F) | In progress |
| Defuzzification & ESP32 integration | ![](https://img.shields.io/badge/-10%25-F85149?style=flat-square&labelColor=24292F) | Next |
| MQTT telemetry & alerting | ![](https://img.shields.io/badge/Not%20started%20-%20-F85149?style=flat-square&labelColor=24292F) | Planned |
| Validation on target router hardware | ![](https://img.shields.io/badge/Not%20started%20-%20-F85149?style=flat-square&labelColor=24292F) | Planned |

### AI Agent Engineering

| Item | Progress | Status |
|---|:---:|:---:|
| Hermes CLI & gateway setup | ![](https://img.shields.io/badge/Complete-3FB950?style=flat-square&labelColor=24292F) | Done |
| Custom skill creation | ![](https://img.shields.io/badge/-60%25-D29922?style=flat-square&labelColor=24292F) | In progress |
| Scheduled automations | ![](https://img.shields.io/badge/-45%25-2F81F7?style=flat-square&labelColor=24292F) | In progress |
| MCP server integration | ![](https://img.shields.io/badge/-30%25-2F81F7?style=flat-square&labelColor=24292F) | Next |
| Agent ↔ hardware bridge | ![](https://img.shields.io/badge/-15%25-F85149?style=flat-square&labelColor=24292F) | Exploring |

### Advanced Control Systems

| Item | Progress | Status |
|---|:---:|:---:|
| State estimators & observers | ![](https://img.shields.io/badge/-25%25-2F81F7?style=flat-square&labelColor=24292F) | Studying |
| LQR & optimal control | ![](https://img.shields.io/badge/-15%25-F85149?style=flat-square&labelColor=24292F) | Studying |
| Adaptive & self-tuning control | ![](https://img.shields.io/badge/Not%20started%20-%20-F85149?style=flat-square&labelColor=24292F) | Planned |

---

<a name="activity"></a>

## Activity

Contribution graph, rendered as an animated snake. Regenerated automatically by
GitHub Actions every six hours.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Platane/snk/output/github-contribution-grid-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Platane/snk/output/github-contribution-grid-snake.svg">
  <img src="https://raw.githubusercontent.com/Platane/snk/output/github-contribution-grid-snake.svg"
       alt="Contribution activity"
       width="100%" />
</picture>

---

<a name="stats"></a>

## GitHub Stats

<div align="center">

[![Statistics](https://github-readme-stats.vercel.app/api?username=fitrinuryatinningrum&show_icons=true&theme=default&hide_border=true&include_all_commits=true&count_private=true&bg_color=24292F&title_color=2F81F7&text_color=C9D1D9&icon_color=8B949E&ring_color=2F81F7)](https://github.com/fitrinuryatinningrum)

[![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=fitrinuryatinningrum&layout=compact&theme=default&hide_border=true&bg_color=24292F&title_color=2F81F7&text_color=C9D1D9)](https://github.com/fitrinuryatinningrum)

[![Contribution Streak](https://streak-stats.demolab.com?user=fitrinuryatinningrum&theme=default&hide_border=true&background_color=24292F)](https://git.io/streak-stats)

[![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=fitrinuryatinningrum&theme=github-compact&hide_border=true&area=true&bg_color=24292F)](https://github.com/fitrinuryatinningrum)

[![Trophies](https://github-profile-trophy.vercel.app/?username=fitrinuryatinningrum&theme=dark&column=7&margin-w=8&margin-h=8&no-frame=true&no-bg=true&no-bg=true)](https://github.com/fitrinuryatinningrum)

</div>

---

<a name="contact"></a>

## Contact

[![GitHub](https://img.shields.io/badge/GitHub-fitrinuryatinningrum-181717?style=flat-square&labelColor=24292F&logo=github&logoColor=white)](https://github.com/fitrinuryatinningrum)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-fitrinuryatinningrum-0A66C2?style=flat-square&labelColor=24292F&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/fitri-nuryatin-ningrum-356575377)
[![Email](https://img.shields.io/badge/Email-fitrinuryatinningrum@gmail.com-EA4335?style=flat-square&labelColor=24292F&logo=gmail&logoColor=white)](mailto:fitrinuryatinningrum@gmail.com)

Open to collaboration on embedded, control, and agent-based projects, and to
interesting open-source issues.

---

<div align="center">

[![Profile Views](https://komarev.com/ghpvc/?username=fitrinuryatinningrum&label=Profile%20Views&color=2F81F7&style=flat)](https://github.com/fitrinuryatinningrum)
[![Followers](https://img.shields.io/github/followers/fitrinuryatinningrum?style=flat-square&labelColor=24292F&logo=github&logoColor=white)](https://github.com/fitrinuryatinningrum)
[![Repos](https://img.shields.io/github/repos/fitrinuryatinningrum?style=flat-square&labelColor=24292F&logo=github&logoColor=white)](https://github.com/fitrinuryatinningrum?tab=repositories)

*Built with care for machines that think.*

</div>

<!--
============================================================
  CUSTOMIZATION NOTES — read, edit, then delete this block
============================================================

1. SKILL PERCENTAGES — "Skills" section
   Each row has ONE number: inside the badge URL
   https://img.shields.io/badge/-80%25-3FB950
                       ^^^^^ replace both number and colour
   Colour scale:
     3FB950 green  = 80–100%  proficient
     D29922 amber  = 50–79%   competent
     2F81F7 blue   = 25–49%   developing
     F85149 red    =  0–24%   introductory
   No separate percentage column is needed — the badge is the value.

2. ROADMAP PROGRESS — "Roadmap" section
   Same single-number rule. For untouched items replace the value with:
   https://img.shields.io/badge/Not%20started%20-%20-F85149

3. STILL TO COMPLETE
   • Obstacle Avoiding Robot + Titan-M2 CNC cards point to the profile
     root. Replace with their real repository URLs once published:
       obstacle-avoiding-robot  → https://github.com/<user>/<repo>
       titan-m2-cnc             → https://github.com/<user>/<repo>
     Also update the two Repository badges in those cards.
   • LinkedIn URL is already set (fitri-nuryatin-ningrum-356575377).

4. THEME
   • Stats cards use an explicit dark background (bg_color=24292F)
     so they read cleanly on both light and dark GitHub themes.
     To go light-mode native, remove the bg_color / text_color params.
   • Snake animation needs .github/workflows/snake.yml to have run at
     least once (Actions → snake.yml → Run workflow). It is inactive
     until then.

5. STATS CACHE
   • Cards are cached by GitHub and may render blank for the first
     few minutes after an edit. Hard reload before assuming breakage.
============================================================
-->