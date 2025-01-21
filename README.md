# ASME Aztec Rover Team (A.R.T.) - Remote Division
**Project Repository: [ASME-Aztec-Rover-Team-A.R.T.-Remote-Division](#)**  
Welcome to the **Remote Division** of the ASME Aztec Rover Team. This repository focuses on the remote communications, electronics, and power distribution aspects of our Mars Rover project. Below, you will find an overview of the team structure, major subsystems, and technical details relevant to our division.

---

## Table of Contents
1. [Project Overview](#project-overview)  
2. [Team Structure](#team-structure)  
3. [Preliminary Design Report Summary](#preliminary-design-report-summary)  
4. [Remote Division Focus](#remote-division-focus)  
5. [Technologies & Tools](#technologies--tools)  
6. [Contributing](#contributing)  
7. [License & Acknowledgments](#license--acknowledgments)
8. [Contact](#Contact)

---

## Project Overview
The **Aztec Rover Team (A.R.T.)** at San Diego State University is a student-led organization dedicated to designing and building a Mars Rover to compete in various rover challenges. Our multidisciplinary team is split into multiple divisions, each responsible for a distinct set of tasks, such as:

- **Chassis & Drivetrain**  
- **Suspension**  
- **Arm & Manipulator**  
- **Laboratory & Procurement**  
- **Vision & Autonomous Navigation**  
- **Power & Controls**  
- **Remote Communications (Our Division)**  

The overarching goal is to create a robust, versatile Mars Rover capable of completing missions related to exploration, science, and autonomous navigation.

<p align="center">
  <img src="https://github.com/user-attachments/assets/6743928a-3128-45f8-a375-6f690b581269" alt="Gearbox Installation" width="600">
</p>

---

## Team Structure
Our team’s leadership is organized as follows:

- **Project Manager (PM)**: Oversees administrative management and coordinates multiple divisions.
- **Project Lead (PL)**: Oversees technical aspects of the project and coordinates the remaining divisions.
- **Division Leads**: Liaison to both the PM and PL, ensuring tasks are delegated and completed efficiently.
- **Members**: Contribute directly to the design, analysis, fabrication, and testing efforts.

We currently have 9 divisions, with roughly 50 members ranging from first-year undergraduates to graduate students, primarily in STEM fields.

**Key Collaboration & Communication Tools**  
- **Discord** for general communication  
- **GitHub** for code and CAD file version control  
- **Google Drive** for documentation, records, and team notes  

---

## Preliminary Design Report Summary
The **Preliminary Design Report** outlines the rover’s design, mission objectives, and plans for fabrication and testing. Major highlights include:

1. **Finances & Facilities**  
   - **Funding** through SDSU Student Success Fee (SSF) and ASME San Diego Chapter.  
   - **Facilities** located in the SDSU Engineering basement workshop, equipped for milling, welding, laser cutting, 3D printing, and more.

2. **Lifecycle Approach**  
   - **System Engineering Engine** approach, with top-down design.  
   - Parallel division collaboration, iterative simulations, and early prototyping.

3. **Systems Integration & Testing**  
   - Weekly leadership and division meetings.  
   - Finite element analysis, local testing of autonomous tasks, and large-scale testing after rover assembly.

4. **Major Subsystems**  
   - **Chassis, Drivetrain & Suspension**: Rocker-bogie suspension, TPU printed wheels.  
   - **Arm & Manipulator**: 6 DOF articulated arm with rotating base, parallel jaw gripper.  
   - **Lab & Procurement**: Soil auger, test tube system, Raman spectroscopy for chemical analysis.  
   - **Vision & GNSS**: Camera-based hazard avoidance and visual markers, plus real-time kinematic GNSS for autonomous navigation.  

5. **Power & Controls**  
   - Off-the-shelf batteries and a power distribution board.  
   - Battery management system for voltage and current tracking.  
   - Emergency stop button for rover-wide power cutoff.  

6. **Remote Communications (Our Division)**  
   - **Nvidia Jetson Orin NX** as the onboard computer.  
   - **Raspberry Pi Pico** microcontroller interfacing with sensors and actuators.  
   - **I2C** for internal component communication, **USB** for Pico-to-NX communication.  
   - **900 MHz point-to-point radios** for remote control between rover and base station.  

---

## Remote Division Focus
As the **Remote Division**, our responsibilities include designing and implementing the long-range communications and operational control of the rover. Specifically, we focus on:

1. **Radio Link**  
   - **900 MHz point-to-point radios** with directional (base station) and omnidirectional (rover) antennas.  
   - Ensuring **reliable data transmission** for rover telemetry and real-time control under varying environmental conditions.

2. **Onboard Computing & Microcontrollers**  
   - Integrating the **Nvidia Jetson Orin NX** and the **Raspberry Pi Pico** via USB.  
   - Utilizing **I2C** for sensor data collection and subsystem control signals.  
   - Handling processes for payload systems, vision processing, and control logic.

3. **Power Distribution & Safety**  
   - Collaborating with the **Power & Controls** team to ensure stable power to communications hardware.  
   - Overseeing the integration of the **emergency stop (E-Stop)** functionality to instantly shut down rover electronics.

4. **Data Monitoring & Logging**  
   - Developing logs for received/transmitted data packets, microcontroller sensor data, and rover status updates.  
   - Coordinating with the base station to provide real-time feedback and alerts.

---

## Technologies & Tools
- **Languages**: C++, Python, embedded C  
- **Hardware**: 
  - Nvidia Jetson Orin NX  
  - Raspberry Pi Pico  
  - 900 MHz Radio Modules  
  - Battery Management System  
- **Software & Frameworks**: 
  - ROS2 Humble  
  - I2C drivers and libraries  
  - Microcontroller SDKs  
  - Embedded Linux environment on the Jetson
  - U-center (U-blox) from GNSS 
- **CAD & Simulation**:  
  - SolidWorks for mechanical assemblies  
  - FEA tools for structural validation  
  - Custom simulation setups for radio link tests  

---

## Contributing
We welcome contributions from SDSU ASME members and the open-source community. Here’s how you can help:

1. **Fork** this repository and clone it locally.  
2. Create a new branch for your feature/bug fix:  
   ```bash
   git checkout -b feature/your-feature
   ```
3. Commit your changes and push them to your repository:
   ```bash
   git add .
   git commit -m "Add your feature"
   git push origin feature/your-feature
   ```
4. Open a **Pull Request** on this repository describing your changes.

Make sure to follow the team's **style guidelines** and review process which will be detailed in the CONTRIBUTING.md file.

---

## License & Acknowledgments
This project is part of the San Diego State University (SDSU) ASME student chapter’s mission to provide hands-on design experience. Funding and support for the Aztec Rover Team have been generously provided by:
- ASME San Diego Chapter
- SDSU Student Success Fee
- Various Individual Sponsors
  
If you use any part of this project, please acknowledge the SDSU ASME Aztec Rover Team.

**Thank you for supporting our mission to develop innovative engineering solutions for our planetary rover.**

---

## Contact
For inquiries, collaborations, or more information on the Remote Division, reach out to any of us on our Discord.
- Project Manager: Giovanni Diaz-Lopez
- Project Lead: Jefferson Young
- **Remote Division Lead**: Sean Hedgecock

_This README is a living document and subject to change as the project evolves._
