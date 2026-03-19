RECTANGULAR WAVEGUIDES

How Airport RADAR Uses Rectangular Waveguides
to Detect and Track Aircraft in the Sky
ASR-9  |  WR-284  |  2.8 GHz  |  TE10 Mode  |  1 MW Power

1. Introduction — What is Airport RADAR?

✈️	Think of it like this:  Imagine you shout in a dark room — the echo tells you how far the wall is. Airport RADAR does exactly this but with invisible microwave waves instead of sound!

RADAR stands for Radio Detection And Ranging. An airport RADAR sends out a powerful microwave pulse, which bounces back when it hits an aircraft. By measuring the echo delay, the system calculates the aircraft position, distance, and speed.

The key question is: How does this 1 megawatt pulse travel from the transmitter to the antenna without losing energy? The answer is the Rectangular Waveguide — a hollow metal tube that guides microwave energy with almost zero loss.

2. Waveguide Structure — Cross-Section Diagram

A rectangular waveguide (WR-284) is a hollow aluminium tube with dimensions a = 72.14 mm (wider wall) and b = 34.04 mm (narrower wall). The ratio a = 2b ensures only the dominant TE10 mode propagates inside.

<img width="906" height="438" alt="image" src="https://github.com/user-attachments/assets/c5ed30a8-8b0c-48be-ac76-21ee685e65c9" />

 
Figure: WR-284 Rectangular Waveguide Cross-Section — TE10 Electric Field Pattern

📐	Key Rule:  In TE10 mode, the Electric field (E) points vertically — strongest at the centre (x = a/2) and zero at both metal walls. This clean, single-mode operation is what makes waveguides ideal for RADAR.

3. Airport RADAR System — How Everything Connects

The rectangular waveguide is the critical link between the transmitter, circulator, antenna, and receiver. All high-power signal routing in airport RADAR passes through WR-284 waveguide sections.

 <img width="938" height="344" alt="image" src="https://github.com/user-attachments/assets/8f609412-df0a-4f1f-b442-305a6a7d2203" />

Figure: Airport RADAR System Flow — WR-284 Waveguide connects all components

💡	Simple Summary:  Transmitter generates 1 MW pulse → Waveguide carries it → Antenna radiates it → Aircraft reflects echo → Waveguide brings echo back → Receiver processes it → ATC screen shows the aircraft blip.

4. TE10 Mode — Electric and Magnetic Field Patterns

The TE10 (Transverse Electric) mode is the dominant mode in WR-284. It is the only mode that propagates at 2.8 GHz in this waveguide, keeping the RADAR signal clean and predictable with no unwanted interference patterns.

 <img width="938" height="375" alt="image" src="https://github.com/user-attachments/assets/30cc071d-ac6f-4c42-88c0-96aa0dbbc6ed" />

Figure: TE10 Mode — Electric field (left) and Magnetic field (right) inside WR-284

•	Electric field (E) — vertical arrows, strongest in the centre, zero at the metal walls
•	Magnetic field (H) — horizontal arrows, strongest at the walls, zero in the centre
•	Single mode only — no other mode propagates at 2.8 GHz in WR-284

5. Key Formulas — With Simple Explanations

Formula 1 — Cutoff Frequency
Cutoff Frequency	fc = c / (2a)	c = 3x10^8 m/s  ;  a = wider wall in metres

Every waveguide has a minimum frequency (cutoff). Signals below this frequency cannot travel through — they die out instantly. Signals above this frequency travel freely. For WR-284: fc = 2.079 GHz.

 <img width="906" height="359" alt="image" src="https://github.com/user-attachments/assets/c581658b-1b8d-473d-ac5d-6d0f98a5fe5d" />

Figure: Cutoff Frequency — Signal dies below fc, travels freely above fc

Formula 2 — Guide Wavelength
Guide Wavelength	lg = L / sqrt(1-(fc/f)^2)	L = free-space wavelength = c/f

The wavelength inside the waveguide is longer than in free air because the wave bounces in a zigzag path between the walls. For WR-284 at 2.8 GHz: lg = 160 mm (vs 107 mm in open air).

 <img width="906" height="359" alt="image" src="https://github.com/user-attachments/assets/a534e25e-1cfd-4373-844e-c83abe742df8" />

