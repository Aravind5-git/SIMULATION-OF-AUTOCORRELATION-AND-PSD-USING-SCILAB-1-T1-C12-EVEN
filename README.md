# SIMULATION-OF-AUTOCORRELATION-AND-PSD-USING-SCILAB-1-T1-C12-EVEN
AIM:

Write a program for Autocorrelation and PSD of signals in SCILAB and verify Wiener-Khinchin relation.

EQUIPMENTS Needed:

.Computer with i3 Processor

.SCI LAB

THEORY:

The Wiener-Khinchin theorem states that the power spectral density of a wide sense stationary random process is the Fourier transform of the corresponding autocorrelation function.

Algorithm:

1.Load or Define the Signal: Input your time-domain signal.

2.Compute Autocorrelation: Calculate the autocorrelation function of the signal.

3.Compute Power Spectral Density (PSD): Estimate the PSD of the signal, either directly using a method like Welch’s periodogram or by using the Fourier transform of the autocorrelation.

4.Plot Results: Visualize the autocorrelation function and PSD.

PROCEDURE:

Refer Algorithms and write code for the experiment.

Open SCILAB in System

Type your code in New Editor

Save the file

Execute the code

If any Error, correct it in code and execute again

Verify the generated waveform using Tabulation and Model Waveform

PROGRAM:
```
clc
clear all; 
t=0:0.01:2*%pi;
x=19*cos(2*t);
subplot(3,2,1);
plot(x);
au=xcorr(x,x);
subplot(3,2,2);
plot(au);
v=fft(au);
subplot(3,2,3);
plot(abs(v));
fw=fft(x);
subplot(3,2,4);
plot(fw);
fw2=(abs(fw)).^2;
subplot(3,2,5);
plot(fw2);
```

OUTPUT GRAPH:

<img width="610" height="460" alt="image" src="https://github.com/user-attachments/assets/399e93b8-2914-48d3-8a72-1c97c4ac357e" />

RESULT:

<img width="1600" height="895" alt="image" src="https://github.com/user-attachments/assets/ffc9e3ae-dbf8-4101-b8be-cec973dca592" />
