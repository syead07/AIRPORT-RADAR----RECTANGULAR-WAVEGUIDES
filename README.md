# AIRPORT-RADAR----RECTANGULAR-WAVEGUIDES
RECTANGULAR WAVEGUIDES
 
Real World Example:
How Airport RADAR Uses Rectangular Waveguides
to Detect and Track Aircraft in the Sky

Every time a plane lands safely — rectangular waveguide theory made it possible.



1. Introduction — What is Airport RADAR?

✈️	Think of it like this:  Imagine you are in a dark room and you shout — the echo tells you how far the wall is. Airport RADAR does the same thing, but with invisible microwave waves instead of sound!

RADAR stands for Radio Detection And Ranging. An airport RADAR system sends out a powerful microwave pulse, and when that pulse hits an aircraft, it bounces back. By measuring how long the echo takes to return, the system calculates exactly where the aircraft is — its distance, direction, and speed.

But here is the key question: How does the powerful microwave pulse travel from the transmitter to the antenna without losing energy? The answer is a Rectangular Waveguide — a hollow metal tube that carries microwave energy with almost zero loss, perfect for the high-power demands of RADAR.

💡	Simple Analogy:  A rectangular waveguide is like a hollow metal corridor for microwaves. The waves walk down this corridor from the transmitter, out through the antenna, bounce off the aircraft, come back in, and walk back to the receiver — all at nearly the speed of light!







2. System Overview — Inside an Airport RADAR


A typical Airport Surveillance RADAR (ASR-9) used at Indian airports has these main parts:

Step 1	Transmitter (Klystron)	Generates a very powerful microwave pulse (up to 1-Megawatt peak power!) at S-band frequency of 2.7 to 3.0 GHz. This is the heart of the RADAR system.


Step 2	Rectangular Waveguide (WR-284)	Carries the high-power pulse from the transmitter to the antenna. Also carries the weak echo back to the receiver. THIS IS OUR TOPIC — the most important component!


Step 3	Circulator / T/R Switch	A smart device inside the waveguide that routes: outgoing pulse to antenna, and incoming echo to receiver. Ensures the two signals never interfere with each other.


Step 4	Rotating Antenna Dish	A parabolic dish that rotates 360 degrees every 4 to 12 seconds. It sends the microwave beam outward and collects returning echoes from aircraft up to 450 km away.


Step 5	Receiver (Low Noise Amplifier)	Picks up the tiny echo signal — as weak as one trillionth of the transmitted power — and amplifies it 1,000,000 times for processing.


Step 6	ATC Display Screen	Processes the echo timing to calculate distance and direction. Shows as a bright blip on the Air Traffic Controller screen so aircraft can be safely guided.









3. What is a Rectangular Waveguide? 

A rectangular waveguide is just a hollow metal tube with a rectangular cross-section. There are NO wires inside — just empty air (or dry nitrogen gas in RADAR systems). Microwave signals travel through this empty space, bouncing between the walls, guided from one end to the other.


📐	Key Dimensions:  a = wider side (72.14 mm for WR-284)  |  b = narrower side (34.04 mm for WR-284)  |  Rule: a is always approximately 2 x b. This 2:1 ratio ensures only ONE wave pattern (TE10 mode) travels inside.


In airport RADAR, the waveguide type is WR-284 (the number 284 means the wider dimension is 2.84 inches = 72.14 mm). It is made of thick aluminium alloy, and in RADAR systems it can be several metres long, connecting the equipment room underground to the spinning antenna on the rooftop tower.

🔍	Why not just use a normal cable?  A coaxial cable at 2.8 GHz loses about 0.5 dB per metre — so across a 10-metre run, 70% of your signal is gone as heat! A rectangular waveguide loses only 0.01 dB per metre — just 0.1% loss. For a 1 MW RADAR transmitter, this difference is the gap between a 450 km RADAR range and a useless 20 km range.








4. Key Formulas — Explained Simply (With Examples)




Formula 1 — Cutoff Frequency  (the most important concept!)
Cutoff Frequency	fc = c / (2a)	c = 3x10^8 m/s  ;  a = wider wall in metres

