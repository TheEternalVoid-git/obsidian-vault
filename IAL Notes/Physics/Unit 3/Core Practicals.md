# Core Practicals

---

## Exam Skills & Mathematical Toolkit

### 1. Uncertainty Rules
* **Adding or Subtracting Values ($A = B \pm C$):** Add the **absolute** uncertainties.
  $$\Delta A = \Delta B + \Delta C$$
* **Multiplying or Dividing Values ($A = B \times C$ or $A = B / C$):** Add the **percentage** uncertainties.
  $$\% \Delta A = \% \Delta B + \% \Delta C$$
* **Power Functions ($A = B^n$):** Multiply the percentage uncertainty by the index $n$.
  $$\% \Delta A = n \times (\% \Delta B)$$

### 2. Line of Best Fit vs. Worst Fit
* To calculate the percentage uncertainty in a gradient ($m$):
  1. Plot data points along with their vertical or horizontal **error bars**.
  2. Draw the **Line of Best Fit** ($m_{\text{best}}$) passing optimally through all points.
  3. Draw the **Line of Worst Fit** ($m_{\text{worst}}$). This is the steepest or shallowest possible straight line that still passes through all error bars.
  4. Calculate the uncertainty using:
     $$\% \text{ Uncertainty in Gradient} = \frac{|m_{\text{best}} - m_{\text{worst}}|}{m_{\text{best}}} \times 100\%$$

### 3. General Accuracy Routines
* **Zero Errors:** Always check instruments (micrometer, vernier calipers, digital scales) before taking readings. Record any shifting value and subtract/add it to all subsequent raw data measurements.
* **Parallax Error:** Position your eye line **perpendicularly** and level with the meniscus or scale marking to ensure precise readings.
* **Anomalous Values:** Inspect data tables before averaging. Explicitly cross out and exclude any anomalous entries from mean calculations.
* **Significant Figures (SF):** Final calculated answers must match the lowest number of significant figures present across the raw variables used.

---

##  The 8 Core Practicals

### 1. Determination of $g$ (Acceleration of Free Fall)
* **Goal:** Determine the acceleration of free fall ($g$) using a falling object under gravity.
* **Apparatus:** Electromagnet, steel ball bearing, trapdoor switch, electronic timer, metre ruler.
* **Method:**
  1. Measure the vertical height ($h$) from the bottom of the suspended ball bearing to the trapdoor platform using a metre ruler.
  2. Switch off the electromagnet power supply to drop the ball. This breaks a circuit loop, automatically starting the electronic timer.
  3. The ball bearing impacts the trapdoor plate, opening the target circuit and halting the timer. Record time ($t$).
  4. Repeat the drop 3 times at this position to compute a mean time.
  5. Vary the height ($h$) upward to collect data for at least 6 different displacement intervals.
* **Graph & Analysis:**
  * Base equation: $s = ut + \frac{1}{2}at^2$. Since $u = 0$, this yields $h = \frac{1}{2}gt^2$.
  * Plot **$h$ on the y-axis** against **$t^2$ on the x-axis**.
  * Gradient of the line: $\text{Gradient} = \frac{g}{2}$
  * Calculate constant: $g = 2 \times \text{Gradient}$
* **Accuracy / Exam Pitfalls:**
  * **Tip:** Choose a small, heavy steel ball bearing to drastically minimize the counter-effects of air resistance.
  * **Trap:** Do not measure $h$ from the top or middle of the ball bearing. Always calculate from its base to maintain absolute consistency with the impact face.

### 2. Determination of the Young Modulus of a Material
* **Goal:** Find the Young Modulus ($E$) of a long metal wire.
* **Apparatus:** Long test wire, G-clamp, bench pulley, slotted mass hanger, micrometer screw gauge, metre ruler, tape marker.
* **Method:**
  1. Clamp one end of a long wire (approx. 2–3 meters) firmly to the laboratory bench. Pass the remaining length over a low-friction pulley at the opposite edge, hanging a mass holder.
  2. Measure the wire's initial diameter ($d$) at 3 separate locations and rotating angles using a micrometer. Compute cross-sectional area: $A = \frac{\pi d^2}{4}$.
  3. Gauge the baseline length ($L$) from the fixed clamp face to a thin paper tape marker fixed on the wire using a metre ruler.
  4. Place a known mass (e.g., 100g) on the holder. Use a parallel ruler scale or traveling microscope to identify the marker displacement. Calculate extension: $\Delta L = \text{new position} - \text{initial position}$.
  5. Increment masses sequentially, tracking matching values of $\Delta L$. Stay within the material's elastic limit.
* **Graph & Analysis:**
  * Base equation: $E = \frac{\text{Stress}}{\text{Strain}} = \frac{F/A}{\Delta L / L} \implies F = \left(\frac{EA}{L}\right)\Delta L$.
  * Plot **Force ($F = mg$) on the y-axis** against **Extension ($\Delta L$) on the x-axis**.
  * Gradient of the line: $\text{Gradient} = \frac{EA}{L}$
  * Calculate constant: $E = \frac{\text{Gradient} \times L}{A}$
