# WRO-FUTURE-ENGINEERS-2025 - TEAM TRAKTORISTAK

<p align="center">
  <img src="other/Logo.png" alt="Traktoristak team logo" width="420">
</p>

> An autonomous vehicle designed for the Future Engineers category of the WRO 2025 that uses computer vision, distance sensing, and autonomous control software to navigate the track and avoid obstacles.

<a name="team-introduction--team-information"></a>
## Team Introduction & Team Information

<table>
  <tr>
    <td align="center" width="50%">
      <img src="t-photos/Members/Richard.jpg" alt="Richard Nagy" width="100%" style="border-radius: 8px;"><br>
      <strong>RICHARD NAGY</strong><br>
      <em>Team Lead, Hardware and Software Developer</em><br>
      <sub>Robot Control, Hardware Integration, Software Architecture</sub>
    </td>
    <td align="center" width="50%">
      <img src="t-photos/Members/Mark.jpg" alt="Mark Gulyas" width="100%" style="border-radius: 8px;"><br>
      <strong>MARK GULYAS</strong><br>
      <em>Mechanical Designer</em><br>
      <sub>Mechanical Design, Robot Assembly, CAD Development</sub>
    </td>
  </tr>
</table>

## Content Structure

* `t-photos` - Contains team member photos and can hold the official team photo and informal group pictures.
* `v-photos` - Includes vehicle images: top, bottom, front, back, left, and right.
* `video` - Holds `video.md` with a link to the driving demonstration.
* `schemes` - Contains the hardware repository with KiCad schematics, wiring references, component pictures, and generated schematic PDF.
* `src` - Full Python source code repository for all robot control components used in the competition.
* `models` - Contains the mechanical repository for robot design files and 3D-printable model assets.
* `other` - Contains supporting files, including resources used for this `README.md` and overall documentation.
* `obstacle challenge & open challenge` - Includes the complete codebase or references for both competition challenges.

---

## Table of Contents

- [Overview](#overview)
- [Team Introduction & Team Information](#team-introduction--team-information)
- [Content Structure](#content-structure)
- [Engineering Documentation](#engineering-documentation)
- [Cloning](#cloning)

---

<a name="overview"></a>
## Overview

This autonomous vehicle prototype was developed for the WRO Future Engineers 2025 competition. The robot uses a Raspberry Pi 3 as its main controller, with a regulated 5 V power system, ultrasonic distance sensors, IR reflectance sensors, a CSI camera, and an L298N motor driver for drivetrain and steering control. The software is written in Python and combines camera-based color detection, distance sensing, race-state logic, PID utilities, and modular hardware drivers to navigate the competition track and avoid obstacles. The project is organized into separate hardware, software, and mechanical areas so the full engineering process can be documented clearly from wiring and schematics to robot behavior and deployment.

<a name="engineering-documentation"></a>
## Engineering Documentation

- [Hardware documentation](schemes/README.md): controller, power system, sensors, camera, motor driver, wiring, and schematic references.
- [Software documentation](src/README.md): setup, robot runtime, deployment, calibration, component tests, architecture, and development workflow.
- [Architecture](src/docs/architecture.md): software structure and runtime responsibilities.
- [Hardware and Configuration](src/docs/hardware-and-config.md): pin configuration and hardware setup.
- [Deployment](src/docs/deployment.md): Raspberry Pi deployment workflow.
- [Calibration](src/docs/calibration.md): camera calibration process.

## Cloning

Clone this repository with its submodules:

```bash
git clone --recurse-submodules https://github.com/Ricsi1231/WRO-Robot.git
```

If the repository was already cloned, initialize and update the submodules:

```bash
git submodule update --init --recursive
```
