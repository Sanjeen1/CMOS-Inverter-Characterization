# CMOS-Inverter-Characterization-
Comprehensive CMOS inverter characterization including VTC, noise margins, delay, rise/fall times, power analysis, and parameter sweeps using NGSpice

## **For line width and color in NGSpice -** 

<img width="191" height="89" alt="image" src="https://github.com/user-attachments/assets/f0780b24-bf2b-4b33-995b-9399eaa364e2" />

**set color0=white** --> Defines color0 as white. color0 is typically used for the background in waveforms/plots. So this sets the waveform window background to white.

**set color1=black** --> Defines color1 as black. Usually, color1 is used for grid lines or axes.

**set color2=red** --> Defines color2 as red. This color will be used for plotting the first waveform trace. 

**Set color3=blue** --> Defines color3 as blue. This color is used for the second waveform trace.

(Similarly, more colors can be defined for other traces if needed.)

**set xbrushwidth=3** --> Sets the brush width (line thickness) of waveforms to 3. This makes plotted traces thicker, which helps visibility.

## **For Rise and fall time -**

**T_rise** → the name of the measurement (SPICE will store result in this variable). trig v(out) val = 0.1*supply rise = 1 means "Start timing when v(out) crosses 10% of VDD on a rising edge." rise=1 means use the first rising crossing. targ v(out) val = 0.9*supply rise = 1 means "Stop timing when v(out) crosses 90% of VDD on the same rising edge."

**T_fall** = the measured fall time. Trigger: When v(out) crosses 90% VDD on a falling edge (fall=1). Target: When v(out) crosses 10% VDD on the same falling edge.

<img width="1255" height="177" alt="image" src="https://github.com/user-attachments/assets/a28616ee-99b5-4cf4-91b9-462d02dc5ce5" />

<img width="752" height="239" alt="image" src="https://github.com/user-attachments/assets/8bda0f51-049c-48bb-b270-b426d9470e42" />

**For Rise time -**

**Trigger:**
trig = 1.002941e-08 s → the instant when v(out) crossed 0.1·VDD on a rising edge.

**Target:**
targ = 1.004662e-08 s → the instant when v(out) crossed 0.9·VDD on that same rising edge.

✅ So the inverter output took 17.2 ps to rise from 10% to 90% of VDD.

## For propogation delay - 

<img width="1207" height="25" alt="image" src="https://github.com/user-attachments/assets/b33026cb-a2e0-4cc6-a187-56facc906c77" />

<img width="736" height="181" alt="image" src="https://github.com/user-attachments/assets/40947c7d-fc31-4f8e-acb6-b4b90738655a" />







