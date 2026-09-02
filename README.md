<h1 align="center">Hi, I'm Saransh 👋</h1>

<p align="center">
  Engineering student who builds systems end to end — from the sensor on the board to the dashboard in the browser.
</p>

<p align="center">
  <a href="mailto:codeaxis048@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <img src="https://komarev.com/ghpvc/?username=Saransh1120&style=for-the-badge&color=blue" />
</p>

---

### About me

- 🎯 Grinding **DSA in C++** — one commit a day, no skipped days
- 🌱 Moving toward **full-stack web development** (TypeScript, React, Node)
- 🔧 I build real hardware too: ESP32 firmware, I2C sensor stacks, custom PCBs on perfboard
- ⚡ I like problems where the software has to survive contact with the physical world

---

## 🚀 Featured projects

### 🫁 RespiGuard — a chest-worn asthma early-warning monitor

Most wearables scream at you the moment a number crosses a textbook threshold.
RespiGuard doesn't. It spends its first days **learning your own baseline** for
SpO₂, breathing rate and heart rate, and only raises an alert when those drift
away from *your* normal **while a wheeze classifier is firing at the same time**.

The part I'm proudest of is the **exertion veto**: if the IMU says you're moving
hard and there's no wheeze in the audio, the score is pushed back down. Climbing
stairs should not look like an asthma attack, and on most devices it does.

- **Hardware:** ESP32-S3 · MAX30102 pulse oximeter · INMP441 I2S mic · BMI270 IMU · BME680 · SSD1306 OLED · Li-Po with buck-boost rail
- **Detection:** weighted deviation scoring across four signals, OK → WATCH → ALERT with a hold window so the display doesn't flicker
- **ML:** wheeze classifier trained on the ICBHI 2017 Respiratory Sound Database (920 recordings, 126 patients)
- **Status:** logic proven in a Wokwi simulation, hardware self-test firmware written, board being hand-soldered

`C++` `Arduino` `ESP32-S3` `I2C / I2S` `Python` `Signal processing`

---

### 🔐 Mohar — sealed custody chain for examination papers

India has had **148 exam-paper leak cases since 2015 and one conviction.** That
gap is not a detection problem, it's an *evidentiary* one — nobody can prove who
touched the paper and when. Mohar is my attempt at the boring infrastructure
that closes it.

Three goals, and I deliberately refused a fourth:

1. Shrink the **exposure window** — how long a paper exists in readable form — from roughly 240 hours down to under one.
2. Make every leak **attributable** to a centre, and where possible a single seat, within minutes of an image surfacing online.
3. Produce a **court-admissible** custody record, not just an internal log.

**Non-goal: pretending leaks can be eliminated.** A human has to read the paper
at some point. Mohar shrinks and instruments those points instead of promising
the impossible — that honesty is a design feature, not a weakness.

- **Backend:** TypeScript · Fastify · PostgreSQL, with a hash-chained append-only ledger
- **Frontend:** control-room dashboard, public verify portal, centre client, Android field app
- **Hardware:** ESP32 room-monitor firmware — tamper and environment telemetry from inside the strongroom
- **Structure:** pnpm monorepo — `services/` `apps/` `packages/` `firmware/` `infra/`

`TypeScript` `Fastify` `PostgreSQL` `React` `Cryptography` `ESP32` `Monorepo`

---

### 📘 c--dsapw — Data structures & algorithms in C++

My daily practice log. Conditionals, loops, patterns, and every DSA topic as I
work through it — committed the same day I solve it. Not polished, deliberately:
it's a record of the reps, not a portfolio piece.

`C++`

---

## 🛠️ Tech I work with

**Languages**

![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

**Frameworks & tools**

![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=arduino&logoColor=white)
![Espressif](https://img.shields.io/badge/ESP32-E7352C?style=for-the-badge&logo=espressif&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)

---

## 📊 GitHub stats

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=Saransh1120&show_icons=true&theme=tokyonight&hide_border=true" />
  <img height="165" src="https://github-readme-streak-stats.herokuapp.com/?user=Saransh1120&theme=tokyonight&hide_border=true" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Saransh1120&layout=compact&theme=tokyonight&hide_border=true" />
</p>

---

<p align="center">
  <i>Consistency beats intensity. Show up, commit, repeat.</i>
</p>