Figure: Guide Wavelength — Inside waveguide (160 mm) vs free-space (107 mm)

Formula 3 — Group Velocity
Group Velocity	vg = c x sqrt(1-(fc/f)^2)	vg < c — actual pulse travel speed

🕐	RADAR Timing:  The RADAR pulse travels at 0.67c inside the waveguide. For a 6-metre waveguide run, this adds a 30 ns delay. The RADAR computer subtracts this delay from all echo measurements so aircraft positions are accurate.

Formula 4 — Wave Impedance
Wave Impedance (TE)	ZTE = 377 / sqrt(1-(fc/f)^2)	ZTE > 377 Ohms always ; matched to transmitter

 <img width="906" height="367" alt="image" src="https://github.com/user-attachments/assets/c06f6148-9eb1-46c3-9e75-f2dc5f63d822" />

Figure: Wave Impedance Matching — Mismatched (left) vs Perfectly Matched (right)

6. Step-by-Step Calculations — All Results

Using WR-284 waveguide at 2.8 GHz (ASR-9 RADAR, Chennai/Mumbai/Delhi airports):

 <img width="938" height="453" alt="image" src="https://github.com/user-attachments/assets/fdb9cd34-90d2-4e76-b389-25ebb099b20f" />

Figure: All 6 Calculation Steps — WR-284 at 2.8 GHz

✅	All answers verified:  fc=2.079 GHz (below 2.8 GHz — safe margin)  |  lg=160 mm  |  vg=2.01x10^8 m/s (67% of light)  |  ZTE=563 Ohm

Detailed Step-by-Step Working:
Step 1 — fc	fc = 3x10^8 / (2 x 0.07214)	= 2.079 GHz

Step 2 — Wavelength	L = 3x10^8 / 2.8x10^9	= 107.1 mm

Step 3 — Key Ratio	sqrt(1 - (2.079/2.8)^2) = sqrt(0.449)	= 0.670

Step 4 — Guide Wavelength	lg = 107.1 / 0.670	= 160 mm

Step 5 — Group Velocity	vg = 3x10^8 x 0.670	= 2.01x10^8 m/s

Step 6 — Wave Impedance	ZTE = 377 / 0.670	= 563 Ohm

7. RADAR Coverage — Real Airport View

The ASR-9 Airport Surveillance RADAR (used at Chennai, Mumbai, Delhi) achieves a detection range of 450 km. This range is possible ONLY because the rectangular waveguide carries the full 1 MW transmit power to the antenna with minimal loss.

 <img width="703" height="703" alt="image" src="https://github.com/user-attachments/assets/a626d6a8-4b71-4347-ab7f-8091515b0336" />

Figure: ASR-9 RADAR Coverage — Chennai Airport, 450 km detection range

🎯	Why range matters:  If a coaxial cable were used instead of WR-284 waveguide, the signal loss would be so high that the RADAR range would shrink from 450 km to under 20 km — completely useless for air traffic control.

8. Conclusion

The rectangular waveguide WR-284 is the invisible backbone of every airport RADAR system. Every time an aircraft is detected and guided safely to landing, these simple hollow metal tubes — engineered using the formulas above — are doing the critical work.

•	Cutoff frequency (2.079 GHz) — natural filter, blocks all noise below this frequency automatically
•	Guide wavelength (160 mm) — used to design antenna slots, matching sections and cavity resonators
•	Group velocity (0.67c) — RADAR computer corrects for this delay to give accurate aircraft positions
•	Wave impedance (563 Ohm) — matched to transmitter so 100% of 1 MW reaches the antenna
•	TE10 single mode — clean, predictable beam with no false aircraft detections

From equations in a textbook to the aircraft blip on an ATC screen —
Rectangular Waveguide Theory keeps our skies safe, every single day.

Rectangular Waveguides  |  Airport RADAR  |  ASR-9  |  WR-284  |  2.8 GHz  |  TE10 Mode  |  Chennai / Mumbai / Delhi Airports
