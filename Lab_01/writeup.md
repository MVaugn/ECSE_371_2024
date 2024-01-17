# Lab 1 #
Mark Vaughn and Jim Horwitz

## Q1 ##
## Q2a ##
## Q2b ##
## Q3a ##
## Q3b ##
## Q4 ##

## Q5 ##
What practical considerations should you keep in mind when determining the magnitude of these components (what are the compromises and penalties)? *Lower resistor values will lead to higher max output current and more power distributed to the load, but at the cost of a higher runtime current, more heat lost, and worse ripple rejection. A higher resistance is the inverse, improved ripple rejection, lower runtime current, and less heat lost at the cost of worse max output current performance and less power distributed to the load*

Figure [x]: Voltage divider schematic

## Q6 ##
Center frequency is 10 kHz.

We chose our resistor to be __ because __.

We then chose our capacitor to be __ because __.

Figure [x]: Schematic and plots for your Saturday Schematic.

Figure [x]: Breadboard your LP filter

Figure [x]: Time-domain check of LPF

Figure [x]: Bode Plot of LPF


## Q7 ##
Figure [x]: RC Band Pass Schematic

## Q7a ##
Using the simulated frequency-domain plot, determine the center-frequency of the bandpass filter. *GREAT QUESTION LARRY*

Calculate and record the Q of the filter. *GREAT QUESTION LARRY*

## Q7b ##
Does it matter which filter, the low-pass or the high-pass, is placed first in your circuit? Investigate this with CircuitLab and explain *GREAT QUESTION LARRY*

## Q7c ##
Figure [x]: Time domain check of RC Bandpass
Figure [x]: Bode Plot of RC Bandpass

## Q7d ##
How close did your breadboard match the simulated results? Record your observations *GREAT QUESTION LARRY*

## Q8 ##
Figure [x]: Schematic of Parallel LC Resonant Passband Filter.

Figure [x]: Plots of Parallel LC Resonant Passband Filter.
## Q8a ##
Using the simulated frequency-domain plot, determine the center-frequency of the bandpass filter.  *GREAT QUESTION LARRY*

Calculate and record the Q of the filter *GREAT QUESTION LARRY*

## Q8b ##
Breadboard your circuit. After performing a quick time-domain check with the oscilloscope (input versus output), perform a Frequency Domain Plot of your breadboarded circuit using the Frequency Response  Analysis (Bode Plot) feature of your oscilloscope.  Record the Bode plot (P).

Figure [x]: Picture of Setup
Figure [x]: Time Domain Output of Scope
Figure [x]: Bode Plot Output of Scope

## Q8c ##
How close did your breadboard match the simulated results? *GREAT QUESTION LARRY*

Record your observations. *GREAT QUESTION LARRY*

## Q8d ##
How does the performance of this filter compare to that of the 2-stage RC bandpass filter in Problem 7?  Record and explain your observations. *GREAT QUESTION LARRY*

What might explain the differences that you observe? *GREAT QUESTION LARRY*

## Q9 ##
Figure [x]: Differentiator Schematic

## Q9a ##
Record waveforms as you change function generator amplitude and frequency.

Figure [x]: Waveforms with changing generator amplitude and frequency

Be prepared to discuss waveforms and operation of the circuit. (Use the capacitor  “axiom”). *Capacitor acts as a high pass filter, adding a zero to the filter around a low frequency. Low frequencies are dropped, while higher frequencies remain. Often times, this means that only the harmonics of a signal (eg square wave) are kept while the original signal is mostly destroyed.*

## Q9b ##
How does the output change shape as the duty cycle, frequency, and amplitude of the input are increased and decreased? *GREAT QUESTION LARRY*

Figure [x]: Output of Differentiator with changes in duty cycle, frequency, and amplitude

## Q9c ##
What components of the input waveform is the filter passing? *A differentiator is a high-pass filter, which means it keeps the high frequencies while dropping the lower frequencies.*

## Q10 ##

Figure [x]: Scope Trace:

## Q10a ##
Figure [x]: Integration Schematic

## Q10b ##
What is the relationship of  (average) DC output voltage vs duty-cycle and frequency of the input? In other words, how does the average DC voltage change with changes at the input? *Frequency has no effect on the DC filtered voltage as the average voltage doesn't change. However, a higher frequency input wave will make the pk-pk ripple less, as the time that the capacitors are charging/discharging is shorter per cycle. As the duty cycle increases, the average DC voltage will also increase.*
## Q10c ##
How does the load affect the ripple? *Load will make ripple worse as the capacitor filtering the input signal will discharge faster.*

DC output voltage vs load? *The DC output voltage on average versus a load should stay the same, however the ripple may make it very unstable, so much so that its difficult to even characterize as DC.*

How would you define the value of a DC voltage that has ripple? *Value +/- %ripple*

Figure [x]: Ripple Scope Traces

## Q10d ##
What happens to the output when the input to your filter is the 1KHz, -3V to +3V square wave from Problem 10?  *GREAT QUESTION LARRY*

What can you conclude about the average value of a square wave or sinewave? *If the square wave has a perfect 50% duty cycle, the average voltage will always be half of the pk-pk voltage. Sine waves are the same; with a voltage centered around half the pk-pk voltage of the wave.*

## Q10e ##
Select values for an integrator which will convert the 1KHz, -3V to +3V square wave to a reasonable sine wave.*GREAT QUESTION LARRY*

How can you improve the “quality” (harmonic distortion) of the sine wave?*GREAT QUESTION LARRY*

What happens to the amplitude of the sine wave as its quality improves?*GREAT QUESTION LARRY*

Figure [x]: Demonstration of ripple quality improvement
## Q10f ##
Thinking of the integrator as a filter, what components of the input waveform are being passed by the filter? *The low frequency components of the input waveform are being passed, while the high frequency components are dropped.*

## Q10g ##
Try adding an integrator stage to improve the sine wave quality.  Keep the load the same.Why does adding the stage help? *Adding a second stage helps remove any high frequency unwanted noise from the input signal, or external EMF noise injected into the system.*


## Q11 ##
Be sure that the current limit on your bench power supply is set to maximum.  Why? *Set the current limit to maximum bc the transient current at the spike of the lamp will further emphasize the spike able to be used for the timing circuit.*

Schematic image here
\* keep the breadboard and circuit working for recitation!