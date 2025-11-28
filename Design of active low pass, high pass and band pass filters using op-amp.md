# EC1421-19EC421-Analysis-and-Design-of-Analog-ICs
# DESIGN OF ACTIVE LOW PASS,HIGH PASS AND BAND PASS FILTERS USING OP-AMP 

## AIM: 

To design and obtain the frequency response of 
i) First order Low Pass Filter (LPF) 
ii) First order High Pass Filter (HPF) 
iii) Band pass filter
 
## APPARATUS REQUIRED

<img width="625" height="170" alt="image" src="https://github.com/user-attachments/assets/900fc8b3-3a8c-4208-bf52-98cc9e281e21" />

## THEORY
## LOW PASS FILTER 
 A LPF allows frequencies from 0 to higher cut of frequency, fH.  At fH the gain is 0.707 
Amax, and after fH gain decreases at a constant rate with an increase in frequency.  The gain 
decreases 20dB each time the frequency is increased by 10.  Hence the rate at which the gain 
rolls off after fH is 20dB/decade or 6 dB/ octave, where octave signifies a two fold increase in 
frequency.  The frequency f=fH is called the cut off frequency because the gain of the filter at this 
frequency is down by 3 dB from 0 Hz.  Other equivalent terms for cut-off frequency are -3dB 
frequency, break frequency, or corner frequency.
# HIGH PASS FILTER 
The frequency at which the magnitude of the gain is 0.707 times the maximum value of 
gain is called low cut off frequency.  Obviously, all frequencies higher than fL are pass band 
frequencies with the highest frequency determined by the closed –loop band width all of the op
amp. 
# BAND PASS FILTER 
A band pass filter has a pass band between two cutoff frequencies fH and fL such that fH > 
fL.  Any input frequency outside this pass band is attenuated.  There are two types of band-pass 
filters.  Wide band pass and Narrow band pass filters.  We can define a filter as wide band pass if 
its quality factor Q <10.  If Q>10, then we call the filter a narrow band pass filter.  A wide band 
pass filter can be formed by simply cascading high-pass and low-pass sections.  The order of 
band pass filter depends on the order of high pass and low pass sections.

## CIRCUIT DIAGRAM: 
## LOW_PASS
<img width="1108" height="553" alt="image" src="https://github.com/user-attachments/assets/7296d916-920a-4412-a8f5-4a2cdc265110" />

## HIGH-PASS
<img width="964" height="458" alt="image" src="https://github.com/user-attachments/assets/12429343-0c29-4b3a-bda5-da9952b79ab7" />

## BAND-PASS
<img width="1226" height="618" alt="image" src="https://github.com/user-attachments/assets/c70d6897-f0e4-462c-a4f4-ae7d03742a65" />


## MODEL GRAPH:
## LOW_PASS
<img width="923" height="426" alt="image" src="https://github.com/user-attachments/assets/a90521d5-76e9-4e0e-ab47-ede0585fc55a" />

## HIGH-PASS
<img width="1209" height="573" alt="image" src="https://github.com/user-attachments/assets/f9c7544c-dce6-43a8-b3d5-2942d41e5d74" />

## BAND-PASS
<img width="1366" height="603" alt="image" src="https://github.com/user-attachments/assets/83845f6f-7d65-446b-95ea-95c9860a2f03" />

## PROCEDURE - (LPF & HPF): 
1. Connect the circuit as shown in the circuit diagram. 
2. Select the corresponding cut-off frequency (higher or lower) and determine the value of C&R. 
select the value of R1 & Rf depending on desired passband gain Af.. 
3. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
4. Tabulate the output voltage Vo with respect to different values of input frequency. 
5. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to  get approximately the same characteristic as shown in the model graph. 
# PROCEDURE:BAND PASS FILTER 
1. Select the lower and higher cut-off frequency and calculate the value of R & C for the given 
frequencies. 
2. Design for LPF & HPF separately and then combine the circuit by first placing the HPF 
followed by a LPF (i.e) HPF in series with LPF. 
3. Connect the circuit as shown in the circuit diagram. 
4. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
5. Tabulate the output voltage Vo with respect to different values of input frequency. 
6. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to get approximately the same characteristic as shown in the model graph

## DESIGN:LPF & HPF:

<img width="429" height="324" alt="image" src="https://github.com/user-attachments/assets/b0f0ac0a-3006-494c-9096-e91ae2d6e87c" />

# DESIGN: BAND PASS FILTER
Design a BPF to pass a band of 400Hz to 2KHz with a pass band gain of 4.  
1. Select the highest cut-off frequency of LPF as fH = 10 KHz and the lowest cut-off frequency 
of HPF as fL = 1 KHz.  
2. Design the HPF first by taking fL = 1KHz. Assume the value of C < 1μf.  
Let C = 0.1μf.  
3. Calculate R from the expression.  
Given: fH = 2KHz  = 1/ (2πR1C1) 
   Let C1 = 0.1 µF, R1 = 7.9 KΩ 
Given: fL = 400Hz  = 1/ (2πR2C2) 
   Let C2 = 0.1 µF, R2 = 39.8 KΩ 
  Pass band Gain=4 
   Now   Ao = 1 + (Rf / R1)  
               2-1=(Rf / Ri) 
                Ri = Rf 
                 Let  Ri = Rf = 10 KΩ
## TABULATION:
## LOW_PASS
<img width="426" height="306" alt="image" src="https://github.com/user-attachments/assets/2ea19940-7b77-49e9-a2f4-4952dde30264" />

## HIGH-PASS
<img width="426" height="293" alt="image" src="https://github.com/user-attachments/assets/37886302-3c00-49a6-83f8-cd5cf1f49504" />

## BAND-PASS
<img width="908" height="435" alt="image" src="https://github.com/user-attachments/assets/c34d1810-a1a3-4e62-a919-d15a2a271a08" />

## CALCULATIONS:
## LOW_PASS
<img width="1333" height="313" alt="image" src="https://github.com/user-attachments/assets/c0ade697-6d9f-452a-886e-b8509c0bc976" />

## HIGH-PASS
<img width="1286" height="546" alt="image" src="https://github.com/user-attachments/assets/dea2e229-f84a-42bf-908f-c7b72b0a1db7" />

## BAND-PASS
<img width="1038" height="516" alt="image" src="https://github.com/user-attachments/assets/71b85621-be3e-4ec3-9aa1-5622283e451d" />

## Model Graph
## LOW_PASS
<img width="1109" height="648" alt="image" src="https://github.com/user-attachments/assets/fbb0e879-d945-4188-804b-75a89d5ffb43" />

## HIGH-PASS
<img width="1223" height="619" alt="image" src="https://github.com/user-attachments/assets/290651ef-77b5-4f3e-a53a-389d692dc385" />

## BAND-PASS
<img width="1287" height="583" alt="image" src="https://github.com/user-attachments/assets/5ccf55d0-a8fe-4f59-b208-e25a735801b7" />

## GRAPH:
## LOW_PASS
<img width="1066" height="951" alt="image" src="https://github.com/user-attachments/assets/8bdd040e-42e6-47f5-8055-20c82e0122dc" />

## HIGH-PASS
<img width="724" height="540" alt="image" src="https://github.com/user-attachments/assets/e4060b3c-9dac-453d-9dca-54a00a5b6d55" />

## BAND-PASS
<img width="672" height="549" alt="image" src="https://github.com/user-attachments/assets/a6693b5f-69a5-4dd8-ba08-51d2abf6f7eb" />

 ## RESULTS:
Thus an Active Low pass, High pass and Band Pass Filters are designed and 
tested using op-amp IC 741. 