* **Accuracy / Exam Pitfalls:**
  * **Tip:** Use a very long, thin wire sample. Maximizing initial length ($L$) drives up the observable extension ($\Delta L$), bringing down percentage uncertainty.

### 3. Determination of the Resistivity of a Wire
* **Goal:** Determine the structural resistivity ($\rho$) of a specialized metal wire (e.g., constantan).
* **Apparatus:** Constantan wire fixed to a metre ruler, digital multimeter (or ammeter + voltmeter layout), power cell, flying lead wire terminal, micrometer.
* **Method:**
  1. Map the diameter ($d$) of the wire at multiple points via a micrometer to figure out the mean cross-sectional area ($A$).
  2. Bridge the wire into a standard low-voltage circuit loop. Connect a digital multimeter configured to analyze resistance ($R$).
  3. Attach the adjustable flying lead clip to the target wire at an initial test baseline length ($l = 10.0\text{ cm}$). Observe and note the resistance ($R$).
  4. Step the flying lead out in set jumps of $10.0\text{ cm}$ up to $100.0\text{ cm}$, logging the new resistance ($R$) at each mark.
* **Graph & Analysis:**
  * Base equation: $R = \frac{\rho l}{A}$.
  * Plot **Resistance ($R$) on the y-axis** against **Length ($l$) on the x-axis**.
  * Gradient of the line: $\text{Gradient} = \frac{\rho}{A}$
  * Calculate constant: $\rho = \text{Gradient} \times A$
* **Accuracy / Exam Pitfalls:**
  * **Tip:** Open the control switch to break the circuit current between individual measurements. Allowing continuous charge raises the internal wire temperature, which alters resistance and introduces systematic bias.

### 4. Determination of the Internal Resistance and EMF of a Cell
* **Goal:** Calculate the internal resistance ($r$) and raw electromotive force ($\varepsilon$) of an electrochemical cell.
* **Apparatus:** Test cell, variable resistor (rheostat), digital ammeter, digital voltmeter, circuit toggle switch.
* **Method:**
  1. Build a series test circuit linking the cell, control switch, ammeter, and adjustable rheostat. Bridge the voltmeter directly in parallel across the positive and negative cell terminals.
  2. Close the circuit switch and adjust the rheostat to its absolute maximum resistance level. Log terminal potential difference ($V$) and current ($I$).
  3. Turn the rheostat dial to lower internal load resistance, systematically taking corresponding pairs of $V$ and $I$ readings over a widespread path (minimum of 6 data lines).
  4. Disconnect the switch between steps to shield the test cell from premature drain or heat shifts.
* **Graph & Analysis:**
  * Base equation: $\varepsilon = V + Ir \implies V = -rI + \varepsilon$ (conforms to $y = mx + c$).
  * Plot **Terminal Voltage ($V$) on the y-axis** against **Current ($I$) on the x-axis**.
  * Interpretation: **Y-intercept = EMF ($\varepsilon$)**; **Absolute value of the Gradient = Internal Resistance ($r$)**.
* **Accuracy / Exam Pitfalls:**
  * **Tip:** Deploy a high-impedance digital voltmeter. This prevents stray current leakages into the measurement branch, keeping terminal readings accurate.

### 5. Determination of the Speed of Sound in Air
* **Goal:** Measure the speed of sound propagation through ambient air utilizing a resonance tube column.
* **Apparatus:** Set of calibrated tuning forks, long open glass tube shell, deep measuring cylinder filled with water, metre ruler.
* **Method:**
  1. Insert the open glass tube vertically into the water-filled outer cylinder. The fluid line acts as a hard acoustic block, forming a custom pipe closed at one end.
  2. Strike a selected tuning fork of fixed frequency ($f$) against a dense rubber block. Position it horizontally over the open lip of the glass tube.
  3. Slowly elevate or lower the glass tube inside the water until the audio note resonates into a stark, sharp peak volume.
  4. Use a vertical ruler to lock down the exact length ($L$) of the internal air column stretching from the cylinder edge to the water line.
  5. Repeat across a profile of varying tuning fork frequencies.
* **Graph & Analysis:**
  * Base equation: $L + e = \frac{\lambda}{4}$. Combined with $v = f\lambda$, this gives $L = \frac{v}{4}\left(\frac{1}{f}\right) - e$ ($e$ = minor end-correction).
  * Plot **Length ($L$) on the y-axis** against **$\frac{1}{f}$ on the x-axis**.
  * Gradient of the line: $\text{Gradient} = \frac{v}{4}$
  * Calculate constant: $v = 4 \times \text{Gradient}$
* **Accuracy / Exam Pitfalls:**
  * **Trap:** The resonance pocket doesn't break cleanly at the physical edge of the tube—it leaks slightly outward. The negative y-intercept value of your plot provides this exact end-correction calculation ($e$).

