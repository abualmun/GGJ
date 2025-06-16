# 🐔 Chicken On A Mission
![](screenshots/0.jpg)
![](screenshots/1.jpg)
**Sack Escape** is a fast-paced 3D game where you play as a brave chicken trying to collect scattered sacks while dodging dangerous barbarians. The game takes place on a spherical world, and the chase never stops!

## 🎮 Game Concept

You're a determined chicken with one goal: collect all the sacks before the barbarians catch you. They're strong, fast, and relentless — but you're smarter, sneakier, and lighter on your claws.

## 🧠 Vector-Based Movement

The core of the game’s mechanics is built around **vector calculations**. Everything — from chasing, escaping, to collecting items — is done using custom vector math. Here are a few highlights:

* 🧭 The chicken always orients to walk on a spherical terrain. Movement is handled with smooth vector-based rotation and orientation.
* 🏃 The player's movement isn't just “left” and “right” — it's defined by movement **relative to the planet's surface**, ensuring the character stays grounded in all directions.
* 📡 Enemies detect and pursue the player using `Vector3.MoveTowards` and awake based on a calculated radius.
* 🧲 Collectables and enemies respond to dynamic vectors, adjusting behavior as the player moves across the globe.

## 🐔 Player Movement

We put a lot of effort into making movement *feel right*:

* Smooth spherical gravity ensures your chicken hugs the planet surface at all times.
* Directional movement works even when the "up" vector changes — thanks to world space vector projection.
* The chicken can sprint, turn sharply, and react naturally to terrain curvature.

## 🛡️ Features

* 🎒 Sack collection with animation and sound feedback.
* 🪓 Barbarians with detection zones and chase logic.
* 🌍 A planet-based level that feels immersive and continuous.
* 🧭 Optional minimap and sack indicators to help navigate.
* ✨ Visual particles and feedback systems in the works.


![](screenshots/2.jpg)

![](screenshots/3.jpg)

## 🔧 Known Issues (but they’re part of the charm!)

* Moving directly across the planet may sometimes slow down due to the limitations of straight-line movement on curved space.
* Win/Lose conditions are being refined for frame-accurate responsiveness.
* Close encounters with enemies can feel abrupt (we're tuning the hit delay).


![](screenshots/4.jpg)