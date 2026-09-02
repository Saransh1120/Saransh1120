## Hi, I'm Saransh

Engineering student. I mostly build things that sit between hardware and software,
because that's where the interesting bugs are.

Right now I'm doing DSA in C++ every day and pushing whatever I solve the same
day. Slowly moving into full-stack web work (TypeScript, React, Node) since
that's where I want to end up. On the hardware side I write ESP32 firmware, wire
up I2C and I2S sensors, and solder on perfboard when I don't have a PCB.

Mail: sargarbhit19@gmail.com

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

`C++` `Arduino` `ESP32-S3` `Python`

<br>

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

`TypeScript` `Fastify` `PostgreSQL` `React` `ESP32`

<br>

### c--dsapw

My daily C++ practice. Conditionals, loops, patterns, and whatever DSA topic I'm
on. It's messy on purpose. It's a log of the reps, not a portfolio piece.

`C++`

<br>

## Stuff I use

C++, Java, TypeScript, JavaScript, Python. React, Node, Postgres on the web side.
Arduino and ESP-IDF for firmware. Git and VS Code for everything else.

<br>

<p align="center">
  <img height="160" src="https://github-readme-stats.vercel.app/api?username=Saransh1120&show_icons=true&theme=dark&hide_border=true" />
  <img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Saransh1120&layout=compact&theme=dark&hide_border=true" />
</p>