### 6. Determination of the Refractive Index of a Material
* **Goal:** Measure the precise index of refraction ($n$) of a dense transparent medium (glass or perspex block).
* **Apparatus:** Solid rectangular optical block, ray box, narrow single-slit plate, power transformer, white tracking paper, protractor, pencil.
* **Method:**
  1. Place the solid block flat in the center of the white paper page. Trace its geometric perimeter cleanly with a sharp pencil.
  2. Direct a crisp, narrow light beam from the ray box into the longer edge interface at a non-zero incident angle.
  3. Mark the incoming ray path and the outgoing emergent path with spaced locator dots. Lift the block and rule straight lines to bridge the trajectory inside the block bounds.
  4. Construct a perpendicular normal line ($90^\circ$) intercepting the boundary point where the ray entered the block.
  5. Use a protractor to gauge the angle of incidence ($i$) in the air zone and the angle of refraction ($r$) inside the block area.
  6. Shift the incoming light angle to collect a minimum of 6 diverse $i$ and $r$ coordinates.
* **Graph & Analysis:**
  * Base equation (Snell's Law): $n = \frac{\sin i}{\sin r}$.
  * Plot **$\sin i$ on the y-axis** against **$\sin r$ on the x-axis**.
  * Gradient of the line: $\text{Gradient} = n$ (Refractive Index)
* **Accuracy / Exam Pitfalls:**
  * **Tip:** Work exclusively with a finely sharpened pencil. Thick marker lines introduce high measurement uncertainty during protractor indexing, ruining accuracy.

### 7. Determination of Liquid Viscosity via Terminal Velocity
* **Goal:** Find the dynamic viscosity coefficient ($\eta$) of a thick liquid column (such as pure glycerol or washing liquid).
* **Apparatus:** Deep glass cylinder filled with test fluid, small precision steel ball bearings, pickup magnet, digital stopwatch, ruler, reference rubber bands.
* **Method:**
  1. Stretch rubber tracking bands around the outer walls of the deep cylinder at uniform spatial intervals (e.g., $10\text{ cm}$ apart). The top band must sit well below the surface level so the falling ball stabilizes to terminal velocity before passing it.
  2. Compute the exact radius ($r$) of a ball bearing sample by recording its diameter with a micrometer.
  3. Release the ball bearing perfectly down the center axis of the liquid column.
  4. Trigger the stopwatch as the sphere crosses the first baseline rubber band, logging split times at successive bands to verify stable uniform velocity.
  5. Calculate terminal velocity: $v = \frac{\text{distance between bands}}{\text{elapsed time}}$.
  6. Rerun testing routines using spheres of varied radii values.
* **Graph & Analysis:**
  * Base equation (Stoke's Law balancing): $v = \frac{2g(\rho_s - \rho_l)}{9\eta}r^2$.
  * Plot **Terminal Velocity ($v$) on the y-axis** against **$r^2$ on the x-axis**.
  * Gradient expression: $\text{Gradient} = \frac{2g(\rho_s - \rho_l)}{9\eta}$
  * Calculate constant: $\eta = \frac{2g(\rho_s - \rho_l)}{9 \times \text{Gradient}}$
* **Accuracy / Exam Pitfalls:**
  * **Tip:** The ball must fall perfectly down the central core axis. Moving too close to the structural container boundaries induces severe wall-effect drag, which slows the descent and skews viscosity calculations.

### 8. Investigation of the Wave Equation (Standing Waves)
* **Goal:** Validate the behavior of the resonant frequency ($f$) of a tensioned string across variations in vibrating length.
* **Apparatus:** Mechanical vibration generator, variable signal generator oscillator, high-tensile string, end pulley, slotted weights, metre ruler.
* **Method:**
  1. Anchor one end of the string to the mechanical vibration node. Run the free span across a low-friction end pulley, hanging fixed weights to generate constant static tension ($T = mg$).
  2. Activate the signal oscillator generator. Tune the output drive frequency until the string hits structural resonance, displaying a clean, wide single-loop envelope (fundamental first harmonic).
  3. Map the active vibrating distance ($L$) stretching between the generator piston knife-edge and the pulley apex via a ruler. Record the target drive frequency ($f$).
  4. Translate the physical position of the vibration platform to manually alter baseline path length ($L$). Re-tune oscillator frequencies to find the fundamental harmonic.
  5. Compile a dataset spanning a minimum of 6 discrete length variations.
* **Graph & Analysis:**
  * Wave mechanics: $v = f\lambda$. At the fundamental mode, $\lambda = 2L \implies f = \frac{v}{2}\left(\frac{1}{L}\right)$.
  * Plot **Frequency ($f$) on the y-axis** against **$\frac{1}{L}$ on the x-axis**.
  * Gradient of the line: $\text{Gradient} = \frac{v}{2}$
  * Calculate wave speed: $v = 2 \times \text{Gradient}$
* **Accuracy / Exam Pitfalls:**
  * **Tip:** Peak resonance loops are tough to balance by eye. Carefully adjust the frequency knob in fine $0.1\text{ Hz}$ increments back and forth until the absolute maximum vertical displacement amplitude is achieved.