🔑	What does cutoff frequency mean?  Every waveguide has a MINIMUM frequency. Signals BELOW this frequency cannot travel through — they just fade and die within a few centimetres. Signals ABOVE this frequency travel freely. It is like a minimum height requirement at a theme park ride — only the right-sized waves are allowed in!
🚫	Below cutoff (f < fc):  Wave CANNOT propagate. It dies out. Actually useful — it blocks low-frequency noise from entering the RADAR receiver automatically.
✅	Above cutoff (f > fc):  Wave travels freely through the waveguide. RADAR designers always pick the operating frequency to be 1.3 to 1.8 times above the cutoff for a safe margin.





Formula 2 — Guide Wavelength  (wavelength INSIDE the waveguide)
Guide Wavelength	lg = L / sqrt(1-(fc/f)^2)	L = free-space wavelength = c/f

📏	What it means:  The wavelength inside the waveguide is LONGER than in open air. Why? The wave zigzags between the walls instead of going straight, so the pattern stretches out. This is important for designing antenna feeds, matching sections, and slot arrays.





Formula 3 — Group Velocity  (how fast the RADAR pulse actually travels)
Group Velocity	vg = c x sqrt(1-(fc/f)^2)	vg < c (always slower than light)

🕐	Why this matters for RADAR:  The RADAR measures aircraft distance by timing how long the echo takes. But the pulse travels at vg inside the waveguide, not at c. The RADAR computer subtracts this waveguide delay so the aircraft range is accurate. If this correction is missed, the RADAR would show aircraft in the wrong position!







Formula 4 — Wave Impedance  (matching for maximum power transfer)
Wave Impedance (TE)	ZTE = 377 / sqrt(1-(fc/f)^2)	377 ohms = free space impedance ; ZTE > 377 always

🔌	What it means:  Just like matching a loudspeaker to an amplifier, the waveguide impedance must match the transmitter output. If they do not match, power reflects back. In a 1 MW RADAR, even 1% reflection is 10,000 Watts bouncing back into the transmitter — enough to destroy it!











5. Step-by-Step Calculation — Real Airport RADAR Numbers

Let us calculate all waveguide parameters for the ASR-9 Airport Surveillance RADAR used at major Indian airports such as Chennai, Mumbai and Delhi. It uses WR-284 waveguide operating at 2.8 GHz.

Given Data:
Waveguide Type	WR-284  (standard S-band radar waveguide)
Wider dimension  (a)	72.14 mm  =  0.07214 m
Narrower dimension  (b)	34.04 mm  =  0.03404 m
Operating Frequency  (f)	2.8 GHz  =  2.8 x 10^9 Hz
Speed of Light  (c)	3 x 10^8 m/s
Free-Space Impedance	377 Ohms




Step 1 — Cutoff Frequency
Formula	fc = c / (2 x a)	

Substitute	fc = 3x10^8 / (2 x 0.07214)	= 3x10^8 / 0.14428

Answer	fc = 2.079 GHz	Cutoff = 2.079 GHz

✅	Check:  2.8 GHz operating frequency is 1.35x above cutoff 2.079 GHz. The RADAR pulse travels safely through WR-284!



Step 2 — Free-Space Wavelength
Formula	L = c / f	

Substitute	L = 3x10^8 / 2.8x10^9	= 0.1071 m

Answer	L = 107.1 mm	Wavelength in open air



Step 3 — Key Ratio  sqrt(1-(fc/f)^2)
fc/f ratio	2.079 / 2.8  =  0.742	

Square it	0.742^2  =  0.551	(fc/f)^2 = 0.551

Final ratio	sqrt(1 - 0.551) = sqrt(0.449)	= 0.670

📌	Remember 0.670  This single number drives ALL the remaining calculations. It appears in guide wavelength, group velocity, and wave impedance formulas below.



Step 4 — Guide Wavelength  (wavelength inside waveguide)
Formula	lg = L / 0.670	

Substitute	lg = 107.1 / 0.670	= 159.9 mm

Answer	lg = 160 mm	50 mm longer than free-space!

📐	What this means:  The microwave pulse wavelength stretches from 107 mm (free air) to 160 mm inside the WR-284 waveguide. RADAR engineers design antenna slot spacings, matching stubs, and cavity resonators based on this 160 mm guide wavelength.



Step 5 — Group Velocity  (actual pulse travel speed)
Formula	vg = c x 0.670	

Substitute	vg = 3x10^8 x 0.670	= 2.01 x 10^8 m/s

Answer	vg = 2.01x10^8 m/s	= 67% speed of light

