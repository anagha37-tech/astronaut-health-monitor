# 🚀 Astronaut Health Monitor

A web dashboard that monitors the health of one astronaut during a space mission, using simulated data that changes over time.

**Live demo:** https://YOUR-USERNAME.github.io/astronaut-health-monitor/

## Features
- 5 health parameters: heart rate, oxygen level, body temperature, sleep duration, exercise time
- Per-parameter status: Normal / Warning / Critical
- Overall status banner (shows the worst status across all parameters)
- Mission day and time indicator
- Live sparkline trends and an alert log
- Random data that updates every 2 seconds

## Alert Logic
Each value is checked against two ranges:
- Inside the normal range → **NORMAL**
- Inside the wider warning range → **WARNING**
- Outside both → **CRITICAL**

Example: Oxygen ≥ 95% is Normal, 90–94% is Warning, and **below 90% triggers a CRITICAL ALERT**. The banner turns red and flashes, and the event is saved in the Alert Log with the mission day and time.

## Tech
HTML, CSS, and JavaScript (single file, no dependencies).
