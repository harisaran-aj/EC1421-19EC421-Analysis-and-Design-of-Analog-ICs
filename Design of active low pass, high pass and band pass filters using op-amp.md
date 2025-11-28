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
![WhatsApp Image 2025-11-29 at 00 00 28_0003ffa9](https://github.com/user-attachments/assets/e46e3e80-f488-450f-a68c-00e41bc63ff0)

## HIGH-PASS

![WhatsApp Image 2025-11-29 at 00 00 28_c33f1408](https://github.com/user-attachments/assets/f9742719-aeee-455c-8807-c555f1dc26e2)

## BAND-PASS

![WhatsApp Image 2025-11-29 at 00 00 28_213efd0e](https://github.com/user-attachments/assets/8fcfbcd9-ba1a-4215-9c9a-64e26e343fee)

## MODEL GRAPH:
## LOW_PASS

![WhatsApp Image 2025-11-29 at 00 00 29_93ca965f](https://github.com/user-attachments/assets/b46b0131-e0e2-4aaf-b5f0-ecac08e54f3b)

## HIGH-PASS

![WhatsApp Image 2025-11-29 at 00 00 29_decef920](https://github.com/user-attachments/assets/2806838e-57a2-49d4-a718-86d369772d96)

## BAND-PASS

![WhatsApp Image 2025-11-29 at 00 00 29_d240d72a](https://github.com/user-attachments/assets/46b21ec2-1d19-45d3-b248-7dea5cadd3d9)

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

![WhatsApp Image 2025-11-29 at 00 05 07_72b9bed3](https://github.com/user-attachments/assets/7ffebc0a-f363-4e52-9c51-650860ba3780)

## HIGH-PASS

![WhatsApp Image 2025-11-29 at 00 05 07_17b9f68d](https://github.com/user-attachments/assets/c6590aeb-3245-41a9-84d2-20d9bd0a9840)

## BAND-PASS

![WhatsApp Image 2025-11-29 at 00 05 07_53d18045](https://github.com/user-attachments/assets/152f9094-5c06-425b-a0d4-eeeab42117a4)

## GRAPH:

## LOW_PASS

![WhatsApp Image 2025-11-29 at 00 06 43_0e3562c9](https://github.com/user-attachments/assets/e23fde35-a9b7-4999-880b-d93b7b83642a)

## HIGH-PASS

![WhatsApp Image 2025-11-29 at 00 06 43_5994abc2](https://github.com/user-attachments/assets/31b6e645-3280-40dc-bb52-c818255d387e)

## BAND-PASS

![WhatsApp Image 2025-11-29 at 00 06 43_c4c7cc14](https://github.com/user-attachments/assets/cfac86d2-a083-4c59-9fc1-e5a974dfeca3)

 ## RESULTS:
Thus an Active Low pass, High pass and Band Pass Filters are designed and 
tested using op-amp IC 741. 