🕐	Timing Correction Example:  Waveguide run in ASR-9 = 6 metres. Travel time = 6 / (2.01x10^8) = 29.9 nanoseconds. The RADAR computer subtracts this 30 ns from every echo delay measurement — so aircraft distance is always accurate.



Step 6 — Wave Impedance  (for perfect power matching)
Formula	ZTE = 377 / 0.670	

Substitute	ZTE = 377 / 0.670	= 562.7 Ohms

Answer	ZTE = 563 Ohms	Matched to transmitter output

🔌	Perfect match = full power:  The 1 MW klystron transmitter output port is matched to 563 Ohms using a waveguide taper (gradual size change). This ensures 100% of transmit power enters the waveguide — maximising RADAR detection range.











6. Visual Diagram — The Complete RADAR Waveguide Path

  TRANSMITTER ===waveguide===> CIRCULATOR ===waveguide===> ANTENNA
  1MW Klystron                T/R Switch                  Rotating Dish
  f=2.8GHz,ZTE=563ohm         routes pulses               sends & receives
                                    |
                                    | echo returns (very weak, ~10^-12 W)
                                    |
                               RECEIVER LNA ===> SIGNAL PROCESSOR ===> ATC SCREEN
                               Amplifies echo    Calculates range       Aircraft blip

🎯	Every === waveguide === in the diagram above is WR-284 rectangular waveguide.  Without it, the 1 MW pulse loses 70% of its power per 10 metres. The RADAR range would collapse from 450 km to just a few kilometres — completely useless for air traffic control.

7. Why Rectangular Waveguide? — Comparison Table

Feature	Coaxial Cable	Circular Waveguide	Rectangular Waveguide (WR-284)
Power handling	Low (kilowatts)	High (megawatts)	Highest (megawatts+)
Signal loss at 2.8 GHz	0.5 dB/m (high!)	0.02 dB/m	0.01 dB/m (lowest)
Number of modes	1 (TEM)	Multiple (messy)	1 dominant (TE10 clean)
Manufacturing	Easy, flexible	Complex, expensive	Easy, standard sizes
RADAR use?	Short runs only	Rarely used	YES — primary choice
Cost	Low	High	Medium — worth it!


8. Summary — All Calculated Values at a Glance

Parameter	Calculated Value	Plain-English Meaning
Cutoff Frequency (fc)	2.079 GHz	Minimum freq; 2.8 GHz is safely above this
Free-Space Wavelength	107.1 mm	Wavelength of 2.8 GHz in open air
Key Ratio sqrt(1-(fc/f)^2)	0.670	Used in all formulas below
Guide Wavelength (lg)	159.9 mm = 160 mm	Wavelength inside waveguide — 50% longer
Group Velocity (vg)	2.01x10^8 m/s (0.67c)	Actual pulse speed; used for timing correction
Wave Impedance (ZTE)	562.7 Ohms = 563 Ohm	Matched to transmitter for zero reflections
Waveguide Loss	~0.01 dB/m	Only 0.1% loss per metre — excellent!

9. Conclusion

The next time you see a plane landing safely at Chennai, Mumbai or Delhi airport, remember: a rectangular waveguide made it possible. Behind every successful aircraft detection is a WR-284 aluminium tube, precisely engineered using the formulas we calculated above, carrying 1 megawatt microwave pulses at 2.8 GHz with almost zero loss.

Here is what rectangular waveguide theory does for airport RADAR, in plain words:

•	Cutoff frequency (2.079 GHz) blocks all low-frequency noise automatically — only the RADAR signal at 2.8 GHz can enter the waveguide.
•	Guide wavelength (160 mm) tells engineers how to design antenna slot arrays and matching sections for maximum radiated power.
•	Group velocity (0.67c) tells the RADAR computer exactly how much waveguide delay to subtract so aircraft distance is always measured correctly.
•	Wave impedance (563 Ohm) ensures the full 1 MW transmitter power enters the waveguide with zero reflections — protecting the transmitter and maximising RADAR range.
•	Single TE10 mode keeps the microwave beam clean — no false aircraft detections from unwanted wave patterns.

From the equations in a textbook to the aircraft blip on an ATC screen —
Rectangular Waveguide Theory keeps our skies safe, every single day.
Rectangular Waveguides  |  Airport RADAR Case Study  |  ASR-9  |  WR-284  |  2.8 GHz  |  TE10 Mode  |  Simple & Student-Friendly
