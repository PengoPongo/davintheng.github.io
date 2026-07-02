# Engineering Portfolio | Davin Theng

Welcome to my personal engineering portfolio repository. This website showcases my academic background, technical skills, and key engineering projects spanning embedded systems, software development, and hardware integration.

🔗 **Live Website:** [[https://pengopongo.github.io/](https://pengopongo.github.io/davintheng.github.io/)]

---

## 🛠️ Technical Skillset

* **Languages:** C, C++, Python, MIPS Assembly, HTML5, CSS3, JavaScript
* **Embedded & Hardware:** PIC32MM Microcontrollers, Raspberry Pi SBCs, Bare-Metal Programming, Hardware Interrupts, ADC Sampling, Circuit Design
* **Core Competencies:** Software Development, Hardware-Software Co-design, UI/UX Prototyping

---

## 🚀 Featured Projects

### 1. Two-Player MIPS Assembly Dice Game
A low-level, bare-metal interactive game built entirely in MIPS Assembly on the **PIC32MM Curiosity Development Board**. 
* **Hardware Interfacing:** Configured I/O ports via memory-mapped registers (`TRISA`, `TRISB`, `TRISC`) to drive a physical 7-segment display and status LEDs.
* **Interrupt-Driven Logic:** Implemented Change Notification (CN) hardware interrupts (Vector #9) on Port B to eliminate wasteful polling cycles for tactile input buttons.
* **True Random Seeding:** Routed an ungrounded analog input pin into a 10-bit Analog-to-Digital Converter (ADC) to sample atmospheric thermodynamic noise, creating a truly unpredictable randomized seed pool for the dice rolls.
* **Signal Debouncing:** Engineered a precise down-counting software delay subroutine loop to isolate and neutralize physical button contact ripples.

### 2. Kin:pathic Visual Timer (Capstone Project)
An assistive visual countdown timer custom-designed for **Kin:pathic ABA** to help children with autism manage routine transitions smoothly.
* **System Architecture:** Powered by a customized Raspberry Pi Micro computer tucked inside a custom, child-safe structural enclosure.
* **UI/UX Stack:** Built an intuitive custom graphics environment complete with a responsive touchscreen interface, enabling caregivers to load target transition images via USB storage.
* **Power Management:** Integrated an efficient battery system safe for extended classroom applications, ensuring an 8+ hour continuous operational runtime.

---

## 💻 Website Architecture & Performance

The website is engineered to be lightweight, responsive, and performant:
* **Vanilla Architecture:** Developed using semantic **HTML5**, standard **CSS3**, and asynchronous native **JavaScript** to optimize asset loads without reliance on heavy framework overhead.
* **Responsive Grid Layouts:** Employs CSS Flexbox and Grid architectures to gracefully scale across ultra-wide desktop monitors, laptops, tablets, and mobile smartphones.
* **Smooth Navigation:** Includes native event-driven window scrolling transitions for internal section jumps across the single-page layout.

---

## 📂 Repository Structure

```text
├── index.html               # Main landing page & summary portfolio text
├── kinpathic-timer.html     # Deep-dive showcase page for the Capstone Timer project
├── dice-game.html           # Deep-dive technical page for the MIPS Dice Game project
├── style.css                # Global stylesheet containing responsive layouts
├── script.js                # Vanilla JS handling navigation animations
└── README.md                # Repository documentation
