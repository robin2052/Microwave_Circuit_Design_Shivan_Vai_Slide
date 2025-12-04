# Harmonic Distortion

<img width="1081" height="791" alt="image" src="https://github.com/user-attachments/assets/271d83f4-81e3-49ae-8bd9-6f1ff293f89f" />

<img width="1074" height="783" alt="image" src="https://github.com/user-attachments/assets/d8e3dd38-f314-42f0-9189-62710b089761" />

<img width="1186" height="350" alt="image" src="https://github.com/user-attachments/assets/ee61a6d0-c77d-426f-a7e1-e717c1b3c576" />

# Why does harmonic distortion happen?

Because real amplifiers are not perfectly linear.
When you increase the input power, the active device (BJT, MOSFET, HEMT) enters:

Nonlinear gm region

Soft compression

Hard clipping

Saturation

As a result, the output waveform gets "bent", creating harmonic components.

# Types of Harmonic Distortion

<img width="1239" height="530" alt="image" src="https://github.com/user-attachments/assets/4c60af52-f641-4f1c-bd5a-1ea944f17658" />

# Why harmonic distortion is important in RF & Microwave?
Because harmonics can:
Interfere with adjacent channels,
Cause spectral regrowth,
Reduce EVM / degrade modulation accuracy,
Harm compliance with FCC/ETSI standards,
Cause receiver blocking,
Reduce power amplifier efficiency due to unwanted outputs,
For LNAs:
→ Low harmonic distortion = better linearity, IMD, IIP3, SFDR

# How to reduce harmonic distortion?
## Increase Linearity of the transistor
1.Use larger transistor
2.Bias at a more linear region ( Class A bias)
3.Increase vgs bias on mosfet/ Vf bias on Bjt
4.Keep gain small signal ( avoid compression)

## Use feedback

1.Resistive feedback reduces distortion
2.But can reduce gain

## Use degeneration

1.Source/emitter degeneration linearizes gm
2.Trade-off: reduces gain/noise

## Improve matching

Proper input/output matching keeps device in linear zone

## Reduce input power

1.Avoid P1dB region
2.Avoid saturation

# Some Important Parameters to know 

## P1dB (1-dB Compression Point)
<img width="1221" height="588" alt="image" src="https://github.com/user-attachments/assets/0899936f-82a8-4ce5-b199-b3590d83e293" />
For More about the 1db Compression Point click on this link - https://www.allaboutcircuits.com/technical-articles/using-the-1-db-compression-point-to-characterize-rf-system-nonlinearity/


## IMD3 (Third-Order Intermodulation Distortion)
<img width="1107" height="519" alt="image" src="https://github.com/user-attachments/assets/7b2f0df1-3c9b-4d11-a488-9bdb88f8c62e" />
For More about third order intermodultaion distortion click on this  link - https://www.allaboutcircuits.com/technical-articles/understanding-intermodulation-distortion-and-the-third-order-intercept-point-in-rf-systems/










