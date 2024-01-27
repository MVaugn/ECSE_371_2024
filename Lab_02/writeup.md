# Lab 2: OpAmps

Mark and Jim

## Q1

![]()
Figure: Q1 Schematic

**With Vin = 0 (input tied to ground), measure and record the DC output voltage with a DMM. What voltage do you expect, and what do you measure? Can you explain?** Vo = -575nV. In the ideal case, its expected to be a Vo = 0V. However, the nonideal input offset voltage of a real world op amp leads to a drift in the output voltage at equilibrium.

**Provide a 0.10 Vpp 10KHz sinewave input. Measure and record the gain of the amplifier and explain why the gain does not equal 100.** 

$V_{pkpk, in} = 64mV$

$V_{pkpk, out} = 551mV$

The gain doesn't equal 100 because the input resistance was designed to be $1k\Omega$, so the signal si being significantly attenuated.

**With a 0.10 Vpp 1KHz sinewave input, slowly increase the input voltage as you observe the amplifier
output waveform; look for saturation. Measure and record the maximum positive and negative voltage
swings:**

Bottom rail saturation:
Output = -11.1V
Input = 1.0V

Top rail saturation:
Output = 12.7V
Input = -1.8V

**Why is output voltage swing important? ** Output voltage swing determines the absolute min/max of your input signal, defining the usable range for a given gain.