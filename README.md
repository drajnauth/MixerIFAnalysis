# MixerIFAnalysis
This program analyzes inputs and outputs from a mixer to identify frequencies that could fold back into the passband
The program assumes that an RF frequency is fed into a mixer along with an LO frequency which generates an IF frequency
The IF frequency may either be the sum RF+LO or the difference of RF-LO 

Enter the RF frequency along with the bandwidth expected for the frequency.  It is best to enter the middle frequenc of the BAND.
For bandwidth, it is best to enter the entire bandwidth of the BAND (e.g. 250000)

Next, enter the IF frequency that is expected to be generated along with the bandwidth of the IF signal. If the IF is feeding
a crystal filter, then enter the bandwith of the crystal filter (e.g. 3000)

You now select how the IF is generated. Select the sum (RF+LO) or difference (RF-LO) button.  The program will automatically
calculate the LO frequency.

You can specific if the LO frequency will be a square wave.  If a square wave is used, then the first 4 harmonics of the square wave 
will be used in the analysis. If unchecked, a Sine wave is assumed and 3 harmonics will be used for the analysis. 

If the radio will have a BPF as part of the Transmit (TX) chain, select the BPF analysis button and then enter the appoximate 
bandwidth (e.g. 400000).  This is used to determine if any fequencies will fold back into the passband of the BPF which is around 
the specified RF frequency.

Finally, select the type of analysis needed.  Harmonic Analysis only means that only harmonics of the LO and BFO will be mixed 
together to see if any frequencies fold back to interfere with the RF frequency or the IF frequencies during Receive (Rx) or 
Transmit (Tx).

The Harmonic & Byproduct analysis will also identify if any of the mixed artifacts will interfere with each other and interfere
with the RF or IF.  It is important to carefully observe the frequencies that mix together. In majority of cases there frequencies 
are so high that their power level will be very small and may be noise. That is it may not be strong enought to cause interference.  
