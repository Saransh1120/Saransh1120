<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=200&section=header&text=Saransh&fontSize=70&fontColor=ffffff&animation=fadeIn&fontAlignY=35&desc=hardware%20%C2%B7%20software%20%C2%B7%20everything%20in%20between&descAlignY=55&descSize=18" />

<p align="center">
  <a href="https://github.com/Saransh1120">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&duration=3000&pause=800&color=4EC9B0&center=true&vCenter=true&width=520&lines=C%2B%2B+and+DSA%2C+every+single+day;Building+Mohar+and+RespiGuard;IoT%2C+sensors+and+drones;Learning+full-stack%2C+one+bug+at+a+time" />
  </a>
</p>

<p align="center">
  <a href="mailto:sargarbhit19@gmail.com"><img src="https://img.shields.io/badge/GMAIL-c14438?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://github.com/Saransh1120?tab=repositories"><img src="https://img.shields.io/badge/PROJECTS-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
  <img src="https://komarev.com/ghpvc/?username=Saransh1120&style=for-the-badge&color=2c5364&label=VISITORS" />
</p>

<br>

## About

Engineering student. I mostly build things that sit between hardware and software,
because that's where the interesting bugs are.

Right now I'm doing DSA in C++ every day and pushing whatever I solve the same
day. Slowly moving into full-stack web work (TypeScript, React, Node) since
that's where I want to end up. My two main projects are Mohar and RespiGuard.

I've also done IoT work with sensors and microcontrollers, and a three day drone
workshop at Sharda University where we assembled a quadcopter from parts and
took it up to basic autonomy.

<br>

## Projects

### RespiGuard

A chest-worn asthma monitor. Most wearables alert you the second a number crosses
some textbook threshold, which is useless because everyone's normal is different.
RespiGuard spends its first few days learning your own baseline for SpO2,
breathing rate and heart rate, and only alerts when those drift away from your
normal *and* a wheeze classifier is firing at the same time.

The bit I like most is the exertion veto. If the IMU says you're moving hard and
there's no wheeze in the audio, the score gets pushed back down. Climbing stairs
shouldn't look like an asthma attack, and on most devices it does.

Built on an ESP32-S3 with a MAX30102 pulse oximeter, an INMP441 mic, a BMI270
IMU, a BME680, and a small OLED. Detection is a weighted deviation score across
four signals, going OK to WATCH to ALERT with a hold so the screen doesn't
flicker. The wheeze model trains on the ICBHI 2017 respiratory sound database.

Logic is proven in simulation and the self-test firmware is written. The board is
still being hand-soldered, so nothing has run on real hardware yet.

<p>
  <img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white" />
  <img src="https://img.shields.io/badge/ESP32--S3-E7352C?style=flat-square&logo=espressif&logoColor=white" />
  <img src="https://img.shields.io/badge/Arduino-00979D?style=flat-square&logo=arduino&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
</p>

### Mohar

Exam paper leaks in India: 148 cases since 2015, one conviction. That gap isn't
really a detection problem, it's an evidence problem. Nobody can prove who
touched the paper and when.

Mohar is a custody chain for exam papers. Three things it tries to do: cut the
window where a paper exists in readable form from around 240 hours to under one,
make any leak traceable back to a centre and ideally a seat within minutes of an
image showing up, and produce a custody record that would actually hold up in
court.

What it does not do is claim leaks can be stopped completely. A human has to read
the paper eventually. So the goal is to shrink and instrument those moments
instead of promising something impossible.

Backend is TypeScript, Fastify and Postgres with a hash-chained append-only
ledger. On top of that there's a control room dashboard, a public verify portal,
a centre client and an Android field app. There's also ESP32 firmware for a room
monitor that reports tamper and environment data from inside the strongroom.

<p>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/Fastify-000000?style=flat-square&logo=fastify&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black" />
</p>

### LPG gas detector

A college IoT project I led. An MQ-2 sensor sits watching the air and feeds an analog
reading into an Arduino Uno. Below the threshold nothing happens. The moment LPG
concentration crosses it, the buzzer goes off and the LEDs light up, so a leak in
a kitchen gets caught long before it turns into a fire.

Nothing fancy in it, but it's the project that got me comfortable with reading a
sensor, picking a sane threshold and driving outputs off it.

Arduino Uno, MQ-2 module, piezo buzzer, LED indicators, 9V supply with a toggle
switch.

<p>
  <img src="https://img.shields.io/badge/Arduino%20Uno-00979D?style=flat-square&logo=arduino&logoColor=white" />
  <img src="https://img.shields.io/badge/MQ--2%20sensor-555555?style=flat-square" />
  <img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white" />
</p>

### Drone workshop

Three days at Sharda University with the AI and Robotics Club, "From Assembly to
Autonomy". We built a quadcopter from the frame up: motors, ESCs, flight
controller, radio link, props, then calibration and flight. Seeing how much of it
is tuning rather than building was the useful part.

### c--dsapw

My daily C++ practice. Conditionals, loops, patterns, and whatever DSA topic I'm
on. It's messy on purpose. It's a log of the reps, not a portfolio piece.

<br>

## Stuff I use

<p>
  <img src="https://skillicons.dev/icons?i=cpp,java,ts,js,python,react,nodejs,postgres,arduino,git,vscode&theme=dark" />
</p>

<br>

## Stats

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=Saransh1120&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=4EC9B0&icon_color=4EC9B0" />
  <img height="165" src="https://github-readme-streak-stats.herokuapp.com/?user=Saransh1120&theme=github-dark-blue&hide_border=true&background=0d1117&ring=4EC9B0&fire=4EC9B0&currStreakLabel=4EC9B0" />
</p>

<p align="center">
  <img height="150" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Saransh1120&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=4EC9B0" />
</p>

<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=Saransh1120&theme=darkhub&no-frame=true&no-bg=true&column=7&margin-w=10" />
</p>

<br>

## Contribution snake

<p align="center">
  <img src="https://raw.githubusercontent.com/Saransh1120/Saransh1120/output/snake.svg" />
</p>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=120&section=footer" />
